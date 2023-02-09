# Vue3 学习笔记

## 1、ubuntu 安装 vue

先安装 nodejs sudo apt install nodejs
安装 npm sudo apt install npm
最后安装 vue sudo npm install vue-router

## 2、本地使用 vue

在 header 里使用如下方式引用:

<script src="js/vue3.js"></script>

使用vue有固定的结构:

```html
    <!-- 这里是一个模板 这有点类似go/template -->
    <!-- 而且这里 不一样的是 当我们在浏览器修改num的值的时候 这里counterz的值也发生了变化 -->
    <!-- vue实现了双向绑定 -->
    <div id="counter">
        <h1>counter:{{ num }}</h1>
    </div>

    <script>
        const Counter={
            data:function(){
                return {
                    num:0
                }
            }
        }
        <!-- 创建一个应用,将配置的对象counter的内容渲染到选择器#counter的元素上 -->
        Vue.createApp(Counter).mount("#counter")
    </script>
```

## 3、使用脚手架工具

命令:
```bash
npm init vite-app <project-name>
```
进入项目:
安装然后运行：
```bash
npm install
npm run dev
```