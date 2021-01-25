# react-native-editable-list

> An editable React list component 
[![NPM](https://img.shields.io/npm/v/react-native-editable-list.svg)](https://www.npmjs.com/package/react-native-editable-list) [![JavaScript Style Guide](https://img.shields.io/badge/code_style-standard-brightgreen.svg)](https://standardjs.com)

## Install

```bash
npm install --save react-native-editable-list
```

## Usage

```jsx
import React, { useState } from 'react';
import { StyleSheet, Text, View, FlatList } from 'react-native';
import EditableList from 'react-native-editable-list';

export default function App() {
  const [list, setList] = useState([]);
  return (
    <View style={styles.container}>
	  <EditableList placeholder='Please, type something' onListChange={setList.bind(this)} list={list}/>
	  <Text> Data </Text>
	  <Text> {list.toString()} </Text>
    </View>
  );
}

const styles = StyleSheet.create({
  container: {
    flex: 1,
    backgroundColor: 'yellow',
    alignItems: 'center',
    justifyContent: 'center',
    padding: 20
  },
});
```

## License

MIT © [phos-dev](https://github.com/phos-dev)
