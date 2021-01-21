//1. Write another function that returns true if the string passed as an argument is a palindrome, or false otherwise. 
//Your function should be case-insensitive, and should ignore all non-alphanumeric characters.
function palindrome(str) {
  return str.toLowerCase() === str.toLowerCase().split('').reverse().join('').replaceAll('/[^a-z\d ]/i', '', str);
}
console.log(palindrome('EebbEe')); 

//2. Write a function that takes an array of numbers, and returns an array with the same number of elements, 
//with each element's value being the running total from the original array.
const cumulativeSum = (sum => value => sum += value)(0);

console.log([5, 10, 3, 2].map(cumulativeSum));

//3. Given a string of words separated by spaces, write a function that swaps the first and last letters of every word. 
//You may assume that every word contains at least one letter, and that the string will always contain at least one word. 
//You may also assume that each string contains nothing but words and spaces, and that there are no leading, trailing, or repeated spaces.

function first_last(str1) 
  {
  if (str1.length <= 1)
  {
    return str1;
  }
  mid_char = str1.substring(1, str1.length - 1);
  return (str1.charAt(str1.length - 1)) + mid_char + str1.charAt(0);
}
console.log(first_last('Hello there'));

//4. Write a function that takes a string consisting of one or more space separated words, and returns an object that shows the number of words of different sizes.
//Words consist of any sequence of non-space characters.

const strFrequency = function (stringArr) {
  return stringArr.reduce((count,num) => {
    count [num] = (count[num] || 0) + 1;
    return count;
  },
  {})
}

let names = ["Hello my name is Jaylene"];

console.log(strFrequency(names));

//5. Write a function that takes two arrays as arguments, and returns an array containing the union of the values from the two. 
//There should be no duplication of values in the returned array, even if there are duplicates in the original arrays. 
//You may assume that both arguments will always be arrays.

function union_arrays (x, y) {
  var obj = {};
  for (var i = x.length-1; i >= 0; -- i)
     obj[x[i]] = x[i];
  for (var i = y.length-1; i >= 0; -- i)
     obj[y[i]] = y[i];
  var res = []
  for (var k in obj) {
    if (obj.hasOwnProperty(k))  // <-- optional
      res.push(obj[k]);
  }
  return res;
}

console.log(union_arrays([1, 3, 5], [3, 6, 9]));

//6. Find the first recurring character in a string. If a string does not have a recurring character, return an empty string.

function getFirstRecurringChar(str) {
  let i = 0;
  const len = str.length;
  const letters = {};
  while(i < len && !letters[str[i]]) { letters[str[i++]] = true; }
  return i < len ? str[i] : null;
};

console.log(getFirstRecurringChar("acbbac"));

//7. Write a multiplicative average function that takes an array of integers as input, multiplies all of the integers together, 
//divides the result by the number of entries in the array, and returns the result as a string with the value rounded to three decimal places.

