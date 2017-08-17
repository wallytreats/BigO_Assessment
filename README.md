# Big O Assessment

 ### O Boy! It's time to evaluate your understanding of Big O Notation!

 ##

  PART ONE: Please answer the following questions:

 1. Describe the purpose of Big 0.

    > Big O is a method of measuring the overall complexity and efficiency of an algorithm in its worst case scenario.

---


 2. What 2 things does it measure?

    > Time and space of an algorithm OR how we measure the speed and the amount of memory required for an alogithm to run.

---


 3. Which of the following shows Big O time complexity in order?

    a) O(1), O(n log n), O(log n), O(n), O(n^2)

    b) O(1), O(log n), O(n), O(n log n), O(n^2)

    c) O(1), O(log n), O(n log n), O(n), O(n^2)

    > b) O(1), O(log n), O(n), O(n log n), O(n^2)

---



4. Which of these algorithm(s) run in O(log n) time?

   Binary Search

   Bubble Sort

   Quick Sort (average case)

   Linear Search

   > Binary Search

---



5. Select the best time complexity that even the most efficient sort algorithm can have.

    O(log n)

    O(n log n)

    O(n)

    O(n^2)

    > O(n)
    O(n) is the best time complexity for sorting algorithms. Of the above O(log n) is faster than O(n), however it is generally optimized for searching rather than sorting.

---


 6. Describe what sets these these 3 complexities apart from each other: O(1), O(n) and O(n^2)

    > O(1) is constant time, this means that it has a consistent action and times that it performs that action.
    O(n) is linear time which takes a consistently incrementing amount of time based upon the length or size of it's input.
    O(n^2) takes exponentially more time as the data set gets larger.


---


7. How would you recognize O(log n) and O(n log n) time complexities in a function?

    > Both are sorting algorithms. O(n log n) will sort and then possibly loop after sorting.

    > A function whose big O followed O(log n) would have one continuously shrinking computational feature, such as a recursion. A function whose big O followed O(n log n) would have a both a shrinking computational feature and a computational feature whose input would vary in size.

---

  ##

  PART TWO: In a new file, write examples of algorithms/functions for each of the Big O complexities below.
    Upload your file to your repository when complete and submit in Learn --> Exercises.

    1. O(1)

    function countTo10 (){
      for(var i = 0; i <= 10; i++) {
        console.log(i);
      };
    };
    countTo10();

    2. O(n)

    function sum(array) {
      let sum = 0;
      for(var i = 0; i < array.length; i++) {
        sum += array[i]
      }
      return sum;
    }

    sum([1,2,3]);

    3. O(n^2)

    var string = "Mississippi";

    function containsDups(string) {
      for(var i = 0; i < string.length; i++){
        for (var j = 1; j < string.length; j++){
          if (i === j) {
            console.log('true');
          }
          else {
            console.log('false');
          }
        }
      }
    };
    containsDups(string);
