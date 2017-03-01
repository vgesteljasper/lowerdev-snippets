# lowerdev-snippets Package

This Atom package adds basic reactjs and es6 snippets.

## notice

_Note this package is made for personal use and for sharing with classmates.
This makes that these snippets may or may not work all that well with existing
ones you have installed as the shortcuts are pretty short and may be common with
other snippets._

## General JavaSript Snippets

**Init Function**
`init`

    const init = () => {
      ${3:console.log(`script initialised`);}
    };

    init();

**getElementsById**
`gbi`

    const ${1:elementName} = document.getElementById(`${2:node}`);

**getElementsByClassName**
`gbc`

    const ${1:elementName} = document.getElementsByClassName(`${2:node}`);

**querySelector**
`sq`

    const ${1:elementName} = document.querySelector(`${2:node}`);

**querySelectorAll**
`qsa`

    const ${1:elementName} = document.querySelectorAll(`${2:node}`);

**Import From**
`imp`

    import ${1:something} from '${2:somewhere}';

**Import From As**
`impas`

    import {${1:something} as ${2:somethingElse}} from '${3:package}';

**Import All From**
`impall`

    import * from '${1:package}';

**Arrow Function**
`func`

    const ${1:methodName} = (${2:params}) => {
      ${3://code}
    };

**Class Constructor**
`cns`

    constructor(${1:args}) {
      ${2://code}
    }

**Export Default Function**
`expdf`

    export default (${1:args}) => {
      ${2://code}
    };

**Export Default Class**
`expdc`

    export default class ${1:className} {
      ${2://code}
    }

## React Snippets

**Container Component** (stateful)
`cc`

    import React, {Component} from 'react';

    class ${1:ComponentName} extends Component {

      state = {}

      render() {
        return (
          <span>${1:ComponentName}</span>
        );
      }
    }

    export default ${1:ComponentName};

**Presentation Component** (stateless)
`pc`

    import React, {PropTypes} from 'react';

    const ${1:ComponentName} = ({someProperty}) => {

      return (
        <span>${1:ComponentName} - {someProperty}</span>
      );

    };

    ${1:ComponentName}.propTypes = {
      someProperty: PropTypes.string.isRequired
    };

    export default ${1:ComponentName};

**setState**
`ss`

    this.setState(${1:newState});

**Component Reference Prop**
`ref`

    ref={el => this.${1:referenceName} = el}

**Comp. Will Mount**
`cwm`

    componentWillMount() {
      ${1:code}
    }

**Comp. Did Mount**
`cdm`

    componentDidMount() {
      ${1:code}
    }

**Comp. Will Receive Props**
`cwr`

    componentWillReceiveProps() {
      ${1:code}
    }

**Should Comp. Update**
`scup`

    shouldComponentUpdate() {
      ${1:code}
    }

**Comp. Will Update**
`cwup`

    componentWillUpdate() {
      ${1:code}
    }

**Comp. Did Update**
`cdup`

    componentDidUpdate() {
      ${1:code}
    }

**Comp. Will Unmount**
`cwun`

    componentWillUnmount() {
      ${1:code}
    }

## React Router Snippets

**Import React Router**
`imprr`

    import {
      BrowserRouter as Router,
      Route
    } from 'react-router-dom';

**Route Render**
`routeren`

    <Route path={`/${1:users/:id}`} render={({match}) => {
      return ${2:<SomeComponent />};
    }} />

**Route Component**
`routecom`

    <Route path={`/${1:users/:id}`} component={${2:someComponent}} />

**Router Link**
`link`

    <Link to={`/${1:somePath}`} />

**Router Nav Link**
`navlink`

    <NavLink
      activeClassName={`active`}
      to={`/${1:somePath}`}
    />

**Router Redirect**
`red`

    <Redirect to={`/${1:somePath}`} />
