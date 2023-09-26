# Software Defects Identification: Results Using Machine Learning and Explainable Artificial Intelligence Techniques 


The datasets is used in our empirical studies and evaluation. We identify 3026 bug fixing based on Pull Requests(PRs) in Github. Each bug fixing is treated as a record in the datasets. 

# Dataset
We calculate 21 static metrics for the total 6052 instances in GHPR dataset, which is the data used for the each approaches. All metrics were calculated by the open-source tool [mauricioaniche/ck](https://github.com/mauricioaniche/ck). The description of the metrics as fellow.
| Feature              | Description                                                                                                                                          |
|----------------------|------------------------------------------------------------------------------------------------------------------------------------------------------|
| CBO                  | Coupling between objects\. Counts the number of dependencies a class has\.                                                                           |
| WMC                  | Weight Method Class or McCabe's complexity\. It counts the number of branch instructions in a class\.                                                |
| DIT                  | Depth Inheritance Tree\. It counts the number of "fathers" a class has\. All classes have DIT at least 1 \(everyone inherits java\.lang\.Object\)\.  |
| rfc                  | Response for a Class\. Counts the number of unique method invocations in a class\.                                                                   |
| lcom                 | Lack of Cohesion of Methods\. Calculates LCOM metric\.                                                                                               |
| totalMethods         | Counts the number of methods\.                                                                                                                       |
| totalFields          | Counts the number of fields\.                                                                                                                        |
| NOSI                 | Number of static invocations\. Counts the number of invocations to static methods\.                                                                  |
| LOC                  | Lines of code\. It counts the lines of count, ignoring empty lines\.                                                                                 |
| returnQty            | Quantity of returns\. The number of return instructions\.                                                                                            |
| loopQty              | Quantity of loops\. The number of loops \(i\.e\., for, while, do while, enhanced for\)\.                                                             |
| comparisonsQty       | Quantity of comparisons\. The number of comparisons \(i\.e\., == and \!=\)\.                                                                         |
| tryCatchQty          | Quantity of try/catches\. The number of try/catches\.                                                                                                |
| parenthesizedExpsQty | Quantity of parenthesized expressions\. The number of expressions inside parenthesis\.                                                               |
| stringLiteralsQty    | String literals\. The number of string literals \(e\.g\., "John Doe"\)\.                                                                             |
| numbersQty           | Quantity of Number\. The number of numbers \(i\.e\., int, long, double, float\) literals\.                                                           |
| assignmentsQty       | Quantity of Variables\. Number of declared variables\.                                                                                               |
| mathOperationsQty    | Quantity of Math Operations: The number of math operations \(times, divide, remainder, plus, minus, left shit, right shift\)\.                       |
| variablesQty         | Quantity of Variables\. Number of declared variables\.                                                                                               |
| maxNestedBlocks      | Max nested blocks\. The highest number of blocks nested together\.                                                                                   |
| uniqueWordsQty       | Number of unique words\. Number of unique words in the source code\.                                                                                 |

