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

1. The constants matter but they dont appear in asymptotic analysis
2. Machines can have different specs to them which changes runtime
3. Asymptotic Analysis ignores smaller input sizes so if your program
   is expected to use more of these, asymptotic complexity is not always
   a good guess for the runtime

I would guess 10 seconds; as the worst case scenerio for binary search is O(log(n)) and the best case is O(1). 
Therefore, the runtime has to fall inbetween these two values. Since we know that 1000 elements took 5 
seconds to run, it has to lie inbetween 5 seconds and log(10000) because more elements will not make the program
run faster. Since log(10000) is 14 I would guess 10.

Asyptotic complexity is not the only thing that impacts how fast a program runs, here are a few things that could increase runtime:
1. The actual complexity of a search is not log(n) but rather this is the function
   that impacts the growth the most, so other constants will impact the actual time.
   Therefore, my guess could be off because I dont know these other values so even
   though that impact both tests, the guess could be completely wrong without them.
2. Programming language could increase runtime as it takes a computer a completely
   different amount of time to complie ceratin programs and this cannot be taken
   into account when talking about specifically asymptotic complexity. Therefore,
   the guess could be off since this was not taken into consideration.
3. Machine components impact runtime as well, so once again asymptoitic analysis
   cannot accruately take this into account. Therefore, my guess would be off since
   I only used asympotic complexity to analze it.



