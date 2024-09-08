# OpenAI API JsonschemaEditor (依赖Jquery)
用于可视化生成符合OpenAI Jsonschema模式的json字符串js库

# 使用示例
* 1.页面中引入 `jsonschemaEditor.js` 和 `jquery` 以及`fontawesome.com/v5`

* 2.示例代码
  ```html
  <!DOCTYPE html>
  
  <html lang="zh-cn" xmlns="http://www.w3.org/1999/xhtml">
  <head>
      <meta charset="utf-8" />
      <title>JsonschemaEditor</title>
      <script src="https://code.jquery.com/jquery-3.6.0.min.js"></script>
      <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.3/css/all.min.css">
      <script src="jsonschemaEditor.js"></script>
  </head>
  <body>
      <div id="editor"></div>
      <script>
          var jsonschemaeditor = JsonSchemaEditor.create($("#editor"), {
              schema: '',//如果创建时赋值，会直接进行可视化渲染
              onSave: function (schema) {
                  //保存操作
                  alert(schema);
              }
          });
          jsonschemaeditor.getSchema();//编辑后获取生成的jsonschema字符串
      </script>
  </body>
  </html>
  ```
  * 示例图1
  ![image](https://github.com/user-attachments/assets/e0bd79b8-25ce-48e9-bbe7-184096d78016)
  * 示例图2
  ![image](https://github.com/user-attachments/assets/194f8d61-de62-45a3-8f92-b4a2b7c40f53)



