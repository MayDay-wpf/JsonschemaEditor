# JsonschemaEditor (依赖Jquery)
用于可视化生成符合OpenAI Jsonschema模式的json字符串js库

# 使用示例
* 1.页面中引入 `jsonschemaEditor.js` 和 `jquery`

* 2.示例代码
  ```javascript
  <script src="../jquery.js"></script>
  <script src="../jsonschemaEditor.js"></script>
  <div id="editor"></div>
  <script>
  var jsonschemaeditor = JsonSchemaEditor.create($("#editor"), {
            schema: '',//如果创建时赋值，会直接进行可视化渲染
            onSave: function (schema) {
               //保存操作
            }
        });
  jsonschemaeditor.getSchema();//编辑后获取生成的jsonschema字符串
  </script>
  ```
  * 示例图
  ![image](https://github.com/user-attachments/assets/e0bd79b8-25ce-48e9-bbe7-184096d78016)
