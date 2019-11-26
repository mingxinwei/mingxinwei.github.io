# React Learning

## Introducing JSX

1. JSX 是 js 的拓展。JSX 在 react 里写出来的是一个`react element`。经过 babel 编译之后就变成`React.createElement()`，这个函数的输出是产生一个特定结构的 js object
2. JSX 可以在`{}`之间放任何 js 表达式
3. JSX 的属性使用 camelCase 命名，属性里也可以用`{}`放 js 表达式

## Rendering Elements

1. Element 是 react 中的 smallest build block
2. Element 构成 Component
3. Element 是不可变的

## Components and Props

1. Component 让你可以把 UI 分为独立的、可以复用的、具有封装性的 code pieces

2. Component 像 js 里的函数，接受参数`props`，输出`react element`

3. Component 有 2 种写法：function component 和 class component
   1. Function component 接受一个 props 参数，输出`react element`
   2. Class component 需要实现一个 render 方法，输入为`this.props`，输出`react element`
   3. Class component 的一个优点是可以存储状态
   
4. Component 总是首字母大写的（为了和 html 的标签区分开，小写开头的被认为是 html 的标签）

5. Component 可以像 html 标签一样嵌套着别的 component，所以大到整个 React App，小到一个 button，都可以表达为 component

   ```jsx
   function Welcome(props) {
     return <h1>Hello, {props.name}</h1>;
   }

   function App() {
     return (
       <div>
         <Welcome name="Sara" />
         <Welcome name="Cahal" />
         <Welcome name="Edite" />
       </div>
     );
   }

   ReactDOM.render(<App />, document.getElementById("root"));
   ```

6. Props 是只读的，不允许改变。

111
