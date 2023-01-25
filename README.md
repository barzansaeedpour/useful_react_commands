# useful_react_commands

useful extension for vscode:

> Debugger for chrome (deprecated but still working)
to debug react projects


> Simple React Snippets
to import react,component: imrc
to import react: imr
to create a class(Component): cc
to create a Stateless Function Component: sfc

> Auto import - ES6, Ts, JSK, TSX
> Auto rename tag
> IntelliSense for CSS class names in Html
> Search node modules


download and install node js then:

```
node -v
```

install create app globaly:
```
npm i -g create-react-app
```

install create app globaly specific version:
```
npm i -g create-react-app@3.3.0
```

------------------------------------------------------------------------

create and run a project:
```
create-react-app appName
```
```
cd firstproject
```
```
npm start
```


or:
go to the folder:cmd
```
create-react-app .
```
```
code .
```
```
npm start
```

to install packages for existing project:
go to the directory of the project:
(this will install all the dependencies from package.json
and create node_modules folder)
```
npm i
```

-----------------------------------------------------------------------
How to use a component:

<Counter counter={5}/>

*** class component: *****

import { Component } from "react";

class Counter extends Component {
    render() {
        console.log(this.props);
    return (
      <div>
        counter: {this.props.counter}
      </div>
    );
  }
}

*** function component: *****

const Counter = (props)=>{
    console.log(this.props);
    return <div>
        counter: {props.counter}
    </div>
}

-----------------------------------------------------------------------

two basic rules:
1) only changing the state and props can cause react re-rendering
2) never change the probs and state directly

components must be pure functions (do not change the inputs)










