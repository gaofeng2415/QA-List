**Q：如何在marked.js中，自定义渲染并且渲染成vue的自定义组件？**

A: marked.js中，自定义渲染，需要使用renderer.js中的renderer.js中的方法，具体可以参考官方文档：https://marked.js.org/#/USING_PRO.md
**TODO...**

**Q：由于接口返回是流式数据，如何让流式数据搭配marked.js渲染成html？**
A: 由于接口返回是流式数据，单片数据可能解析失败。目前我们没有好的解决方案，只能拿到全部数据，然后使用marked.js解析成html。
**TODO...**