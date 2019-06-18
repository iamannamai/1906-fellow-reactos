# 1906 Fellows Algos Schedule

## Resources

- Refer to the [CtCI JS repo](https://github.com/careercup/CtCI-6th-Edition-JavaScript) for solutions to additional problems
- [CtCI ES2015](https://github.com/careercup/CtCI-6th-Edition-JavaScript-ES2015) for most up-to-date syntax
- Solutions can also sometimes be found in the [FSA Technical Interview Prep Repo](https://github.com/FullstackAcademy/technical-interview-prep/)
- [GIST TEMPLATE](https://github.com/FullstackAcademy/technical-interview-prep/blob/master/algorithms/reacto-template.md)

## Practicing Algos

- **REACTOS** - Pairs can be assigned each week, but the pair can self organize around _when_ they want to do their REACTOS. Questions are provided as starting points.
  - _Suggestion/Optional_: Interviewers _can_ create gists in preparation of walking through questions with their interviewees. These gists can look like the REACTOs delivered in Senior Phase, but at minimum should probably include:
    - Question
    - Examples/Test Cases
    - Hints (taken from CtCI, or provided)
    - At least one solution
    - Explanations of code
- **MOBBING** - Also provided are suggestions of questions to mob program together. Mobbing groups can self-organize based on REACTO pairs. We're taking a loose definition of mobbing, so we can decide the rules of engagement, but to start:
  - Everyone gets an understanding of the question
  - Anyone can pitch in with an approach
  - One driver (whiteboarder) at a time, switching off after 5 - 10min

## Schedule

### Week 1: Arrays and Strings

<details>

#### REACTOS

- **1.5 One Away**

  <details>
  There are three types of edits that can be performed on strings: insert a character, remove a character, or replace a character. Given two strings, write a function to check if they are one edit (or zero edits) away.
    <details><summary>Hints</summary>

      - #23 - Start simple. Can you check each of the conditions separately?
      - #97 - What is the relationship between "insert" and "remove"? Do they need to be two separate checks?
      - #130 - Can you do all three checks in a single pass?

    </details>
  </details>

  - **Solutions**: [CtCI JS](https://github.com/careercup/CtCI-6th-Edition-JavaScript/blob/master/chapter01/1.5%20-%20OneAway/oneAway.js) | [CtCI ES2015](https://github.com/careercup/CtCI-6th-Edition-JavaScript-ES2015/blob/master/src/chapter1/ch1-q5.js)
  - **Gists**: N/A

- **1.7 Rotate Matrix (aka Rotate Image)**

  <details>
  Given an image represented by an NxN matrix, where each pixel in the image is 4 bytes, write a method to rotate the image by 90 degrees. Can you do this in place?
    <details><summary>Hints</summary>

      - #51 - Try thinking about it layer by layer. Can you rotate a specific layer?
      - #100 - Rotating a layer means swapping the layer in 4 arrays. Could you swap the values in 2 arrays? Could you extend this to 4?

    </details>
  </details>

  - **Solutions:** [CtCI JS](https://github.com/careercup/CtCI-6th-Edition-JavaScript/blob/master/chapter01/1.7%20-%20Rotate%20Matrix/rotateMatrix.js) | [CtCI ES2015](https://github.com/careercup/CtCI-6th-Edition-JavaScript-ES2015/blob/master/src/chapter1/ch1-q7.js)
  - **Gists** - N/A
  - [LeetCode](https://leetcode.com/problems/rotate-image/)

- **1.8 Zero Matrix**

  <details>
  Write an algorithm such that if an element in an MxN matrix is 0, its entire row and column are set to 0

    <details><summary>Hints</summary>
      - #17 - Transforming the matrix as you encounter 0s would clear out the entire matrix. What can you do instead?
      - #74 - Can you minimize the additional space needed to `O(N)`? What information do you actually need to figure out the new matrix?
      - #102 - Can you further minimize the additional storage needed to `O(1)` by mutating the input?

    </details>

  </details>

  - **Solutions**: [CtCI JS](https://github.com/careercup/CtCI-6th-Edition-JavaScript/blob/master/chapter01/1.9%20-%20String%20Rotation/stringRotation.js) | [CtCI ES2015](https://github.com/careercup/CtCI-6th-Edition-JavaScript-ES2015/blob/master/src/chapter1/ch1-q9.js)
  - **Gists**: N/A
  - [LeetCode](https://leetcode.com/problems/set-matrix-zeroes/)

#### MOB

- 16.22 Langston's Ant
- 16.17 Contiguous Sequence (DP)

</details>

### Week 2: Linked Lists, Stacks and Queues

<details>

#### Notes on Chapter

<details>

Notes on the following data structures covered in this chapter can be found at [DS_AND_TECHNIQUES.md](DS_AND_TECHNIQUES.md).

- Linked Lists
- Stacks
- Queues

</details>

#### REACTOS

- **2.2 Return Kth to Last**

  <details>
    Implement an algorithm to find the kth to last element of a singly linked list.
    <details><summary>Hints</summary>

      - #8 - What if you knew the size of the linked list? What is the difference between finding Kth-to-last or Xth element?
      - #25 - If you don't know the linked list size, can you compute it?
      - #41 - Try implementing recursively.
      - #126 - Can you implement this iteratively? Imagine two adjacent pointers moving through the linked list at the same speed.

    </details>
  </details>

  - **Solutions**: [CtCI JS](https://github.com/careercup/CtCI-6th-Edition-JavaScript/blob/master/chapter02/2.2%20-%20Return%20Kth%20to%20Last/returnKthToLast.js) | [CtCI ES2015](https://github.com/careercup/CtCI-6th-Edition-JavaScript-ES2015/blob/master/src/chapter2/ch2-q2.js)
  - **Gists**: N/A
  - [AlgoExpert](https://www.algoexpert.io/questions/Remove%20Kth%20Node%20From%20End) | [LeetCode](https://leetcode.com/problems/merge-k-sorted-lists/) - Mostly the same question

- **3.4 Queue via Stacks**

  <details>
    Create a `MyQueue` class that implements a queue using two stacks.
      <details><summary>Hints</summary>
        - #98 - How could you remove the oldest item from a stack if you only had access to the newest item?
        - #114 - We can remove the oldest item from a stack by pushing everything into a new stack, and then pushing everything back. What is the time complexity of an operation like this?
      </details>
  </details>

  - **Solutions**: [CtCI JS](https://github.com/careercup/CtCI-6th-Edition-JavaScript/blob/master/chapter03/3.4%20-%20Queue%20via%20Stacks/queueViaStacks.js) | [CtCI ES2015](https://github.com/careercup/CtCI-6th-Edition-JavaScript-ES2015/blob/master/src/chapter3/ch3-q4.js)
  - **Gists**: N/A

- **16.26 Calculator**

  <details>
    Given an arithmetic equation consisting of positive integers and operations `+ - * /` (no parentheses), return the result.
    Ex. `2*3+5/6*3+15` returns `23.5`
    <details><summary>Hints</summary>
      - #520 - Can we simply go from left to right? Why/why not?
      - #623 & #664 - How would you prioritize your operators?
      - #697 - Consider maintaining separate stacks for your operators and numbers. When would you push/pop from these stacks?
    </details>
  </details>

  - **Solutions**: N/A
  - **Gists**: N/A

#### MOB

- 2.8 Loop Detection ([LeetCode](https://leetcode.com/problems/linked-list-cycle-ii/))
- 2.6 Palindrome (if you've already seen Loop Detection)
- 17.9 Kth Multiple

</details>

### Week 3: Trees and Graphs

<details>

#### Notes on Chapter

<details>

Notes on the following data structures covered in this chapter can be found at [DS_AND_TECHNIQUES.md](DS_AND_TECHNIQUES.md).

- Trees
- Binary Tree Traversal
- Binary Heaps
- Graphs

</details>

#### REACTOS

- **4.3 List of Depths**

  <details>
  Create a linked list of all the nodes at each depth of a binary tree. If you have a tree with depth D, you will have D linked lists.
    <details><summary>Hints</summary>

      - #107 - Try modifying a graph search algorithm to track the depth from the root
      - #123 - A hash table or array that maps from level number to nodes at that level might also be useful
      - #135 - You should be able to come up with an algorithm involving both DFS and BFS

    </details>
  </details>

  - **Solutions:** [CtCI JS](https://github.com/careercup/CtCI-6th-Edition-JavaScript/blob/master/chapter04/4.03%20-%20List%20of%20Depths/listOfDepths.js) | [CtCI ES2015](https://github.com/careercup/CtCI-6th-Edition-JavaScript-ES2015/blob/master/src/chapter4/ch4-q03.js)
  - **Gists:** N/A

- **4.4 Check Balanced**

  <details>
  Implement a function to check if a binary tree is balanced. Balanced refers to a tree such that the heights of the two subtrees of any node never differs by more than one.
    <details><summary>Hints</summary>

      - #21 - Can you check the condition for a balanced tree for a single node? How about every node?
      - #33 - Computing the height of a subtree for each node might be fairly inefficient. What is the runtime for a brute force approach?
      - #49 & #105 - What if you could access the height of a node's subtree AND compute whether the node is balanced
      - #124 - Consider a helper function to check the height and balance of a node

    </details>
  </details>

  - **Solutions:** [CtCI JS](https://github.com/careercup/CtCI-6th-Edition-JavaScript/blob/master/chapter04/4.04%20-%20Check%20Balanced/checkBalanced.js) | [CtCI ES2015](https://github.com/careercup/CtCI-6th-Edition-JavaScript-ES2015/blob/master/src/chapter4/ch4-q04.js)
  - **Gists:** N/A
  - [LeetCode](https://leetcode.com/problems/balanced-binary-tree/)

- **4.7 Build Order**

  <details>
    Given a list of projects and dependencies, where a dependency is an array of pairs where the first project of the pair is dependent on the second project, find a build order that will allow the projects to be built. Return an error if there is no valid build order. All of a project's dependencies must be build before the project is. Ex:

  - projects: `a, b, c, d, e, f`
  - dependencies: (a, d), (f, b), (b, d), (f, a), (d, c)
  - output: `f, e, a, b, d, c`

    <details><summary>Hints</summary>

    - #26 - What data structure could you use to represent your dependencies? (consider a directed graph where each node is a project that lists the projects that it is a dependency of)
    - #47 & #60 - Nodes without any incoming edges can be built first. How do you find this node? Where do you go from here?
    - #85 - Once you decide to build a node, its outgoing edge can be deleted. How do you find other/the next node(s)?
    - #125 & #133 - Taking a completely different direction, what would a DFS from a completely arbitrary node give you? What is the last node? What about the nodes before it?

    </details>

    - **Solutions:** [CtCI JS](https://github.com/careercup/CtCI-6th-Edition-JavaScript/blob/master/chapter04/4.07%20-%20Build%20Order/buildOrder.js) | [CtCI ES2015](https://github.com/careercup/CtCI-6th-Edition-JavaScript-ES2015/blob/master/src/chapter4/ch4-q07.js)
    - **Gists:** N/A

  </details>

#### MOB

- Merge K Sorted Lists ([LeetCode](https://leetcode.com/problems/merge-k-sorted-lists/))
- 17.12 BiNode ([LeetCode](https://leetcode.com/problems/flatten-binary-tree-to-linked-list/))

</details>

### Week 4: Bit Manipulation / Math and Logic Puzzles

<details>

#### Notes From Chapters

- Review bit logic `& | ^ >> << ~`
- Sieve of Erastosthenes (for generating a list of primes)
- Probability
- Independence !== Mutual Exclusivity

#### REACTOS

- **5.6 Conversion**

- **5.8 Draw Line**

- **6.10 Poison**

#### MOB

- 16.5 Factorial Zeros
- 16.7 Number Max

</details>

### Week 5: Object Oriented Design / Databases

<details>

#### Notes on Chapter

Most of this week will be theoretical/discussion-based.

- When handling Object Oriented Design questions, ask who is using it and how
- Define core objects in the system
- Analyze the relationships in your system
- What actions can be taken (methods)
- Design Patterns
  - Singleton Class - can only have one instance of a class
  - Factory Method - create many instances from a template/class

#### REACTOS

- **7.1 Deck of Cards**
- **7.10 Minesweeper**
- **14.1 - 14.5 SQL Practice & Normalization**

#### MOB

- 7.4 Parking Lot
- 14.7 Design Grade Database

</details>

### Week 6: Recursion and Dynamic Programming

### Week 7: System Design and Scalability

<details>
Most of this week will be theoretical/discussion-based.

#### Notes From Chapter

Consider taking some time this week to read the chapter. It will be lengthy, but given the minimal exposure we've had to the topic, should be good for at least providing a foundation for being able to speak on the it should it ever come up.

**Additional Resources**

- Grokking the System Design Interview

#### REACTOS

Pick 2 this week

- **7.7 Chat Server**
- **9.1 Stock Data**
- **9.5 Cache**
- **9.6 Sales Rank**

#### MOB

- **9.2 Social Network**
- **9.7 Personal Finance Manager**

</details>

### Week 8: Sorting and Searching
