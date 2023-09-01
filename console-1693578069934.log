// Generic Object
undefined
var obj = {id:101, name:'Ram', city:'Delhi'};
undefined
typeof obj;
'object'
obj instanceof Object;
true
typeof Object;
'function'
function createEmp(id, name , salary){
    var emp = {}; // Object Literal
    emp.id = id;
    emp.name = name;
    emp.salary = salary;
    return emp;
}
undefined
var ram = createEmp(1001, 'Ram', 22222);
undefined
ram;
{id: 1001, name: 'Ram', salary: 22222}
typeof ram;
'object'
ram instanceof Object;
true
ram instanceof createEmp;
false
var shyam = createEmp(1002, 'Shyam', 122222);
undefined
shyam;
{id: 1002, name: 'Shyam', salary: 122222}
var tom = createEmp(1003, 'Tom', 122222);
undefined
tom;
{id: 1003, name: 'Tom', salary: 122222}
// Specific Objects
undefined
function Person(id, name ,age){
    console.log('Person ',this);
}
var tim = new Person(1001, 'Tim',21);
VM960:2 Person  Person {}
undefined
tim instanceof Person;
true
tim instanceof Object;
true
// Function Constructor
function Person(id, name ,age){
    console.log('Person ',this);
    this.id = id;
    this.name = name;
    this.age = age;
    console.log('Person with Values ',this);
    // this - keyword - current calling object reference
}
var tim = new Person(1001, 'Tim',21);
VM1185:3 Person  Person {}
VM1185:7 Person with Values  Person {id: 1001, name: 'Tim', age: 21}
undefined
// what is prototype?
undefined
function Customer(id, name, balance){
    
}
var tom = new Customer(1001, )
undefined
function Customer(id, name, balance){
    this.id = id;
    this.name = name;
    this.balance = balance;
}
var tom = new Customer(1001, 'Tom', 22222);
var tim = new Customer(1002, 'Tim', 322222);
var kim = new Customer(1003, 'Kim', 42222);

undefined
tom;
Customer {id: 1001, name: 'Tom', balance: 22222}
tim;
Customer {id: 1002, name: 'Tim', balance: 322222}
kim;
Customer {id: 1003, name: 'Kim', balance: 42222}
function Customer(id, name, balance){
    this.id = id;
    this.name = name;
    this.balance = balance;
    this.printCustomer = function(){
        console.log(`Id is ${this.id} Name ${this.name} Balance ${this.balance}`);
    }
}


undefined
var tom = new Customer(1001, 'Tom', 22222);
var tim = new Customer(1002, 'Tim', 322222);
var kim = new Customer(1003, 'Kim', 42222);
undefined
tom;
Customer {id: 1001, name: 'Tom', balance: 22222, printCustomer: ƒ}
tim
Customer {id: 1002, name: 'Tim', balance: 322222, printCustomer: ƒ}
kim;
Customer {id: 1003, name: 'Kim', balance: 42222, printCustomer: ƒ}
tom.printCustomer();
VM1637:6 Id is 1001 Name Tom Balance 22222
undefined
tim.printCustomer();
VM1637:6 Id is 1002 Name Tim Balance 322222
undefined
kim.printCustomer();
VM1637:6 Id is 1003 Name Kim Balance 42222
undefined
Customer;
ƒ Customer(id, name, balance){
    this.id = id;
    this.name = name;
    this.balance = balance;
    this.printCustomer = function(){
        console.log(`Id is ${this.id} Name ${this.name} Balance $…
Customer.prototype;
{constructor: ƒ}
typeof Customer.prototype;
'object'
Customer.prototype instanceof Object;
true
tom;
Customer {id: 1001, name: 'Tom', balance: 22222, printCustomer: ƒ}
tim;
Customer {id: 1002, name: 'Tim', balance: 322222, printCustomer: ƒ}
kim;
Customer {id: 1003, name: 'Kim', balance: 42222, printCustomer: ƒ}
tom.__proto__ === Customer.prototype;
true
tom.__proto__ === tim.__proto__ && tom.__proto__ === kim.__proto__;
true
Customer.prototype.show= function(){
    console.log(`Id is ${this.id} Name ${this.name} Balance ${this.balance}`);
}
ƒ (){
    console.log(`Id is ${this.id} Name ${this.name} Balance ${this.balance}`);
}
tom.show();
VM2395:2 Id is 1001 Name Tom Balance 22222
undefined
kim.show();
VM2395:2 Id is 1003 Name Kim Balance 42222
undefined
tim.show();
VM2395:2 Id is 1002 Name Tim Balance 322222
undefined
tim;
Customer {id: 1002, name: 'Tim', balance: 322222, printCustomer: ƒ}balance: 322222id: 1002name: "Tim"printCustomer: ƒ ()[[Prototype]]: Objectshow: ƒ ()constructor: ƒ Customer(id, name, balance)[[Prototype]]: Object
tim.show();
VM2395:2 Id is 1002 Name Tim Balance 322222
undefined
tim.__proto__;
{show: ƒ, constructor: ƒ}
tim.__proto__ === Customer.prototype;
true
tim.__proto__.show;
ƒ (){
    console.log(`Id is ${this.id} Name ${this.name} Balance ${this.balance}`);
}
tim.__proto__.show();
VM2395:2 Id is undefined Name undefined Balance undefined
undefined
tom.show();
VM2395:2 Id is 1001 Name Tom Balance 22222
undefined
tom.show(); // tom.__proto__.show()
VM2395:2 Id is 1001 Name Tom Balance 22222
undefined
tom.__proto__;
{show: ƒ, constructor: ƒ}
tom.__proto__.show();
VM2395:2 Id is undefined Name undefined Balance undefined
undefined
tom.__proto__.show.call(tom);
VM2395:2 Id is 1001 Name Tom Balance 22222
undefined
tom.show(); // tom.__proto__.show.call(tom)
VM2395:2 Id is 1001 Name Tom Balance 22222
undefined
