# ES-6
# Introduction to ES6

ES6 is also known as ECMAScript 2015. It is a standardised scripting language for JavaScript (JS), It allows us to write code in a clever way which basically makes the code more modern and more readable. It contains a lot of features (let, const, arrow functions, class, promises etc.) to standardize javascript. It is generally used for client-side scripting, and it is also used for writing server applications and services by using Node.js.

# Basic datatypes Of ES6


Primitive datatypes

    • Null
    
    • Boolean
    
    • Undefined
    
    • Number
    
    • BigInt
    
    • String
    
    • Symbol (New in ES6)
        
# 1. Null



   The null in JavaScript is a data type that is represented by only one value, JavaScript null is a primitive type that contains a special value null, the ‘null’ itself. A null value means no value.

Syntax : null

var a = null;

console.log(a);   // This returns null

# 2. Boolean


Boolean datatype represents a logical entity. it can have two values: true and false. In JavaScript, the Boolean is used as a function to get the value of an object, a variable, conditions, expressions, and many more in terms of true and false.

Syntax : var val = new Boolean(value);

Example :

var a = 2, b = 5, c = 10;

alert(b > a) // true

alert(b > c) // false

# 3. Undefined


A variable that has not been assigned a value has the value undefined. undefined is a property of the global object. That is, it is a variable in global scope. The initial value of undefined is the primitive value undefined.
With the var keyword, we’re declaring a variable, but until a value is assigned to it, it’s undefined.

Syntax : undefined

Example :

var a;

alert(a);

In the above example, we have not assigned any value to a variable named 'a'. So it is undefined.

# 4. Number


Number represents integer and floating numbers (decimals and exponentials).

Syntax : number

Example :

    let n = 310;
    
    n = 12.345;
    
# 5. BigInt


The bigint type represents the whole numbers that are larger than 253-1. To form a bigint literal number, you append the letter n at the end of the number.

Syntax : BigInt(number)

Example :

let bigInt = 9007199254740991n;

var bigNum = BigInt(

"123422226666555557777777");

console.log(bigNum);


var bigHex = BigInt("0x1ffffffeeeeeeeeef");

console.log(bigHex);

var bigBin = BigInt(

"0b10101010010101010011111111");

console.log(bigBin);

# 6. String


In JavaScript, a string is a sequence of zero or more characters. A string literal begins and ends with either a single quote('), a double quote ("), and backticks(`).
JavaScript's String type is used to represent textual data. It is a set of "elements" of 16-bit unsigned integer values. Each element in the String occupies a position in the String. The first element is at index 0, the next at index 1, and so on. The length of a String is the number of elements in it.

Syntax : keyword string_name

Example :

let greeting = 'Hi';

let message  = "Bye";

let msg = 'I\'m also a valid string'; // use \ to escape the single quote (')

# 7. Symbol


The JavaScript ES6 introduced a new primitive data type called Symbol. Symbols are immutable (cannot be changed) and are unique.

Syntax : keyword variablename Symbol()

Example :

      let s1 = Symbol();
      
    console.log(Symbol() == Symbol()); // false
    

# Data Structure in ES6


7 most used data structures
    • Arrays
    
    • Stack
    
    • Queues
    
    • Linked List
    
    • Trees
    
    • Graphs
    
    • Hash table
    
    • Map
    
    • Set
    
# 1. Arrays


Arrays are the most basic data structure. It is a group of similar types of elements stored together at contiguous memory locations and each cell has a corresponding numeric index used to select its data.

Example :

var arr=["prabhas","sumit","deepak"];

for (i=0;i<arr.length;i++){  

document.write(arr[i] + ", ");  //[prabhas sumit deepak]

}

# 2. Stack


Stack is a linear data structure that follows the LIFO(Last In First Out) or FILO(First In Last Out) principle. It contains only one pointer the top pointer that points to the topmost element of the stack. Whenever we add an element to the stack, it is added at the top of the stack and also whenever we delete an element from the stack it is deleted from the top of the stack.

Example :

class Stack {

constructor()

{

    this.items = [];
    
}

In above definition we have created a skeleton of a stack class which contains a constructor in which we declare an array to implement stack.

# 3. Queue


Queue Data Structure is a collection of elements that implements the FIFO principle, First In First Out. Its main actions are enqueued to insert an element, dequeue to remove, and peek(sometimes referred to as peep) to look at the top element.

Example :

    var queue = [];
    
    queue.enqueue(2); 
    
    queue.enqueue(5);  
    
    var i = queue.shift(); 
    
    alert(i);             

# 4. Linked List


The linked list is a linear data structure in which elements are not in contiguous memory locations. It consists of a group of nodes and each node has its own data and address to the next node. The entry point to a linked list is called the head. The head is a reference to the first node in the linked list. The last node on the list points to null. If a list is empty, the head is a null reference.

Example :

const list = {

    head: {
    
        value: 6
        
        next: {
        
            value: 10 
            
            next: {
            
                value: 12
                
                next: {
                
                    value: 3
                    
                    next: null  
                    
                    }
                    
                }
                
            }
            
        }
        
    }
    
};

# 5. Tree


The tree is a non-linear hierarchical data structure consists of nodes connected by edges. Each node contains some data and the link of other nodes that can be called children. The topmost node of the tree is known as a root node. Nodes with linked child nodes are called internal nodes while those without child nodes are external nodes(leaf nodes).

There are a number of different types of trees:-

1. Binary Tree

2. Binary Search Tree

3. AVL Tree

4. Balanced tree

5. Red black tree

6. 2-3 tree

7. N-ary tree

Example :

class Tree {

constructor(data) {

  let node = new Node(data);
  
  this._root = node;
  
}
Tree contains two lines of code. The first line creates a new instance of Node; the second line assigns node as the root of a tree.

# 6. Graph


A graph is a common data structure consists of a finite set of nodes and edges. A graph can be seen more like a network. The interconnected objects are represented by points known as vertices, and the links that connect the vertices are called edges.
There are two common types of graphs:-
    • Undirected Graphs => In an undirected graph, edges are not associated with the directions with them. It means if an edge exists between vertex X and Y then the vertices can be traversed from Y to X as well as X to Y.
    • Directed Graphs => In a directed graph, edges are associated with the directions with them. It means if an edge exists between vertex X and Y then the vertices can be traversed from X to Y only. Here, vertex A is called the initial node while vertex B is called the terminal node.
    
Example :

class Graph {

    constructor(noOfVertices)
    
    {
    
        this.noOfVertices= noOfVertices;
        
        this.AdjList = new Map();
        
        }
        
    }
    
# 7. Hash table


Hash Table(also called a hash, hash map) is a data structure that stores the data in an associative manner using hashing. Hashing is the technique of mapping keys, values into the hash table by using a hash function. Here “key” is a searched string and the “value” is the data paired with that key.

Example :

    class HashTable {
    
    constructor() {
    
    this.values = {};
    
    this.length =  0;
    
    this.size =  0;
    
    }
    
    calculateHash(key) {
    
    return key.toString().length % this.size;
    
    }
    
}
The constructor contains an object in which we’re going to store the values, the length of the values, and the entire size of the hash table. This function takes the provided key and returns a hash that’s calculated using an arithmetic modulus.

# 8. Map


Maps are collections of keys and values of any type, in simple word Map is a collection of Key-value pairs. It works like an object in JavaScript. It returns a new or empty map.

Example :

const map1 = new Map();

map1.set('a', 1);

map1.set('b', 2);

map1.set('c', 3);

console.log(map1.get('a'));
// expected output: 1

map1.set('a', 97);

console.log(map1.get('a'));
// expected output: 97

console.log(map1.size);
// expected output: 3

map1.delete('b');

console.log(map1.size);//2

# 9. Set


It is a data structure introduced in ES6 version. A Set is a collection of values like an array but it don’t contain any duplicates. It is mutable so that our program can add and remove values as it goes. It returns set object.

Example :

const mySet1 = new Set()

mySet1.add(1) 

mySet1.add(5) 

mySet1.add(5) 

mySet1.add('hello')

const o = {a: 1, b: 2}

mySet1.add(o)

mySet1.add({a: 1, b: 2}) 

console.log(mySet)

# References :


* https://www.geeksforgeeks.org/es6-collection/

* https://dev.to/nehasoni__/7-javascript-data-structures-you-must-know-57ah

* https://www.javascripttutorial.net/javascript-data-types/

* https://developer.mozilla.org/en-US/docs/Web/JavaScript/Data_structures
