# Typescript basics

## Variable
C:
int age = 20

Javascript:
let age = 20

Typescript:
let age: number

## let and const

let age = 20
age = 21

const age = 20
age = 21 //not allowed

## Types

Javascript:
let name = "pig8y"      // string
let age = 20            // number
let isStudent = true    // boolean
let data                // undefined
let value = null        // null

Typescript:
let name: string = "pig8y"      
let age: number = 20            
let isStudent: boolean = true    
let data: undefined                
let value: null = null 

## Function

C:
int function(int a, int b) {
        return a + b;
}

Javascript:
function add(a, b) {
        return a + b
}

Typescript:
function(a: number, b: number): number {
        return a + b
}

## Arrow function
Typescript:
const add = (a: number, b: number): number => a + b

## Condition
C:
if (age >= 18) {
        printf("adult\n");
} else {
        printf("minor\n");
}

Javescript/Typescript:
if (age >= 18) {
        console.log("adult\n");
} else {
        console.log("minor\n");
}

## Object
C:
struct task {
        int id;
        char title[100];
        bool completed;
};

Javascript:
const task = {
        id: 1,
        title: "Revise Typescript",
        completed: false,
};

Typescript:

type Task = {
        id: number;
        title: string;
        completed: boolean;
};

const task: Task {
        id: 1,
        title: "Revise Typescript",
        completed: false,
}

let object:

let task: Task = {
        id,
        title,
        completed,
};

## Type

type Task = {
        id: number;
        title: string;
        completed: boolean;
};

## Optional property

type Goal = {
        id: number;
        title: string;
        description?: string;
};

const goal: Goal = {
        id: 1,
        title: "learn Typescript basics";
}

if (goal.description) {
        console.log(goal.description)
}

## Union type

type TaskStatus = "todo" | "inProgess" | "done"
type Task = {
        id: number;
        title: string;
        status: TaskStatus;
}

const task: Task = {
        id: 1,
        title: "Revise Typescript",
        status: "inProgess",
};


## null and undefined

undefined = no value assigned yet/ does not exist
null = set to empty intentionally

## Destructuring

Definition: destruct the value from object/array, become variable

type TaskStatus = "todo" | "inProgess" | "done"
type Task = {
        id: number;
        title: string;
        status: TaskStatus;
}

const task: Task = {
        id: 1,
        title: "Revise Typescript",
        status: "inProgess",
};

const { id, title, status } = task
console.log(id)         // 1
console.log(title)      // Revise Typescript
console.log(status)     // inProgrss

the variable name has to aglin with the object property name unless you've changed it

const { id: userId } = task // change the variable name
console.log(userId)     // 1

## Spread operator

const oldTask = ["read", "code"]
const newTask = [...oldTask, "review"] // ["read", "code", "review"]

const task = {
        id: 1,
        title: "Revise Typescript",
        status: "inProgess",
};

const updatedTask = {
        ...task,
        status: "done"
}       


// {
        id: 1,
        title: "Revise Typescript",
        status: "done"
   } 

## template literal
C:
pritnf("Hello, &s\n", name);

Javascript/Typescript:
const message = `Hello ${name}`

## async, await
Definition