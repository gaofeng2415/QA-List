**Q：el-form-item添加提示信息，校验出错时隐藏该怎么做？**

A: 可以通过设置自定义属性+自定义class来实现。具体demo如下：
```html
<el-form-item class="show-underline-tip" data-underline-tip="这是行下信息">
 <!-- 任意内容 -->
</el-form-item>
```
```scss
.show-underline-tip:not(.is-error) {
  // 这里有疑问，如何将伪元素下放到el-form__content下？
  &:before {
    content: attr(data-underline-tip);
    position: absolute;
    bottom: 0;
    left: 0;
    color: #606266;
    font-size: 12px;
  }
}
```
