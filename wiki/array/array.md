# Arrays

use to hold a collection of objects

- Declaration:

let values = Array.of(1, 2, 3);
const values = ['a', 'b', 'c'];

- Access elements:

let value1 = values[0];

- Manipulating arrays:

push - adds to the end of array and returns the array
values.push('d','e'); - returns the array with added element // a,b,c,d

pop - removes the last value of the array and returns it
values.pop(); // d

shift - moves the entire aray to the left and removes the first element and returns the first element
unshift - adds elements to the beginning, opposite to shift

values.shift()
values.unshift('a')

slice(startElement, endElement) - takes 2 indices as parameters. cuts off elements before startElement and after endElement.
values.slice(1,2) // [b,c]

splice(1, 1, elementToBeInserted) - splice is opposite to slice but can be used to insert if there by entering a 3rd parameter.

---

- Array Iteration

values.indexOf('c') // returns the index of an element

- filter()
  const set values.filter(function(item) {
  return item > 'b';
  })

- find() - find the item/s
  const found = values.find(function(item) {
  return item.length > 1;
  })

- forEach(): iterate
  values.forEach(function(item) {
  console.log(item)
  })
