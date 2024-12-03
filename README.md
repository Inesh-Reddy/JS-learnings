# Callbacks and Higher-Order Functions

    Challenge 1 :
    Create a function addTwo that accepts one input and adds 2 to it.

    Challenge 2 :
    Create a function addS that accepts one input and adds an "s" to it.

    Challenge 3 :
    Create a function called map that takes two inputs:
    an array of numbers (a list of numbers)
    a 'callback' function - a function that is applied to each element of the array (inside of the function 'map')
    Have map return a new array filled with numbers that are the result of using the 'callback' function on each element of the input array.

        map([1,2,3,4,5], multiplyByTwo); //-> [2,4,6,8,10]
        multiplyByTwo(1); //-> 2
        multiplyByTwo(2); //-> 4`

    Challenge 4 :
    Create a function called forEach that takes an array and a callback, and runs the callback on each element of the array. forEach does not return anything.
    let alphabet = '';
    const letters = ['a', 'b', 'c', 'd'];
    forEach(letters, function(char) {
    alphabet += char;
    });
    console.log(alphabet);   //prints 'abcd'

    Challenge 5 :
    In challenge 3, you've created a function called map. In this challenge, you're going to rebuild the map function by creating a function called mapWith. This time you're going to use forEach inside of mapWith instead of using a for loop.

    Challenge 6 :
    Create a function called reduce that takes an array and reduces the elements to a single value. For example it can sum all the numbers, multiply them, or any operation that you can put into a function.
    const nums = [4, 1, 3];
    const add = function(a, b) { return a + b; }
    reduce(nums, add, 0);   //-> 8
    Here's how it works. The function has an "accumulator value" which starts as the initialValue and accumulates the output of each loop. The array is iterated over, passing the accumulator and the next array element as arguments to the callback. The callback's return value becomes the new accumulator value. The next loop executes with this new accumulator value. In the example above, the accumulator begins at 0. add(0,4) is called. The accumulator's value is now 4. Then add(4, 1) to make it 5. Finally add(5, 3) brings it to 8, which is returned.

    Challenge 7 :
    Construct a function intersection that takes in an array of arrays, compares the inner arrays, and returns a new array with elements found in all of them. BONUS: Use reduce!

    Challenge 8 :
    Construct a function union that takes in an array of arrays, compares the inner arrays, and returns a new array that contains all elements. If there are duplicate elements, only add it once to the new array. Preserve the order of the elements starting from the first element of the first array. BONUS: Use reduce!

    Challenge 9 :
    Construct a function objOfMatches that accepts two arrays and a callback. objOfMatches will build an object and return it. To build the object, objOfMatches will test each element of the first array using the callback to see if the output matches the corresponding element (by index) of the second array. If there is a match, the element from the first array becomes a key in an object, and the element from the second array becomes the corresponding value.

    Challenge 10 :
    Construct a function multiMap that will accept two arrays: an array of values and an array of callbacks. multiMap will return an object whose keys match the elements in the array of values. The corresponding values that are assigned to the keys will be arrays consisting of outputs from the array of callbacks, where the input to each callback is the key.
