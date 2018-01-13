菜鸟教程上react学习：

[1]index.html---最基础的react应用，输出hello world

* react.min.js - React 的核心库

* react-dom.min.js - 提供与 DOM 相关的功能

* babel.min.js - Babel 可以将 ES6 代码转为 ES5 代码，这样我们就能在目前不支持 ES6 浏览器上执行 React 代码。Babel 内嵌了对 JSX 的支持。通过将 Babel 和 babel-sublime 包（package）一同使用可以让源码的语法渲染上升到一个全新的水平。

[2]create-react-app/my-app

* 通过create-react-app命令快速创建react项目

* 项目基于Webpack+ES6

[3]JSX

* 嵌入多个html标签，需要使用一个div元素包裹它们，添加自定义属性需要使用data-前缀;

* 独立文件 可以将React JSX代码放在一个独立文件中；

* 表达式写在{}---JSX中不能使用if else语句，但可以使用conditional(三元运算)表达式来替代;

* 样式--camelCase语法设置内联样式,--react会在指定元素数字后自动添加px;

* 标签内的注释要写在花括号中，标签外的注释不需要写在括号内;

* JSX允许在模板中插入数组，数组会自动展开所有成员。

* React可以渲染---html标签 vs react组件
  ----React 的 JSX 使用大、小写的约定来区分本地组件的类和 HTML 标签。
  
    * 要渲染HTML标签，只需要在JSX中使用小写字母的标签名；
    
    * 要渲染React组件，只需要创建一个大写字母开头的本地变量；
    
[4]react组件：

* -React.createClass方法用于生成一个组件类HelloMessage

* -<HelloMessage/> 实例组件类并输出信息--react自定义组件类必须以大写字母开头

[5]React把组件看做是一个状态机，通过与用户的交互，实现不同的状态，然后渲染UI.让用户界面和数据保持一致。

react里，只需要更新组件的state，然后根据新的state重新渲染用户界面(不要操作DOM);

* getInitialState方法用于定义初始状态，也就是一个对象，这个对象可以通过this.state属性读取。

* 当用户点击组件，导致组件变化，this.setState方法就会修改属性值，每次修改后，会自动调用this.render方法，再次渲染组件。

[6] 

* state可以与用户交互来改变值；

* props值是不变的。getDefaultProps设置props默认值；

* 组合使用state、props--可以在父组件中设置state，并通过子组件使用props将其传递到子组件上。
 
