# JavaScriptPractice + notes-

Introduction: This tutorial contains examples and description of modern javascript.
-------------

Variable vs Constant Declaration (ES6)
--------------------------------------
1- var vs let vs const: var was present for defining the variables, ES6 introduced two new keywords let and const
a- let-> Used to define the variables
b- const-> Used to define the constant values

Note: It is better to use let/const instead of var.

Arrow Functions
---------------
Introduced in ES6 to allow to write shorter syntax

a- Traditional js function:
-----------------------------
var func = functionName(Arguments) {function body}

b-Arrow Functions
-----------------
const func = () => {funtion body}


Classes & Objects
-------------------
sytax:
class ClassName {
  constructor() { ... }

  funcion() {} //Class methods just like java
}

eg, class Employee {
		 constructor(name, salary) {
			 	this.name = name;
				this.salary=salary;
		 }

		 function getSalary() {
			 return this.salary;
		 }
		 function getName() {
			 return this.name;
		 }

}

ES6 Modules
--------------------
Modules are used to organize the code for re-use. It is just a javascript file.

Exporting from Module
----------------------
a- Export keyword is used to export the components from the module.

Example: suppose in file ./name.js following code is present
let name = "ark:
let upperCaseName =() => name.toUpperCase();

export { name, upperCaseName} ;//This will export these values to be used in another JS file


Importing the Module:
---------------------
b- import keyword is used to import a component from a module.


Example: code present in ./main.js

import {name, upperCaseName} from ./name.js;

Some GIT basics
----------------
To clone the repository -> git clone repoURL
To create the feature branch-> a- clone the project
                               b- git checkout -b feature_branch_name
							   c- commit changes -> git commit -m message
							   d- git push origin feature_branch_name