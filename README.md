
### Remove falsy values from an array
```javascript
const arr = [0, 'yellow', '', NaN, 1, true, undefined, 'orange', false]
	
console.log(arr.filter(Boolean)); // Output -> ['yellow', 1, true, 'orange']
console.log(arr.filter(a => !!a)); // Output -> ['yellow', 1, true, 'orange']
```

### Get a random element from array
```javascript
const colors = ['yellow', 'orange', 'blue', 'purple', 'green'];
const randomColor = colors[Math.floor(Math.random() * colors.length)];
	
console.log(randomColor); // Output -> blue
```

### Shuffle an array
```javascript
const list = [1, 2, 3, 4, 5, 6, 7, 8, 9];
const shuffled = list.sort(() => Math.random() - 0.5)
    	
console.log(shuffled); // Output -> [6, 2, 1, 4, 5, 3, 9, 8, 7]
```

### Find the intersection of two arrays
```javascript
const numOne = [0, 2, 4, 6, 8, 8];
const numTwo = [1, 2, 3, 4, 5, 6];
const duplicateValues = [...new Set(numOne)].filter(item => numTwo.includes(item));
        	
console.log(duplicateValues); // Output -> [2, 4, 6]
```

### Find the Day of year
```javascript
const dayOfYear = (date) => {
	Math.floor((date - new Date(date.getFullYear(), 0, 0)) / 1000 / 60 / 60 / 24);	
}
```
