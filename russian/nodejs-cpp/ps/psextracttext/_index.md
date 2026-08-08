---
title: "AsposePSExtractText"
second_title: "Aspose.Page для JavaScript через C++"
description: "Извлечь текст из PS-файла"
type: docs
weight: 10
url: /ru/nodejs-cpp/ps/psextracttext/
---
## AsposePSExtractText function

Извлечь текст из PS-файла. Текст может быть извлечён только в том случае, если он написан шрифтом Type 42 (TrueType) или шрифтом Type 0 с шрифтами Type 42 в его Vector Map.

```js
function AsposePSExtractText(
    fileBlob,
    fileName, 
    start,
    end
)
```

| Параметр | Тип | Описание |
| --------- | ---- | ----------- |
| fileBlob | Объект Blob | Содержимое исходного файла. |
| fileName | string | Имя исходного файла. |
| начало | int | Указывает страницу, с которой начинать извлечение текста. Этот параметр полезен для многостраничных документов. |
| конец | int | Указывает страницу, до которой следует завершить извлечение текста. Этот параметр полезен для многостраничных документов. |

### Возвращаемое значение

Объект JSON
| Поле | Описание |
| ----- | ----------- |
|  | errorCode | код ошибки (0 нет ошибки) |
|  | errorText | текстовая ошибка ("" нет ошибки) |
|  | текст | извлечённый текст |

### Примеры

```js
  var fPSExtractText = function (e) {
    const file_reader = new FileReader();
    file_reader.onload = (event) => {
      const json = AsposePSExtractText(event.target.result, e.target.files[0].name);
      if (json.errorCode == 0) {
        document.getElementById('output').textContent = "Text:" + json.text;
      }
      else 
        document.getElementById('output').textContent = json.errorText;
    }
    file_reader.readAsArrayBuffer(e.target.files[0]);
  }
```

**Web Worker example**:
```js

  /*Create Web Worker*/
  const AsposePageWebWorker = new Worker("AsposePageforJS.js");
  AsposePageWebWorker.onerror = evt => console.log(`Error from Web Worker: ${evt.message}`);
  AsposePageWebWorker.onmessage = evt => document.getElementById('output').textContent = 
    (evt.data == 'ready') ? 'library loaded!' :
      (evt.data.json.errorCode == 0) ? 
        ((evt.data.operation == 'AsposePSExtractText') ? `Text: ${evt.data.json.text}` : `` ) : `Error: ${evt.data.json.errorText}`;

  /*Event handler*/
  const fPSExtractText = e => {
    const file_reader = new FileReader();
    file_reader.onload = event => {
      AsposePageWebWorker.postMessage({ "operation": 'AsposePSExtractText', "params": [event.target.result, e.target.files[0].name] }, [event.target.result]);
    };
    file_reader.readAsArrayBuffer(e.target.files[0]);
  };

```

### См. также

* function [AsposePSGetBoundingBox](../psgetboundingbox/)
