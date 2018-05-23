# Learn-React

## Components

Everything in React is a component, and these usually take the form of JavaScript classes.

```html

class Hello extends React.Component {
    render() {
        return <h1>Hello world!</h1>;
    }
}

```

To get our application to render on the screen we also have to use 

```html

ReactDOM.render(
    <Hello />, 
    document.getElementById("root")
);

```

## Handling data

Two types of data in React: props and state

<pre>

*  State - Private and can be changed from within the component itself.
*  Props - External, and not controlled by the component itself. Passed down from components higher up the hierarchy, who also control the data.

</pre>

## Props

How to pass prop to a component

```html

ReactDOM.render(
    <Hello message="my friend" />, 
    document.getElementById("root")
);

```
How to access this prop inside the component  

```html

class Hello extends React.Component {
    render() {
        return <h1>Hello {this.props.message}!</h1>;
    }
}

```


