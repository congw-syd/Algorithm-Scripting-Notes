# Find the Longest Word in a String
## Basic Code Solution
```javascript
function findLongestWordLength(str) {
  var words = str.split(' ');
  var maxLength = 0;
  
  for (var i = 0; i < words.length; i++) {
    if (words[i].length > maxLength) {
      maxLength = words[i].length;
    }
  }
  return maxLength;
}
```
## Intermediate Code Solution
```javascript
function findLongestWordLength(s) {
  return s.split(' ')
          .reduce(function(x, y) {
            return Math.max(x, y.length)
           }, 0);
}
```
### array.reduce()
```javascript
arr.reduce(callback[, initialValue])
```
If an initialValue is provided, the reduce method calls the callback function one time for **each** element present in the array, in ascending index order. If an initialValue is not provided, the reduce method calls the callback function on each element, starting with the **second** element.
## Advanced Code Solution
