# Prep topics Discussion :
We are about To discuss A few Intresting topics In JS Whcih Are : 
* Event Loop .
* JS callback functions.
* JS Promises.
* JS Async/Await.
* Test-Driven Development.
## **First Topic**

### **Event Loop :**
Have you ever Heard about "asynch In JS"?
in simple words when you write a code in js you will think it will be execudeted line by line .

Well It's Right But what if you Have lines Of codes Which need a Little bit of time To be executed - liek setTimeOut , Promises ETC... -

well here we go 
as you know behind the scene Every Thing executed In Call Stack.
each line will be executed and then the one After and so on .

but when we have as an exapmle  setTimeOut Built-in Function where it needs some time to be executed .
Here is an example to explain it :

![image1](/img1.png)

* Here the Stack is empty
let's see how the code will run :

![image2](/img2.png)

so it executes the first Log and then let's see :

![image3](/img3.png)
it will take the setTimeOut , wait that's it?
No.

After the setTimeOut be in the Stack it won't directly execute it So it will be sent to the Webapis
where There it will Take the 5 seconds to be ready to be sent
to the task queue , let's see this in pictures :


![image3](/img4.png)

![image3](/img5.png)

Now The event loop will check if the Stack is empty it will send the "Cb" To the Stack to be executed.
![image3](/img6.png)

### **So In Another Words :**
The event loop is The simplest part of this process and it has only one thing to do which is to look at the stack and to the task queue If the stack is empty it takes the first thing in the queue to send it to the stack to be executed. 


## **Second Topic**

### **JS callback functions :**
SO as we said in the previous topic JavaScript runs code sequentially in top-down order.
 But , there are some cases that code runs (or must run) after something else happens and also not sequentially , This  called asynchronous programming.


So the call back function is a JS function we use it to call a function inside another function  as a parameter  .

meaning that the call back function it makes sure it won't be run unless something happen first (the First Function run before) .

## **Third Topic**

### **JS Promises :**
The promise In Js is the ideal way to deal with asynch operayions.
 Also promises :
 * Improves Code Readability
* Give Better handling of asynchronous operations.
* Give Better flow of control definition in asynchronous logic.
* Better To Handle Errors .

### Promises states :
* fulfilled: Action related to the promise succeeded.
* rejected: Action related to the promise failed
* pending: Promise is still pending  not fulfilled or rejected yet.
* settled: Promise has fulfilled or rejected.

It Takes A callback Function with two params as resolved or receted.
Promise  Takes method as an exapmle .then method , so any thing in the .then will be executed after the promise itself depending on if the promise resolved or rejected.

* They are used for asynchronous handling.
* And They are used to handle asynchronous http requests.

## **Fourth Topic**

## **JS Async/Await :**
### async and await  work to work with promises in asynchronous Functions and they make promises easier to be written.

* async makes a function return a Promise meaning it's written before the function and make it asynchronous function to return  a promise .

* await makes a function wait for a Promise meaning it will make the function (promise) wait after the other  lines of codes run and the stack is empty the the thing inside await will run.
## **Fifth Topic**
### **Test-Driven Development :**
Test driven developement is (for my understanding) it's about testing codes .
in simple words it is a file which tests our code like we used to see testing json files in our problem solving codes.
it has ways and specifications for the test itself.
 
 ## in another words :
 it's the way to check if the code follows a specific way(test).

