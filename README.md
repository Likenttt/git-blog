# git-blog
记录. 


## Electron 

#### [Electron中主线程（main）和渲染线程（renderer）为什么要使用ipc通信](https://stackoverflow.com/questions/67344365/electron-why-do-we-need-to-communicate-between-the-main-process-and-the-render)
为了避免资源泄漏以及安全风险，不要在渲染线程中使用node的api（nodeIntegration set为false，注意是否真实使用了），可以通过ipc给主线程发送消息，让主线程来处理，处理完再交给渲染线程
![image](https://user-images.githubusercontent.com/26034018/147847420-e984df62-97d9-4cf2-a810-524b441ace3a.png)

#### [js异步函数中的的变量如何返回](https://stackoverflow.com/questions/23667086/why-is-my-variable-unaltered-after-i-modify-it-inside-of-a-function-asynchron)

