1.通过该项目，请简要说明 typescript 比 javascript 的优势在哪？

​	答:  javascript中类型检查较弱，一般的错误都需要在执行的过程中遇到才会有错误，一些小错误可能不太容易发现，但是在Typescript 类型检查是比较严格，对接口的参数以及返回值，类型判断都有实时的错误警告，避免了大多数运行中的错误

2.请简述一下支付流程

​	答: 客户端向服务器发送订单信息以及订单价格   服务端返回支付宝的支付地址，支付后成功后，支付宝会向服务端post一个支付状态，并且跳转到之前设定的返回地址

3.react-redux 的主要作用是什么，常用的 api 有哪些，什么作用？

​	答:  统一管理项目的数据状态，以及进行变更数据状态的数据方法，常用API 有applyMiddleware  createStore，createStore用于创建一个store对象，其中保存了数据状态和数据方法，applyMiddleware  用于添加中间件

4.redux 中的异步如何处理？

​	答: 通过在applyMiddleware  中添加saga中间件，在store的数据处理链条中添加saga方法处理环节，将异步函数书写在saga中，在异步函数处理完成，再执行reducer方法进行数据状态变更