# Big O Assessment

 ### O Boy! It's time to evaluate your understanding of Big O Notation!

 ##

  PART ONE: Please answer the following questions:

 1. Describe the purpose of Big 0.

    > The purpose of Big O is to measure the efficiency of your algorithm

---


 2. What 2 things does it measure?

    > time and space

---


 3. Which of the following shows Big O time complexity in order?

    a) O(1), O(n log n), O(log n), O(n), O(n^2)

    b) O(1), O(log n), O(n), O(n log n), O(n^2)

    c) O(1), O(log n), O(n log n), O(n), O(n^2)

    > b

---



4. Which of these algorithm(s) run in O(log n) time?

   Binary Search

   Bubble Sort

   Quick Sort (average case)

   Linear Search

   > Binary search

---


5. Select the best time complexity that even the most efficient sort algorithm can have.

    O(log n)

    O(n log n)

    O(n)

    O(n^2)

    > O(log n)

---


 6. Describe what sets these these 3 complexities apart from each other: O(1), O(n) and O(n^2)

    >
    -O(1) - constant time - this kind of algorithm runs at the same speed no matter what the inputs are
    -O(n) - linear time - this kind of algorithm will decrease its efficiency at a linear speed
    -O(n^2) - this kind of algorithm's efficiency will decrease exponentially as the inputs increase

---


7. How would you recognize O(log n) and O(n log n) time complexities in a function?

    >
    -O(log n) - you would notice that each time a loop in your function runs, the data that you're searching through gets cut in half. sort of like a process of elimination (ie: binary search)
    -O(n log n) - you would notice that the data must be repeatedly changed and manipulated in order to get to your final goal. it is not very efficient (ie: merge sort)

---

  ##

  PART TWO: In a new file, write examples of algorithms/functions for each of the Big O complexities below.
    Upload your file to your repository when complete and submit in Learn --> Exercises.

    1. O(1)
    function one(arr) {
      return arr[0];
    }

    2. O(n)

    function n (arr,target) {
      for (var i=0; i < arr.length; i++) {
        if (arr[i] == target) {
             return true;
        }
      }
      return false;
    }

    3. O(n^2)

  function squared(arr) {
    let result = [];
    for (let i = 0; i < arr.length; i++) {
      for (let j = i; j < arr.length;i++) {
        if (arr[i] > arr[j]) {
          result.push(arr[j]);
        }
        else {
          arr.splice(i,1)
        }
      }
    }
    return result;
  }
