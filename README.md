# Theory vs. Practice

- List 3 reasons why asymptotic analysis may be misleading with respect to
  actual performance in practice.

- Suppose finding a particular element in a binary search tree with 1,000
  elements takes 5 seconds. Given what you know about the asymptotic complexity
  of search in a binary search tree, how long would you guess finding the same
  element in a search tree with 10,000 elements takes? Explain your reasoning.

- You measure the time with 10,000 elements and it takes 100 seconds! List 3
  reasons why this could be the case, given that reasoning with the asymptotic
  complexity suggests a different time.

Add your answers to this markdown file.

1. Asymptotic analysis just measures how it grows not the actual speed. Therefore constants are ignored and those matter in pratice.
2. It also doesn't consider space, in the real world using more space is expensive both financially and speed wise as data is further and further away physically.
3. The best case and average and worst case might have varying levels of occurance. For example the best case of insertion sort is faster than the best case for quick sort, but the best case for quick sort occurs far more often so on average it is faster.

- The complexity of BST is O(log n) as the input increases by a factor of 10 I'd expect the time to increase by a factor of log 10 which is 3.322. So around 16 seconds roughtly.

- It could be that the new items were sorted so the tree ended up with a very large height and was not balanced. Meaning that the search time was closer to that of a linked list than a BST.
  
I certify that I have listed all sources used to complete this exercise, including the use of any Large Language Models. All of the work is my own, except where stated otherwise. I am aware that plagiarism carries severe penalties and that if plagiarism is suspected, charges may be filed against me without prior notice.
