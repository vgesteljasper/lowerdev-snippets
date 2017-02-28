# lowerdev-snippets package

This Atom package adds basic reactjs and es6 snippets.

##notice

_Note this package is made for personal use and for sharing with classmates.
This makes that these snippets may or may not work all that well with existing
ones you have installed as the shortcuts are pretty short and may be common with
other snippets._

## general ES6 snippets

**init function**
`init`

    /**
     * @author ${1:name} <${2:example@email.com}>
     */

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


**es6 import**
`im`

    import ${1:something} from '${2:somewhere}';


## react snippets


**new container component** (stateful)
`cc`

    import React, {Component} from 'react';

    class ${1:ComponentName} extends Component {

      state = {}

      render() {
        return(
          <span>${1:ComponentName}</span>
        );
      }
    }

    export default ${1:ComponentName};


**new presentation component** (stateless)
`pc`

    import React, {PropTypes} from 'react';

    const ${1:ComponentName} = (props) {

      // const {title} = props;

      return(
        <span>${1:ComponentName}</span>
      );

    }

    ${1:ComponentName}.propTypes = {
      // title: PropTypes.string.isRequired
    }

    export default ${1:ComponentName};


**import react-router**
`ir`

    import {${1:routerType} as ${2:newName}} from 'react-router';


**setState**
`ss`

    this.setState({
      ${1:key: value}
    });


**componentWillMount**
`cwm`

    componentWillMount() {
      ${1:code}
    }


**componentDidMount**
`cdm`

    componentDidMount() {
      ${1:code}
    }


**componentWillReceiveProps**
`cwr`

    componentWillReceiveProps() {
      ${1:code}
    }


**shouldComponentUpdate**
`scu`

    shouldComponentUpdate() {
      ${1:code}
    }


**componentWillUpdate**
`cwup`

    componentWillUpdate() {
      ${1:code}
    }


**componentWillUnmount**
`cwun`

    componentWillUnmount() {
      ${1:code}
    }


**component reference prop**
`ref`

    ref={el => this.${1:referenceName} = el}
