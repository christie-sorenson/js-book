# Data Types and Variables
The basic types JavaScript supports include numbers, strings, and Booleans. More complex types such as objects, arrays, and functions are also part of the language. This chapter covers in detail the basic data types and their usage. Functions and composite types, such as objects, are also briefly introduced, but a complete exposition of their capabilities is reserved for Chapters 5 and 6.

Adding some new text here to see what happens...


## Key Concepts


A variable can be thought of as a container that holds data. It's called a “variable” because the data it contains—its value—varies. For example, you might place the total price of items a customer is buying in a variable, and then add tax to this amount, storing the result back in the variable. 

The type of a variable describes the nature of the data stored. For example, the type of a variable holding the value 3.14 would be number while the type of a variable holding a sentence would be string. Note that “string” is programming language lingo for a sequence of characters—in other words, some text.

Since you need to have some way to refer to variables, each variable is given an identifier, a name that refers to the container and allows the script to access and manipulate the data it contains. Not surprisingly, a variable's identifier is often referred to as its name. When scripts are run, the JavaScript interpreter (the facility within the browser that executes JavaScript) needs to allocate space to store a variable's value. Declaring a variable is the process of telling the interpreter to get ready to associate data with the name. 

In JavaScript, variables are declared using the var keyword with the name of the variable you wish to declare. For example, you might write
```javascript
var firstName;
```
You can now store data in the variable known by the identifier firstName. Presumably, given the context of the name you'd be storing a string here. We could then assign a value like "Thomas" to the variable. We call the string "Thomas" a literal, which describes any data appearing directly in the source code. The complete example is now

```javascript
var firstName;
firstName = "Thomas";
```
The illustration here demonstrates all the terms used so far together.

Illustration 1
New illustration here based upon old – Rob/Andrew redo to come

Although it is good programming practice to declare variables before use, JavaScript allows the implicit declaration of variables by using them on the left-hand side of an assignment. In other words, when the interpreter sees a variable being assigned data it will create that variable automatically even if it hasn’t been previously declared using the var keyword. For example, you might just assign a variable, like so:
```javascript
lastName = "Schneider";
```
and whoosh it springs into existence. 
Unfortunately this feature of JavaScript can lead to less readable code and can also lead 
to subtle, hard-to-find errors involving variable scope, a topic we'll discuss later in the chapter. Unless you're writing a very simple script (less than a dozen lines), always explicitly declare your variables.


### Weak Typing


Many high-level languages, including C and Java, are strongly typed. That is, a variable must be declared before it is used, and its type must be included in its declaration. Once a variable is declared, its type cannot change. At the other end of the spectrum are untyped languages such as LISP. LISP supports only two primitive data types: atoms and lists. It does not draw any distinction between strings, integers, functions, and other data types. As a weakly typed language, JavaScript falls somewhere in between these two extremes. Every variable and literal has a type, but data types are not explicitly declared. For example, we might define 
a variable to hold our favorite number.  
```javascript
var favNumber;
```
Notice we don’t indicate what the type is of variable, though the name kind of gives away that it is a number and in this case our favorite one which is 3, so we assign it like so.
```javascript
favNumber = 3;
```
Now given that we aren’t indicating type it is possible assign the variable to be the string value "San Diego".
```javascript
favNumber = "San Diego";
```
Logically the example doesn't make much sense and it is certainly possible to continue on assigning it to a Boolean
```javascript
favNumber = true;
```
or even some complex type like an array.
```javascript
favNumber = ["Larry","Curly","Moe"];
```
Weak typing would seem to unleash our burden of thinking about type, but really it has its own peculiar concerns, so let’s sit and discuss how this all actually works.  First, when the variable `favNumber` is declared, it is empty. In fact, its data type is actually the type undefined. Then we assign it to the number 3, so its data type is Number. Next we reassign it to the string "San Diego", so the variable's type is now String. Later it is set to a Boolean and then even a composite type like an Array. As you can see, types are inferred from content, and a variable automatically takes on the type of the data it contains.  In some sense the variable is simply a name that references some arbitrary type of data and we are free to change what the name references at any time and use the value as we like.

As a comparison to JavaScript’s weak typing let’s observe what might happen in a more strongly typed language like C, Java, or Pascal. With such a language you might define the type allowed in `favNumber` explicitly, like so:
```javascript
var favNumber : number;
```
Given this example, an assignment like
```javascript
favNumber = 3;
```
would be perfectly valid. But if you assigned some non-numeric type to the variable like
```javascript
favNumber = "San Diego";
```
it would cause an error or warning to occur.   Weak typing of course would let things proceed without warning.

At first blush weak typing provides simplicity and flexibility since programmers don't have to worry about types, but it does so at the expense of runtime errors and security issues. We'll see many issues with weak typing throughout both the chapter and the book. For now, introducing the general concept is enough. Let's begin to look at each of the types in turn which will allow us to revisit the topic with a bit more depth.

Detecting when an infinite value has been reached use the isFinite() method found on the Global object.  For example,



### QUIZ

<quiz name="Gitbook Quiz">
    <question multiple>
        <p>What is gitbook used for?</p>
        <answer correct>To read books</answer>
        <answer>To book hotel named git</answer>
        <answer correct>To write and publish beautiful books</answer>
        <explanation>GitBook.com lets you write, publish and manage your books online as a service.</explanation>
    </question>
    <question>
        <p>Is it quiz?</p>
        <answer correct>Yes</answer>
        <answer>No</answer>
    </question>
    <question>
        <p>This is multiple dropdown quiz, in each dropdown select a correct number corresponding to the dropdown's order</p>
        <answer>
            <option correct>First</option>
            <option>Second</option>
            <option>Third</option>
            <option>Fourth</option>
        </answer>
        <answer>
            <option>First</option>
            <option correct>Second</option>
            <option>Third</option>
            <option>Fourth</option>
        </answer>
        <answer>
            <option>First</option>
            <option>Second</option>
            <option correct>Third</option>
            <option>Fourth</option>
        </answer>
        <answer>
            <option>First</option>
            <option>Second</option>
            <option>Third</option>
            <option correct>Fourth</option>
        </answer>
    </question>
</quiz>
