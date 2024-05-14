## Data Filtering

- 1. Given an array of numbers, filter out only the even numbers.

```js
let numbers = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10];
const even = [];
const odd = [];

for (let i = 0; i < numbers.length; i++) {
  const item = numbers[i];
  if (item % 2 === 0) {
    even.push(item);
  } else {
    odd.push(item);
  }
}
console.log(even, odd);
```

- Finding out all the items that statisfies the given conditions
- 2. Find out all the books which have more than 250 pages.(Data Filtering)

```js
const books = [
  {
    id: 1,
    title: "Book 1",
    author: "Author 1",
    pages: 200,
  },
  {
    id: 2,
    title: "Book 2",
    author: "Author 2",
    pages: 300,
  },
  {
    id: 3,
    title: "Book 3",
    author: "Author 3",
    pages: 250,
  },
];

for (let i = 0; i < books.length; i++) {
  const item = books[i];
  if (item.pages > 250) {
    result = item.id;
  }
}
console.log(result);
```

- 3.Given an array of strings, filter out only the strings containing the letter 'a'.

```js
const fruits = ["apple", "banana", "orange", "strawberry"];

const nameA = [];
for (let i = 0; i < fruits.length; i++) {
  const item = fruits[i];
  if (item.indexOf("a") >= 0) {
    nameA.push(item);
  }
  console.log(nameA);
}
```

- 4. Separate out all male and female students in two group

```js
const students = [
  {
    firstName: "John",
    lastName: "Smith",
    age: 22,
    gender: "male",
  },
  {
    firstName: "Michael",
    lastName: "Johnson",
    age: 20,
    gender: "male",
  },
  {
    firstName: "William",
    lastName: "Williams",
    age: 23,
    gender: "male",
  },
  {
    firstName: "David",
    lastName: "Jones",
    age: 19,
    gender: "male",
  },
  {
    firstName: "James",
    lastName: "Brown",
    age: 21,
    gender: "male",
  },
  {
    firstName: "Mary",
    lastName: "Smith",
    age: 20,
    gender: "female",
  },
  {
    firstName: "Jennifer",
    lastName: "Johnson",
    age: 18,
    gender: "female",
  },
  {
    firstName: "Linda",
    lastName: "Williams",
    age: 24,
    gender: "female",
  },
  {
    firstName: "Patricia",
    lastName: "Jones",
    age: 22,
    gender: "female",
  },
  {
    firstName: "Susan",
    lastName: "Brown",
    age: 19,
    gender: "female",
  },
];

const boys = [];
const girls = [];

for (let i = 0; i < students.length; i++) {
  const item = students[i];
  if (item.gender === "male") {
    boys.push(item);
  }
  if (item.gender === "female") {
    girls.push(item);
  }
}
console.log({ boys, girls });
```

- 5. Seperate strings, number and object data types from the given array in 3 different groups.

```js
const unprocessedData = [
  "Firoj",
  301010,
  "who",
  "false",
  true,
  null,
  undefined,
  { name: "shoaib", profession: "student" },
  4444,
  "",
  {},
  false,
];

let numbers = [];
let objects = [];
let strings = [];

for (let i = 0; i < unprocessedData.length; i++) {
  const item = unprocessedData[i];
  if (typeof item === "string") {
    strings.push(item);
  } else if (typeof item === "number") {
    numbers.push(item);
  } else if (typeof item === "object" && item !== null) {
    objects.push(item);
  }
}
console.log("string", strings);
console.log("number", numbers);
console.log("object", objects);
```
