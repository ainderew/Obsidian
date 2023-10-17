```javascript
function onClickOutside(ele, cb) {
  document.addEventListener('click', event => {
    if (!ele.contains(event.target)) cb();
  });
};

// Using
onClickOutside('#list', () => console.log('Hi!'));
// Will log 'Hi!' whenever the user clicks outside of #list
```
