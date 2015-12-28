# React expandable listview
[![Gitter](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/cht8687/help)

<big><h1 align="center">React expandable listview</h1></big>

<p align="center">
  <a href="https://www.npmjs.com/package/react-expandable-listview">
    <img src="https://img.shields.io/npm/v/react-expandable-listview.svg?style=flat-square"
         alt="NPM Version">
  </a>

 <a href="https://coveralls.io/github/cht8687/react-expandable-listview?branch=master">
    <img src="https://coveralls.io/repos/cht8687/react-expandable-listview/badge.svg?branch=master&service=github" alt="Coverage Status" />
 </a>

  <a href="https://travis-ci.org/cht8687/react-expandable-listview">
    <img src="https://img.shields.io/travis/cht8687/react-expandable-listview.svg?style=flat-square"
         alt="Build Status">
  </a>

  <a href="https://npmjs.org/package/react-expandable-listview">
    <img src="http://img.shields.io/npm/dm/react-expandable-listview.svg?style=flat-square"
         alt="Downloads">
  </a>

  <a href="https://david-dm.org/cht8687/react-expandable-listview.svg">
    <img src="https://david-dm.org/cht8687/react-expandable-listview.svg?style=flat-square"
         alt="Dependency Status">
  </a>

  <a href="https://github.com/cht8687/react-expandable-listview/blob/master/LICENSE">
    <img src="https://img.shields.io/npm/l/react-expandable-listview.svg?style=flat-square"
         alt="License">
  </a>
</p>

<p align="center"><big>

</big></p>

![React expandable listview](src/example/react-expandable-listview.gif)

## Installation

### npm

```
$ npm install --save react-expandable-listview
```


## Demo

[http://cht8687.github.io/react-expandable-listview/example/](http://cht8687.github.io/react-expandable-listview/example/)

## Example Code

[https://github.com/cht8687/react-expandable-listview/tree/master/src/example](https://github.com/cht8687/react-expandable-listview/tree/master/src/example)

## Usage

```js
<ReactExpandableListView 
        data={data} 
        headerAttName="headerName"
        itemsAttName="items" 
        styles={styles}
      />
```

## Options

#### `data`: PropTypes.array.isRequired

```js
const DATALIST = [
{
 	headerName : "ListA",
 	isOpened: true,
    items : [{
      title : "items1"
    }, {
      title : "items2"
    }]
},
{
 	headerName : "ListB",
 	isOpened: true,
    items : [{
      title : "items1"
    }, {
      title : "items2"
    }]
}
];
```

#### `headerAttName`: PropTypes.string.isRequired

variable name of header in your `data` object.
In above example, it's `headerName`.

#### `itemsAttName`: PropTypes.string.isRequired

variable name which hold items data in your `data` object.
In above example, it's `items`.

#### `styles`: PropTypes.object.isRequired

```js
let styles = {
   outerDiv: {
    height: '400px',
    overflowY: 'auto',
    outline: '1px dashed blue',
    width: '400px',
  },

  ul: {
    margin: '0px',
    listStyleType: 'none',
    padding: '0'
  },

  fixedPosition: {
    position : 'fixed',
    width : '383px',
    top: '0px'
  },

  listHeader: {
    width: '383px',
    height: '20px',
    background: 'orange',
    color: 'white'
  },

  listItems: {
    color: 'blue'
  },
};
```

`outerDiv`, `ul`, `fixedPosition`, `listHeader`, `listItems` are required, you can modify the CSS to meet your needs.


## Development

```
$ git clone git@github.com:cht8687/react-expandable-listview.git
$ cd react-expandable-listview
$ npm install
$ webpack-dev-server
```

*tip:* If you have already had webpack-dev-server running, you might have EADDRINUSE error, please ensure the port is not in use.

Then

```
open http://localhost:8080/webpack-dev-server/
```

## License

MIT
