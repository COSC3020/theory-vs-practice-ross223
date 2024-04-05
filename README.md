[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-24ddc0f5d75046c5622901739e7c5dd533143b0c8e959d652212380cedb1ea36.svg)](https://classroom.github.com/a/FgMJElkj)
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

1. Asymptotic analysis observes the algorithm without considering constant
   factors, so while they impact the runtime, they don't show up in the
   asymptotic analysis.
2. Certain notations like big O aren't closely related to the actual time complexity.
   For instance, most programs have runtime of $O(n!)$ and while this is true,
   it doesn't explain anything about the actual runtime of the program.
3. Asymptotic analysis is only useful for input sizes larger than a
   specific n_0, so runtime for values below this n_0 are not accurately
   depicted by the analysis.

The asympotitic analysis for binary search is O(log(n)). This means for a certain n the runtime
should be about log of that n. So, log(1000) is approximately 9.97 and log(10000) is approximately
13.29. Since we know that running the program with 1000 elements took 5 seconds, that means that 
running the program with 10000 elements should be proportional to the log values. Therefore,
a good guess could be calculated using cross multiplication:

5/9.97 = x/13.29 => x = (5/9.97) * 13.29 => x = 6.66

So a good guess would be 6.66 seconds.

1. The program was run on a different machine than the first one that had worse specs. This would
   impact the guess as the runtime could not be correctly calculated using only asymptotic complexity.
2. The algorithm was made unefficent for data sets. Since I am just assuming that the
   average case for the algorithm is O(log(n)) this would impact the runtime because in reality
   the runtime could be much worse depending on the implementation.
3. There are other programs running on the computer during the test. Programs can slow each other
   down due to necessary computational memory. If other programs were running on the computer,
   different times would be observed because of the unaccounted external runtimes.



