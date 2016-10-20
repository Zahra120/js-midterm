Instructions:

- Add your answers inline to the markdown file.
- Use your own words.
- Come up with an answer from memory. Write it down, even if the answer is "I don't know."
- Then, we will go over the answers in class. Write down your revised answer below your original answer.

---
### Part 1: Control Flow - 15 minutes

1. Draw a diagram of an if statement. Name each of the components and how they work together.
if (){


}

2. Draw a diagram of a for loop. Describe each of its components. Indicate the order in which they are executed / evaluated.
for (var i = 0; condition ; i++){


}

3. Functions
 - 3a. Draw a diagram of a function. Describe each of its components and what each component does. Specify which of them are optional.
 function name(){


}
 - 3b. Draw a diagram of a function being called, showing the instruction execution order.

   name();
---
### Part 2: Data Types - 10 minutes

4. Primitive Data Types
 - 4a. Give an example of an empty string and a non-empty string.

     var letter = "" ;
     var letter1 = "hello";
 - 4b. Give an example of a boolean.
     var num = true ;
      undefined = false;
 - 4c. Give an example of a Number.
      var num = 4;
5. Arrays
 - 5a. Give an example of an empty array.
     var arr = [];
 - 5b. Give an example of an array with three elements in it.
     var arr1 = [3,"hello", 34];
 - 5c. How do you add another element to this array?
      arr1 [arr1.length] = 23;
      arr1[3] = 23;
 - 5d. How do you get the length of this array?
   arr1.length
 - 5e. Show how to iterate through the array using a loop.
 for (var i = 0; i< arr1.length; i++){
     console.log(i);
}

6. Objects
 - 6e. Give an example of an empty object.
     var obj = {};
 - 6b. Give an example of an object with three keys and three values.
      var obj1 = {name : "zahra",
              surname : "fam",
              city : "leiden"
           }



 - 6c. Give an example of an object with two keys and two functions as values.
      var obj3 = {
         printHello : function(){

            console.log( "hello");
         },
         returnHello: function(){
             var h = "hello";
            return h;
         }

      }
 - 6d. Describe one way of adding a key to an object.
      var obj = {}
         obj.key = "myname";
 - 6e. Describe the other way of adding a key to an object.
       obj["key"] = "myname";
 - 6f. Explain the difference between these two ways, and when it is appropriate to use each way.

 - 6g. Describe how to iterate though an object using a loop.
   var obj={
      key1:value1,
      key2 : value2,
      key3 : value3
   }
 var keys = [key1 ,key2, key3];
      for (var i = 0; i< 3; i++){

          console.log( obj.keys[i]);
      }

---
### Part 3: Algorithms - 20 minutes

7. What is an algorithm?


8. For the following problem, first write down how exactly to solve the problem in English. Once you are able to describe it in English, translate it into code.

```js
// Given an array of values, write a function that finds the index of where the value is located, and if nothing is found, returns -1.
 var array = [1,3,4];
 var index = function(value){
   for (var i = 0; i< array.length; i++){
      //console.log (i);
      if (array[i] === value) {
         var index0fvalue = i;
       }
      //else {
      //    return -1;
      // }

   }

   return index0fvalue ;//
}

// Do not use the indexOf function.
// example: for ['apple', 'orange', 'pineapple']
	// 'orange' returns '1'
	// 'durian' returns '-1'
```

9. Again, for the following problem, first write down how exactly to solve the problem in English. Once you are able to describe it in English, translate it into code.

```js
// Write a function that finds all the indexes of where the value is located and returns them in an array, and if nothing is found, returns -1
// example: ['apple', 'orange', 'orange', 'pineapple']
	// 'orange' returns [1,2]
```
```js
var array = [1,3,4];
var index = function(value){
   var array2 = [];

   for (var i = 0; i < array.length; i++) {
      if (array[i] === value) {
         array2[array2.length] = i;
      }
   }

   if (array2.length > 0) {
      return array2;
   } else {
      return -1;
   }
}
```
