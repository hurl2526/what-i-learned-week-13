#  **What I Learned Week 13**
## **Monday** 

Went over hw  

started arrow functions

Gets rid of word function and brackets and word return 

const add = (a,b) => a +  b

// arrow functions!

// (slightly) quicker syntax!

const sayHi = () => {
  console.log('hi');
}


// ACTUAL one-liners!



const add5 = (a) => a + 5;

const add = (a, b) => a + b;

const truncate = (str) => str.length > 10 ? str.slice(0, 7) + '...' : str;

// console.log(truncate('hello'))


const isOdd = (num) => num % 2 === 1;
// console.log(isOdd(6))
const numbers = [3, 5, 8, 16, 23];

// easy filters and maps!
const oddNumbers = numbers.filter((num) => num % 2 === 1);
const plus9000 = numbers.map((num) => num + 9000);

// console.log(oddNumbers)
// console.log(plus9000)






## **Tuesday**

Went over HW  

more on queue and stack:  
stacks and queues :
const Stack = function() {
  return{
    items: [],
    add: function(name){
      this.items.push(name);
    },
    remove: function(){
      return this.items.pop();
    },
    peek: function(){
      return this.items[this.items.length-1];
    },
  };
};

const Queue = function() {
  return{
    items: [],
    add: function (name){
      return this.items.push(name);
    },
    remove: function(){
      return this.items.shift();
    },
    peek: function(){
      return this.items[0];
    },
  };
};


// inheritance

class Animal {
  constructor(species) {
    this.species = species;
  }
}

class Dog extends Animal {
  constructor() {
    super('dog');
  }
}

const doggie = new Dog();

// console.log(`The value of doggie is: `)
// console.logyyu(doggie)

// composition
const makeCar = (name) => {
  return {
    name: name,
    maxSpeed: 120,
    wheelCount: 4,

    drive: function() {
      return `Vroom.`;
    }
  }
}

const robot = () => {
  return {
    sound: function() {
      return 'bleep bloop'
    }
  }
}

const KnightRider = (name) => {
  return {
    ...makeCar(name),
    ...robot(),

    drive: function() {
      return `Vroom. I'm KNIGHT RIDER`;
    }
  }
}

const kr = KnightRider('kr');
// console.log(`The value of kr is: `)
// console.log(kr)


Then went to inline using head and tail


## **Thursday**
HW, Project, What to learn for final...  

1 string building   2 looping   3 filtering   4 mapping   5 copying objects so they aren't mutated   6 using callbacks (taking functions as parameters)   7 factory functions (functions that return objects

projects to review:

Datasausr
Oops
Grado raide
uptown funk
filter feeder *** try inline
Cartographer 
Ray
methodfunctionKill

**keyboard shortcuts to remember**  
* multiplt cusors: click at end of one word 
* option click at end of another word.
* Also, highlight a word and then click command D to grab the next of same word  
* select word, command shift L selects them all