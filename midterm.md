# CMPSC 201 Midterm Exam
## Your Name

1. [10 points] What makes a programming language successful (name at least five factors)? Then, give an example of a specific language and outline which of of these factors make this particular language successful. 

2. [10 points] Give a regular expression for the following string. You may only use the basic operations of concatenation, choice (|), and repetition (∗), plus the simple extensions ? and +, and character sets if appropriate.
```
All strings of 0's and 1's that have at least one character and start and end with the same character. 
Note that the strings 0 and 1 by themselves are in this set, as well as longer strings
of 0's and 1's that have the same character at the beginning and at the end.
```

3. [8 points] For the regular expression `(oink)*oink*` give an example of two strings that can be generated by this regular expression and two that use the same alphabet but cannot be generated.

4. [5 points] (**True or False**): Assume `num = 10`. If we re-assign `num` using the statement `num = 30`, then `num`'s original value "10" represents "garbage" and must be "collected". Explain your answer.

5. [12 points]
Given the following grammar (start symbol `S`, terminal symbols `a`, `+`, and `*`):

  `S -> S + E | E`

  `E -> E * a | a`

Draw a parse tree or write out the derivation for the string `a * a + a * a` or explain why no such tree can be constructed.


6. [12 points] Consider the following grammar, where `num` and `var` are terminals and `S` is a non-terminal and the start symbol. Show that this grammar is ambiguous or argue why it is not ambiguous.

  ```
  S -> num | S var S
  ```

7. [12 points] Given the following grammar, use the shift-reduce algorithm to parse the input string `num + num + num` or demonstrate that this is not possible. Show all of your steps.

```
S' -> S
S -> S + E | E
E -> num
```

8. [9 points] For the following language features, specify its binding time.

  - Keywords (for example, `class` in Java)


  - Meaning of operators (for example, - (subtract))


  - Storage allocation method for a variable


9. [12 points]
Answer two questions about the following Java program; use the line numbers to identify particular statements or variables. Assume that `Widget` is a valid class defined in some other file.

   <img src="https://github.com/allegheny-computer-science-201-f2020/midterm-review/blob/main/images/widget.png" width="500" height="500">
 
 - On line 5, is stack or heap allocation is performed? Justify your answer.
 
- Suppose method `func2` calls method `func1`. What variables are stored in `func1`'s stack frame?

- Suppose method `func2` calls method `func1`. What variables are stored in `func2`'s stack frame?


10. [10 points] Assume the following JavaScript program.

```
1. var num = 1;

2. function func1() {
3.     num = num + 1;
4. }

5. function func2() {
6.    var num = 3;
7. }

8. func1();
9. func2();
10. console.log(num);
```


  - What is the output of the program? 
  
  - What are the scopes of `num` in `func1`, `func2`, and on line 10?


