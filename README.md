
# Readability

A program that computes the approximate grade level needed to comprehend some text.

## Coleman-Liau index

A number of “readability tests” have been developed over the years that define formulas for computing the reading level of a text. One such readability test is the Coleman-Liau index. The Coleman-Liau index of a text is designed to output that (U.S.) grade level that is needed to understand some text. The formula is

```index = 0.0588 * L - 0.296 * S - 15.8```


where `L` is the average number of letters per 100 words in the text, and `S` is the average number of sentences per 100 words in the text.

## Usage/Examples


```
$ ./readability                                                                                     
Text: One fish. Two fish. Red fish. Blue fish.                                                      
Before Grade 1 
```

```
$ ./readability
Text: Congratulations! Today is your day. You're off to Great Places! You're off and away!
Grade 3
```

```
$ ./readability
Text: Harry Potter was a highly unusual boy in many ways. For one thing, he hated the summer holidays more than any other time of year. For another, he really wanted to do his homework, but was forced to do it in secret, in the dead of the night. And he also happened to be a wizard.
Grade 5
```

```
$ ./readability                                                                                     
Text: When he was nearly thirteen, my brother Jem got his arm badly broken at the elbow. When it hea
led, and Jem's fears of never being able to play football were assuaged, he was seldom self-consciou
s about his injury. His left arm was somewhat shorter than his right; when he stood or walked, the b
ack of his hand was at right angles to his body, his thumb parallel to his thigh.                   
Grade 8  
```

```
$ ./readability
Text: As the average number of letters and words per sentence increases, the Coleman-Liau index gives the text a higher reading level. If you were to take this paragraph, for instance, which has longer words and sentences than either of the prior two examples, the formula would give the text an twelfth-grade reading level.
Grade 12                                                      
```

```
$ ./readability                                                                                     
Text: A large class of computational problems involve the determination of properties of graphs, dig
raphs, integers, arrays of integers, finite families of finite sets, boolean formulas and elements o
f other countable domains.                                                                          
Grade 16+     
```
### Links

For more information about Readability visit: 

---------------------------------
[cs50 course](https://cs50.harvard.edu/x/2023/psets/6/readability/)
---------------------------------------------------------------
