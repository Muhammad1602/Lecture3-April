# Lecture3-April
# Homework
## _Methods_

[![N|Solid](https://dmitripavlutin.com/javascript-method/cover.png)

A method is a block of code which only runs when it is called.
You can pass data, known as parameters, into a method.
Methods are used to perform certain actions, and they are
also known as functions.

## _JS strings_

- Double Quotes

- Single Quotes

- ✨Backticks

## JAVA SCRIPT STRING METHODS
![The San Juan Mountains are beautiful!](https://res.cloudinary.com/practicaldev/image/fetch/s--LiXsFcOv--/c_imagga_scale,f_auto,fl_progressive,h_900,q_auto,w_1600/https://dev-to-uploads.s3.amazonaws.com/uploads/articles/bhe8j6h5ex4eaamejawv.png)
- `charAt()`
> The charAt() method returns the character at a specified index (position) in a string.
```
var anyString = 'Дивный новый мир';

console.log("Символ по индексу 0   равен '" + anyString.charAt(0)   + "'");
console.log("Символ по индексу 1   равен '" + anyString.charAt(1)   + "'");
console.log("Символ по индексу 2   равен '" + anyString.charAt(2)   + "'");
console.log("Символ по индексу 3   равен '" + anyString.charAt(3)   + "'");
console.log("Символ по индексу 4   равен '" + anyString.charAt(4)   + "'");
console.log("Символ по индексу 5   равен '" + anyString.charAt(5)   + "'");
console.log("Символ по индексу 999 равен '" + anyString.charAt(999) + "'");
```

-  `concat()`
> The concat() method joins two or more strings.
```
var hello = 'Привет, ';
console.log(hello.concat('Кевин', ', удачного дня.'));

/* Привет, Кевин, удачного дня. */
```

- replace()`
> The replace() method searches a string for a value or a regular expression.
```
var re = /яблоки/gi;
var str = 'Яблоки круглые и яблоки сочные.';
var newstr = str.replace(re, 'апельсины');
console.log(newstr); // апельсины круглые и апельсины сочные.
```


- `replaceAll()`
> The replaceAll() method returns a new string with all matches of a pattern replaced by
a replacement.
```
const p = 'The quick brown fox jumps over the lazy dog. If the dog reacted, was it really lazy?';

console.log(p.replaceAll('dog', 'monkey'));
// Expected output: "The quick brown fox jumps over the lazy monkey. If the monkey reacted, was it really lazy?"


// Global flag required when calling replaceAll with regex
const regex = /Dog/ig;
console.log(p.replaceAll(regex, 'ferret'));
// Expected output: "The quick brown fox jumps over the lazy ferret. If the ferret reacted, was it really lazy?"

```

- `split()`
>The split() method splits a string into an array of substrings. The split() method returns the new
array. The split() method does not change the original string. If (" ") is used as separator, the string
is split between words.
```
var myString = 'Привет, мир. Как дела?';
var splits = myString.split(' ', 3);

console.log(splits);
//Привет,,мир.,Как
```

- `substring(start,end)`
>The substring() method extracts characters, between two indices (positions), from a string, and
returns the substring.
The substring() method extracts characters from start to end (exclusive).
The substring() method does not change the original string.
If start is greater than end, arguments are swapped: (4, 1) = (1, 4).
Start or end values less than 0, are treated as 0.

```
var anyString = 'Mozilla';

// Отобразит 'Moz'
console.log(anyString.substring(0, 3));
console.log(anyString.substring(3, 0));
```

- `slice(start, end)`
>The slice() method returns a shallow copy of a portion of an array into a new array object
selected from start to end ( end not included) where start and end represent the index of items
in that array.
```
const str = 'The quick brown fox jumps over the lazy dog.';

console.log(str.slice(31));
// Expected output: "the lazy dog."

console.log(str.slice(4, 19));
// Expected output: "quick brown fox"
```

- `toLowerCase()`
>The toLowerCase() method converts a string to lowercase letters.
```
console.log('АЛФАВИТ'.toLowerCase()); // 'алфавит'
```

- `toUpperCase()`
>The toUpperCase() method converts a string to uppercase letters, using current locale.
```
console.log('алфавит'.toUpperCase()); // 'АЛФАВИТ'
```

- `trim()`
>Method trim() removes whitespace from both sides of a string
```
var orig = '   foo  ';
console.log(orig.trim()); // 'foo'
```

- `includes()`
>The includes() method returns true if a string contains a specified string.
Otherwise it returns false.
```
'Синий кит'.includes('синий'); // вернёт false
```


- `toString()`
>The toString() method returns a string representing the object.
By default toString() takes no parameters.
```
var x = new String('Привет, мир');

console.log(x.toString()); // Отобразит 'Привет, мир'
```

-  `indexOf()`
>The indexOf() method returns the position of the first occurrence of a value in a string.
The indexOf() method returns -1 if the value is not found.
```
'Синий кит'.indexOf('Синий');   // вернёт  0
'Синий кит'.indexOf('Голубой');  // вернёт -1
'Синий кит'.indexOf('кит', 0);    // вернёт  6
```

- `repeat()`
>The repeat() method creates a new string by repeating the given string a specified number of
times and returns it.
```
'абв'.repeat(1);    // 'абв'
'абв'.repeat(2);    // 'абвабв'
```



## JAVA SCRIPT NUMBER METHODS
![The San Juan Mountains are beautiful!](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcR_2lmuLBkmG3pF3WK5L4zHgv0sEBsg9r4lax7nUXbSvmkrZWf2FUPeznwGtWVQqR-SsKk&usqp=CAU)

- Math.floor()
> The Math.floor() function rounds down a number to the next smallest integer.
```
console.log(Math.floor(5.95));
// Expected output: 5

console.log(Math.floor(5.05));
// Expected output: 5
```

-  Math.round()
> The Math.round() function returns the number rounded to the nearest integer.
```
console.log(Math.round(0.9));
// Expected output: 1

console.log(Math.round(5.95), Math.round(5.5), Math.round(5.05));
// Expected output: 6 6 5
```

- Math.ceil()
> The ceil() method rounds a decimal number up to the next largest integer and returns it.
```
console.log(Math.ceil(.95));
// Expected output: 1

console.log(Math.ceil(4));
// Expected output: 4
```

- Math.max() 
> The max() method finds the maximum value among the specified values and returns it.
```
console.log(Math.max(1, 3, 2));
// Expected output: 3

console.log(Math.max(-1, -3, -2));
// Expected output: -1
```

- Math.min()
>The min() method finds the minimum value among the specified values and returns it.
```
console.log(Math.min(2, 3, 1));
// Expected output: 1

console.log(Math.min(-2, -3, -1));
// Expected output: -3

```

- Math.pow()
>The pow() method computes the power of a number by raising the second argument
to the power of the first argument.
```
console.log(Math.pow(7, 3));
// Expected output: 343

console.log(Math.pow(4, 0.5));
// Expected output: 2

```

-  Math.sqrt()
>The sqrt() method computes the square root of a specified number and returns it
```
function calcHypotenuse(a, b) {
  return (Math.sqrt((a * a) + (b * b)));
}

console.log(calcHypotenuse(3, 4));
// Expected output: 5

```
- Math.abs()
>The abs() method finds the absolute value of the specified number (without any sign) and returns it.
```
function difference(a, b) {
  return Math.abs(a - b);
}

console.log(difference(3, 5));
// Expected output: 2
```

- Math.random()
>The Math.random() function returns a floating-point, pseudo-random number between 0 (inclusive)
and 1 (exclusive).
```
console.log(Math.random());
// Expected output: a number from 0 to <1
```
-  isNaN()
>The isNaN() function checks if a value is NaN (Not-a-Number) or not.
```
var x = NaN

x != x // true
x !== x // true
```