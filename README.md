- [digi](https://github.com/digi1874/digi)
- [digi 文档](https://digi1874.github.io/digi-doc/1.0.4/index.html)
- [demo](https://github.com/lin09/digi-demo)
- [digi-router](https://github.com/digi1874/digi-router)
- [digi-router 文档](https://digi1874.github.io/digi-router/docs/digi-router/1.0.1/index.html)
- [digi-classname](https://github.com/digi1874/digi-classname)
- [digi-refs](https://github.com/digi1874/digi-refs)


```
// 简单例子
import digi, { createData } from 'digi'

// 创建监听数据
const data = createData({ a: 123 })

// 添加元素
digi({ text: data.$tp('a') })

console.log(document.body.lastChild.outerHTML)
// => <div>123</div>

data.a = 321
// => watch a => newVal: 321, oldVal: 123

console.log(document.body.lastChild.outerHTML)
// => <div>321</div>
```
