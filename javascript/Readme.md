## Destructuring
```bash
const obj = {
    player: 'John',
    rank: 50,
    clan: star
}

const player = obj.player;
const rank = obj.rank;
let clan = obj.clan;

// this is equal to above

const {player, rank} = obj;
let {clan} = obj;
```

## Object properties
```bash
const name = 'Jack';

const obj = {
    [name]: 'Hello',
    [1+2]: 'Hi'
}
```

## Template strings
```bash
const name = 'Jack';

const greeting = "Hello from " + name;
const bestGreeting = `Hello from ${name}`;
```

## Arrow functions
```bash
function add1(a, b){
    return a+b;
}

const add1 = (a, b) => {
    return a+b;
}

const add2 = (a, b) => a+b;
```

## Arrays
```bash
const array = [1, 2, 3, 4, 5];
array.forEach(num => console.log(num)});

const mapArray = array.map(num => num*2);
console.log(mapArray); // [2, 4, 6, 8, 10]

const filterArray = array.filter(num => num>2);
console.log(filterArray); // [3, 4, 5]

const reduceArray = array.reduce((sum, num) => {
    return sum+num;
}, 10); // initial value of sum is 10
console.log(reduceArray); // 25

```