# react-native-editable-list

> An editable React list component

[![NPM](https://img.shields.io/npm/v/react-native-editable-list.svg)](https://www.npmjs.com/package/react-native-editable-list) [![JavaScript Style Guide](https://img.shields.io/badge/code_style-standard-brightgreen.svg)](https://standardjs.com)

## Install

```bash
npm install --save react-native-editable-list
```

## Usage

```jsx
import React, { Component } from 'react'

import EditableList from 'react-native-editable-list'

class Example extends Component {
  constructor() {
    super();
    this.state = {
      obs: []
    }
  }
  onChange(list) {
    this.setState({obs: list})
  }
  render() {
    return <EditableList list={this.state.obs} onListChange={this.onChange.bind(this)}/>
  }
}
```

## License

MIT © [phos-dev](https://github.com/phos-dev)
