# Reverse a String
```javascript
  function reverseString(str) {
    return str.split('').reverse().join('');
  }
  
  reverseString("hello");
```
## String.split()
```javascript
  var str = 'The quick brown fox jumps over the lazy dog.';

  var words = str.split(' ');
  console.log(words);

  var chars = str.split('');
  console.log(chars);

  var strCopy = str.split();
  console.log(strCopy);
```
```
  > Array ["The", "quick", "brown", "fox", "jumps", "over", "the", "lazy", "dog."]
  > Array ["T", "h", "e", " ", "q", "u", "i", "c", "k", " ", "b", "r", "o", "w", "n", " ", "f", "o", "x", " ", "j", "u", "m", "p", "s", " ", "o", "v", "e", "r", " ", "t", "h", "e", " ", "l", "a", "z", "y", " ", "d", "o", "g", "."]
  > Array ["The quick brown fox jumps over the lazy dog."]
```
## String.reverse()
```javascript
  var array1 = ['one', 'two', 'three'];
  console.log('array1: ', array1);

  var reversed = array1.reverse(); 
  console.log('reversed: ', reversed);

  /* Careful: reverse is destructive. It also changes
  the original array */ 
  console.log('array1: ', array1);
 ```
 ```
  > "array1: " Array ["one", "two", "three"]
  > "reversed: " Array ["three", "two", "one"]
  > "array1: " Array ["three", "two", "one"]
 ```
## String.join()
```javascript
  var elements = ['Fire', 'Air', 'Water'];

  console.log(elements.join());
  console.log(elements.join(''));
  console.log(elements.join('-'));
```
```
  > "Fire,Air,Water"
  > "FireAirWater"
  > "Fire-Air-Water"
```
