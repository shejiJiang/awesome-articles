收集前端好文章并总结

## [哪些技术会决定前端开发者的未来发展](https://mp.weixin.qq.com/s/BOtrzkQbGMC5EQces-cD0w)
    1.不要盲目追寻社区的热点，有时只是学会了换个语言实现了增删改；
    2.typescript值得学习，它引入了类型机制、静态编译能力解决了生产力的问题，并且各大框架都在往ts上靠；
    3.图形技术(canvas/webgl)，它不可能成为前端的热门技术，但却是前端开发者进阶必学的技术，因为它直接操作了图形接口；
    4.编辑器领域技术，小众领域、webIDE的出现使得这一领域的人才需求变多；
    others:Serverless(会火)、IOT(看不到进展，js in iot没能解决耗能问题)、GraphQL(一直没火，不是技术本身问题，是损害了后端开发利益)、AI In FE(目前和前端交集少，就算有也是调包侠)

## [图解浏览器的工作原理](https://mp.weixin.qq.com/s/X4yAFZBNLwaDUFYaR0Cn5g)
    1.chrome浏览器是多进程工作方式(浏览器进程(ui-thread、network-thread、storage-thread)、渲染进程、GPU进程、插件进程等)；
    2.输入地址到渲染页面过程，输入处理(ui-thread)->开始导航(ui-thread)->读取响应(network-thread)->查找渲染进程(ui-thread)->确认导航->渲染进程渲染；
    3.渲染进程的工作，构建dom树->样式计算(css树)->布局(布局树)->绘制各元素->合成帧；
    4.事件处理，渲染主线程利用合成器渲染，对于快速滚动区域的滚动事件合成器直接合成，对于其它事件会先交给主线程；
