# Reflection

## Question 1 (50 words)
#### When and why should you use a function like `carefulSubract` rather than `subtract`? 

A function like ‘subtract’ returns an undefined or NaN value when passed a parameter that is not a number, whereas a function like ‘carefulSubtract’ returns a string. By returning a string that specifies the problem, the reader/coder can determine whether or not the failure to return a number is a result of faulty code or the result of something other than a number being passed.

## Question 2 (100 words)
#### What are `data types`, and how does data typing work in JavaScript? Name at least 4 built-in data JS data types. 

In Javascript, ‘data types’ are specific form of data that are recognized by the code. Data types are set categories of data that can be tested (e.x. the type.of operator used in Problem 6 of the first set is able to test if a value is a specific data type). They are also treated in different ways by the code (e.x. Adding two numbers will yield a different result from adding a number and a string, as the code recognizes the difference between the data types). Some examples of Javascript data types are: numbers, strings, booleans, ‘null’ values, and ‘undefined’ values.

## Question 3 (100 words)
#### What is the advantage to storing information as an object (`{firstName: 'Italo', lastName: 'Calvino', profession: 'novelist' }`) rather than as an array (`['Italo', 'Calvino', 'novelist']`)? Are there any disadvantages?

By storing information as an object, you are able to easily access the information within each property of the object individually, with a clear syntax that specifies what each property is. Information stored in an array does not specify the properties of the elements within the array, and therefore cannot provide the same accuracy and detail as an object with properties. So instead of specifying elements of an array with [0] or [1] (etc…), information stored in an object allows elements to be specified with specific and easily identifiable syntax. With arrays, the elements can be rearranged and the code will no longer produce the same results, but with an object, the order of the properties will not impact the code as long as the values of the properties remain coordinated. While this is often an advantage, it can also be a disadvantage if the information that is being stored should be able to be moved around within the array.

## Question 4 (150 words)
#### The function `sentences` transforms a data structure (in this case, a list of object literals) into a sequence of sentences. If the data structure were less predictable (e.g., if some properties of each object were occasionally missing, or if their data type was not always the same), what programming techniques could you use to ensure that your function produced a coherent output? Also, can you think of a more interesting "transform" that could be done with the same data structure?

If the data structure of a list of object literals was missing properties or had changing data types, the coherence of the code output could be guaranteed by adding code that checks if the values are present and if the values are the correct data type. As used in Problem 6 of the first problem set, ‘if… else’ conditions can be used to clearly identify the missing or incorrect aspects of the properties and output strings that indicate these problems. Instead of simply returning ‘undefined’ or ‘NaN’ (etc.) to the console, this would mean that coherent strings are returned to the console. This data structure is used in the assignment to return a sentence, but it can also be used in a function that returns categorical information. For example, code can be written that, when passed an array of object literals with properties, returns sorted information based on specific property values that are called by the code. 