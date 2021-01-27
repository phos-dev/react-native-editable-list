# react-native-editable-list

> An editable list component for React Native.

[![NPM](https://img.shields.io/npm/v/react-native-editable-list.svg)](https://www.npmjs.com/package/react-native-editable-list) [![JavaScript Style Guide](https://img.shields.io/badge/code_style-standard-brightgreen.svg)](https://standardjs.com)

## Install

```bash
npm install --save react-native-editable-list
```

## Usage

```jsx
import React, { useState } from 'react';
import { StyleSheet, Text, View, FlatList, TextInput, TouchableOpacity } from 'react-native';
import EditableList from 'react-native-editable-list'

export default function App() {
  const [list, setList] = useState([]);
  return (
    <View style={styles.container}>
	  <EditableList placeholder='Type something' onListChange={setList.bind(this)} list={list}/>
	  <Text style={styles.data}> Data </Text>
	  <Text> {list.length ? JSON.stringify(list) : 'Please, type something.'} </Text>
    </View>
  );
}

const styles = StyleSheet.create({
  container: {
    flex: 1,
    backgroundColor: 'yellow',
    alignItems: 'center',
    justifyContent: 'center',
    padding: 40
  },
  data: {
      fontSize: 20
  }
});
```

## License

MIT © [phos-dev](https://github.com/phos-dev)
