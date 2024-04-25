# view-state-util

## Usage Example
index.js
```js
let viewStatesMap = [
  {
    group: 'screens',
    states: [ 'homepage' ],
    inverseStates: [ 'homepage' ],
  },
];

viewStateUtil.Init(viewStatesMap); 
```
style.css
```
/* vendors/view-state-util */
[data-view-name] { display: none; }
```
index.html
```html
<div data-view-group="screens" data-view-states="">
  <div data-view-group="screens" data-view-name="homepage">
    Main screen
  </div>
  <div data-view-group="screens" data-view-name-not="homepage">
    Settings
  </div>
</div>
```