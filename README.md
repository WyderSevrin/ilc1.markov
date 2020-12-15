# TP 4A 2020-21: Text generator with Markov's chains

## Questions
1. Fork this github repository  (2 points)
2. Run the project
3. Comment the 3 classes: MarkovApp, MarkovChain & MarkovData (3 points)
4. Commit your changes and check-it into github
5. On github, make a pull request (1 point)
6. Complete the next section: "Analyze IADT functions" into this file (2 points)
7. Commit your changes (commit README.md)
8. On github, update your pull request (1 point)
9. Make tests defined into section: "Functions to test now" (call your test functions using the rule: GIVEN_WHEN_THEN) (10 points)
10. Check the test coverage with the Jacoco coverage report provided into: /target/site/jacoco/index.html
11. Commit your changes
12. On github, update your pull request (1 point)
13. that ends

## Analyze IADT functions
Hereafter, for each classes give function to be tested. Remember that all functions does not have to be tested, some code can be checked by a simple inspection or an analyse, another code can be validated by definition (rules, etc) the others function can be tecsted by unit tests, integration tests or validation tests (IADT: Inspect, Analyse, Define, Test). 

### Class app.MarkovApp

| Function      |     I A D T     |        Comment |
| :------------ | :-------------: | :------------- |
| main |  | x | 
| readFileAsString |  | x | 

### Class markov.MarkovChain

| Function      |     I A D T     |        Comment |
| :------------ | :-------------: | :------------- |
| MarkovChain  |  | x |
| generateMarkov  |  | x |
| learn  |  | x |
| setRgen  |  | x |

### Class markov.MarkovData

| Function      |     I A D T     |        Comment |
| :------------ | :-------------: | :------------- |
| read  |  |x  |
| learnWord  |  | x |
| renforceWord  |  | x |
| Etc.  |  | x |

## Functions to test now

### Class markov.MarkovChain

```Java
public void learn(String text)
public String generateMarkov(int numWords)
```

### Class markov.MarkovData

```Java
public void read(String text)
public boolean renforceWord(String keyString, String wordToLearn)
```

## Tricks & tips

- Start with simple classes (models, libraries, etc) at the end make test into complex classes (classes with multiple relations)
- Never test auto generate code
- Never test creator (its a design problem)
- Use @Test before each testFunction !
- You can test a function than throws an exception with the argument: expected
```Java
@Test(expected=Exception.class)
```

## Documentation and validation set
https://www.dcode.fr/chaine-markov-texte