# Theory vs. Practice

- List 3 reasons why asymptotic analysis may be misleading with respect to actual performance in practice.

- Suppose finding a particular element in a binary search tree with 1,000
  elements take 5 seconds. Given what you know about the asymptotic complexity
  of search in a binary search tree, how long would you guess finding the same
  element in a search tree with 10,000 elements? Explain your reasoning.

- You measure the time with 10,000 elements and it takes 100 seconds! List 3
  reasons why this could be the case, given that reasoning with the asymptotic
  complexity suggests a different time.

Add your answers to this markdown file.

1. Asymptotic analysis just measures how it grows, not the actual speed. Therefore constants are ignored and those matter in practice.
2. Differences in hardware. For example if an algorithm needs to take a square root, due to how the cpu is designed this could take a constant different amount of time depending on the hardware.
3. The performance will depend on the implementation which asymptotic analysis can't always capture. For example it might be much faster to merge arrays for merge sort in a language like C compared to a language like python or JS.

- The complexity of BST is O(log n). O(log 1,000) = 9.97 and O(log 10,000) = 13.29. That's a percent change of 33.33% longer so I would expect very roughly for the time to be around $5 \cdot (1+0.33) = 6.66$ seconds.

- It could be that the new items were sorted so the tree ended up with a very large height and was not balanced. Meaning that the search time was closer to that of a linked list than a BST.
- The tests could have been run on different machines with different hardware. For example one could have a faster cpu than the other.
- The tests could have been run on the same machine but with different external loads, like maybe in one of the tests an intensive rendering workload or compilation workload is being run.
 
I certify that I have listed all sources used to complete this exercise, including the use of any Large Language Models. All of the work is my own, except where stated otherwise. I am aware that plagiarism carries severe penalties and that if plagiarism is suspected, charges may be filed against me without prior notice.
