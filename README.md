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
3. If you use an asymptotically better algorithm with smaller input sizes, other algorithms could be better

I would guess 10 seconds as the worst case scenerio for binary search is O(log(n)) and as you add more elements,
it is more likely to approach this bound. Since log(10000) is about 14, I would say something in between these two
values is a good guess.

Asyptotic complexity is not the only thing that impacts how fast a program runs, here are a few things that could increase runtime:
1. The actual complexity of a search is not log(n) but rather this is the function that impacts the growth the most so other constants will impact the actual time
2. Programming language could increase runtime
3. Machine components impact runtime as well


