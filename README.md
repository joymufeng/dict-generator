Dict Generator
---------------------------------------------------
## Introduction
---------------------------------------------------
A method of generating all char sequences according to a list of chars, which is based on the simulation of n-ary's mathematical manipulation.For example, for char list:
```scala
  List('a', 'b', 'c')
```
While set maxWordLength=2, it will generate the following char sequences,
```scala
  List("a", "b", "c", "ba", "bb", "bc", "ca", "cb", "cc")
```
Because this method treats the first char 'a' as minimal value, you can imagine it as 0 in decimal number, so aa equals to a. That means, if you set maxWordLength=2, for the char sequences whose length less than 2, you should manually add the additional char sequence that is prefixed with one or more 'a'. According to above example, you should manually add the following additional char sequences:
```scala
  List("aa", "ab", "ac")
```

