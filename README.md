# react-native-tabbed-control

[![Platform](https://img.shields.io/badge/platform-react--native-lightgrey.svg)](http://facebook.github.io/react-native/)
[![npm version](http://img.shields.io/npm/v/react-native-segment-control.svg)](https://www.npmjs.com/package/react-native-tabbed-control)

## Demo

<img src="https://github.com/manenga/react-native-tabbed-control/blob/f9102583d0fc93b9fae6c2e4ef2dda6954b84f8e/tab-demo.gif?raw=true" width="30%" /> 

## Installation

```
$ npm install react-native-tabbed-control --save
```

## Example Without Attached Views

```JSX
...
import TabbedControl from 'react-native-tabbed-control';

const tabs = [{title: 'South Africa'} , {title: 'Zambia'}];

updateIndex(selectedIndex) {
  this.setState({selectedIndex: selectedIndex});
}
  
render() {
  return (
    <View>
      <TabbedControl tabs={tabs} color={'#024b30'} onIndexChange={this.updateIndex}/>
    </View>
  );
};
```

## Example With Static Views Attached

```JSX
...
import TabbedControl from 'react-native-tabbed-control';

const One = () => { return <Text>This is first view</Text>; };
const Two = () => { return <Text>This is second view</Text>; };

const tabs = [
  {
    title: 'One',
    view: One
  },
  {
    title: 'Two',
    view: Two
  }
];

render() {
  return (
    <View style={styles.container}>
      <TabbedControl tabs={tabs} color={'#024b30'} />
    </View>
  );
};
```

## Tab Properties
| Property | Type | isRequired |
| --- | --- | --- |
| title | String | YES |
| view | View | NO |

## TabbedControl Properties
| Property | Type | isRequired |
| --- | --- | --- |
| tabs | Tab Array | NO |
| color | Color | NO |
| onIndexChange | Function | NO |

## How can I support the developers?
- Star our GitHub repo ⭐
- Create pull requests, submit bugs, suggest new features or documentation updates 🔧
- Follow me on [Twitter](https://twitter.com/mmungandi)
- Follow me on [Instagram](https://instagram.com/mungandi)
- Buy me coffee or [Donate](https://paypal.me/Mungandi)

## More from the developers
- [Rona Mobile App](https://github.com/manenga/Rona/) - Covid19 Global Pandemic Statistics Tracker

## License
[MIT](https://github.com/manenga/react-native-tabbed-control/blob/master/LICENSE) license.

## From Developers
Made with ♥ by [Manenga](https://linkedin.com/in/mungandi/)

## TO-DO's:
- [X] onIndexChange when a tab is tapped
- [ ] Add icons as tab titles
- [ ] Update selected index on scroll
