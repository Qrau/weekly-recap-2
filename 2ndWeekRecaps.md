# Wilderz Chill Monday!  
## Second week recap!
In this document we will do quick Recap about what we learned the last week :).. Javascript Basics, Git and GitHub, and other topics that we all went through.. 
# Berlin Wilderz! Let's call the Monday function :D..


#
#


## Git & GitHub :
___
#
#

1. ## creating Git locally
##### `[git init]`  will create new repository or update an existing one.
##### `[git clone URL]` will download a repository from online (GitHub) to local (Git) directory.
##### `[git status]` will show if there were changes has been made on the repository files.
#####  after doing some changes to your files, you can `[git add .]` it to your local Git, then add :
##### `[git commit -m"NAME YOUR CHANGES HERE"]` to commit the changes on your local Git repository.
##### `[git push URL]` will upload the added and committed changes from local Git repository to the online GitHub URL repository.
#
#

2. ## using Git branches

after cloning a project we can create branches from the master copy that we have cloned using these codes :
##### `[git branch]`  will show the status of the branches
##### `[git branch NAME-YOU-CHOSE]` will create a new branch within the given name.
##### `[git checkout]` will switch to the branch that you have just created.
#####  after commting changes on your local Git branch, you can `[git push origin branch_name]` to upload the branch.
#
#

3. ## related links and documents

Git and GitHub are very easy to use if you understand how they work, there are many thing you can do using Git and GitHub together.

- the simple guide - no deep shit!.... is a very useful article to understand Git and Github
https://rogerdudler.github.io/git-guide/
- Simple Git workflow.... is a very useful article to understand Git and Github workflow
https://www.atlassian.com/git/articles/simple-git-workflow-is-simple
- A Complete list of all Git Commands

  https://git-scm.com/docs/git#_git_commands

- CHIP AND DALE Wild workshop

  https://wildcodeschool.github.io/workshop-git/

- How to use .gitignore

  https://www.toolsqa.com/git/git-ignore/

#
#
#
## Javascript basics :
___
##


#
#

1. ## let, const and var

               {
               let myFirstName = "Alexander";
               console.log("My name is "+ myFirstName + " the Great!");
               }

               // results: My name Alexander the Grea!


##### in the example above we can replace the `[let]` command with `[const]` or `[var]`, what are the differences between them? you can check that by checking [this-link](https://dev.to/sarah_chima/var-let-and-const--whats-the-difference-69e#:~:text=var%20declarations%20are%20globally%20scoped%20or%20function%20scoped%20while%20let,be%20updated%20nor%20re%2Ddeclared.) out.
#
#
#
- ### to understand why we put our code inside `{}` will show you one example
               {
               let myFirstName = "Alexander";
               console.log("My name is "+ myFirstName + " the Great!");
               }

               {
               let myFirstName = "Cleopatra";
               console.log("My name is "+ myFirstName + " the Wicked!");
               }

               // results: My name Alexander the Grea!
               // and: My name is Cleopatra the Wicked!

#
- ### but if we do the same code WITHOUT writing our code in `{}` will show an Error
               
               let myFirstName = "Alexander";
               console.log("My name is "+ myFirstName + " the Great!");
              
               
               let myFirstName = "Cleopatra";
               console.log("My name is "+ myFirstName + " the Wicked!");
               

               // results: Uncaught SyntaxError: 
               // Identifier 'myFirstName' has already been declared 

#
- ### the same thing applies to the  `[if]`, `[for]`, `[while]` and similar commands
               
               if (true)
               {
               let message = "Hello!";
               alert(message);   // results: Hello!
               }
               alert(message);   // results: message is not defined
 
- ### example  `[for]` and `[while]` loops
               
               for (let i = 0; i < 3; i++) {
                   alert(i); // results: 0, then 1, then 2
                   }
               alert(i); // results: Error, no such variable

 
             
               
            

#
#
#
#
#
2. ## objects and arrays
               

               {
                 let listOfNumbers = [2, 3, 5, 7, 11];
               console.log(listOfNumbers[2]);
               // → 5
               console.log(listOfNumbers[0]);
               // → 2
               console.log(listOfNumbers[2 - 1]);
               // → 3
               }

               {
                 let sequence = [1, 2, 3];
                 sequence.push(4);
                 sequence.push(5);
                 console.log(sequence);
                 // → [1, 2, 3, 4, 5]
                 console.log(sequence.pop());
                 // → 5
                 console.log(sequence);
                 // → [1, 2, 3, 4]
               }


##### objects and arrays are sort of categorising your elements, if you still feel missing the basics you can check [this-link](https://www.simplilearn.com/javascript-arrays-and-objects-tutorial) out to follow up :)..
#
#
#
- ### some good examples of codes that simplify it
               {
               let object1 = {value: 10};
               let object2 = object1;
               let object3 = {value: 10};

               console.log(object1 == object2);
               // → true
               console.log(object1 == object3);
               // → false

               object1.value = 15;
               console.log(object2.value);
               // → 15
               console.log(object3.value);
               // → 10
               }
- ### modifying an object

               {
                 let anObject = {left: 1, right: 2};
               console.log(anObject.left);
               // → 1
               delete anObject.left;
               console.log(anObject.left);
               // → undefined
               console.log("left" in anObject);
               // → false
               console.log("right" in anObject);
               // → true
               }

- ### you can create an object with differenet elements and console it in one line!


               {
               console.log(Object.keys({x: 0, y: 0, z: 2}));
               // → ["x", "y", "z"]
               }
               // or
                 console.log(Object({x: 0, y: 0, z: 2}));   
               // → Object {
                 x: 0,
                 y: 0,
                 z: 2
               }

- ### Object.assign command


               {
               let objectA = {a: 1, b: 2};
               Object.assign(objectA, {b: 3, c: 4});
               console.log(objectA);
               // → {a: 1, b: 3, c: 4}
               }
       

#
#
#
#
#
3. ## functions
![javascript function.](https://storage.googleapis.com/quest_editor_uploads/spxzevSxmv7QXvFF5TkcMDkhTwthpmGb.png "")

               

               {
                 function helloWorld(){
	                 console.log("Hello,");
	                 console.log("World!");
                 }
               }
               helloWorld();
               // → Hello,
               // → World!




##### to know more about functions basics you can check [this-link](https://javascript.info/function-basics) out to follow up :)..
#
#
#
- ### Inner variable inside a function is only visible inside that function.
               function showMessage() {
                 let innerVariable = "Hello!";
                 alert(innerVariable);
               }
               showMessage(); // Hello!

               alert(innerVariable); // <-- Error! 
#

- ### A function can access an outer variable as well
               let outerVariable = 'John';
               function showMessage() {
                 let message = 'Hello, ' + outerVariable;
                 alert(message);
               }
               showMessage(); // Hello, John

#

- ### A The function has full access to the outer variable. It can modify it as well.
               let userName = 'John';
               function showMessage() {
                 userName = "Bob"; // 
                 let message = 'Hello, ' + userName;
                 alert(message);
               }
               alert(userName); 
               // John before the function call
               showMessage();
               alert(userName); 
               // Bob, the value was modified by the function
#
#
#
#
#
4. ## Parameters and Arguments
#


- ### Consider the following add() function:
               function add(x, y) {
                  return x + y;
               }
               add(100,200);
##### In this example, the x and y are the parameters of the add() function, and the values that we passed to the add() function 100 and 200 are the arguments.
#
#
- ### get the current date using parameters, try it yourself
               function functionName(firstParameter = today()) {
                 console.log(firstParameter);
               }

               function today() {
                 return (new Date()).toLocaleDateString("en-US");
               }
               functionName();
#
#
- ### assigning parameters values
               function add(x = 1, y = x, z = x + y) {
                   return x + y + z;
               }
               console.log(add()); // 4

#
#
- ### the arguments object

               function add(x = 1, y = x, z = x + y) {
                   return x + y + z;
               }
               console.log(add()); // 4
#
#
- ### another simple example

               function add(x, y = 1, z = 2) {
                   console.log( arguments.length );
                   return x + y + z;
               }

               add(10); // 1
               add(10, 20); // 2
               add(10, 20, 30); // 3
##### The value of the arguments object inside the function is the number of actual arguments that you pass into. See this example:.
#
#
#

#
5. ## The for loop
![javascript function.](https://cdn-images-1.medium.com/max/640/1*QoMetPjm8T-N9Ii8gfqvag.png)

               for (let i = 0; i < 5; i++) {
                  console.log(i);
               }

               // Results:
               0
               1
               2
               3
               4
#
#
- ### 0-index based counter
##### For loop counters are 0-index based. Let’s skip the middle statement and try breaking out of the loop using our own condition (i > 1):
               for (let i = 0;; i++) {
                   console.log("loop, i = " + i);
                   if (i > 1)
                       break;
               };
               // Results:
               "loop, i = 0"
               "loop, i = 1"
               "loop, i = 2"

#
#
- ### Loop’s Length

               {
               for (let i = 0; i < 3; i++) console.log("loop");
               }
               // results:
               // “loop.”
               // “loop.”
               // “loop.”

#
#
- ### for…of Loops And Strings

               let string = 'text';
               for (let value of string)
                 console.log( value );
               // results:
               // 't'
               // 'e'
               // 'x'
               // 't'
#
#
- ### for…of Loops And Arrays

               let array = [0, 1, 2];
               for (let value of array)
                 console.log( value );
               // results:
               // 0
               // 1
               // 2
#
#
6. ## related links and documents

JavaScript is a text-based programming language used both on the client-side and server-side that allows you to make web pages interactive..

- The Modern JavaScript Tutorial
https://javascript.info/intro
- What can JavaScript do?
https://www.w3schools.com/js/js_examples.asp
- The Complete Guide to Loops in JavaScript
https://morioh.com/p/b8bf0ec1d5d7
- Variable scope, closure
https://javascript.info/closure
- Data Structures: Objects and Arrays
  https://eloquentjavascript.net/04_data.html
- The && and || Operators in JavaScript
  https://mariusschulz.com/blog/the-and-and-or-operators-in-javascript
#
#
#
#
#
## Finally.. 
___

Still some un-categorise-able notes I share randomly with you:
- we can review our hard challenges with the Speaker on Wednesdays between 4 and 5 pm, we also have to split in groups and orgnize it.
- Each of us bring one bag of coffee on Monday. 
- Reviewing the quests only for the big challenges will happen with Wilfredoo, or share the solution.
- we can do our own workshop, where we share our knowledge together, whatever you think you can bring.
- we audio speaker to hear the Guest calls.
- thanks for your attention! Good luck...



#
#
#
#
#
#
#
#
#
#
#
#
#
#
#
