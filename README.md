# DNA-PATTERN-MATCHER
A small implementation of Longest Common Subsequence algorithm to find matches in two DNA or RNA samples

## What is Longest Common Subsequence(LCS)?
Following is detailed algorithm to print the LCS. It uses the same 2D table L[][].<br>

1) Construct L[m+1][n+1] .<br>

2) The value L[m][n] contains length of LCS. Create a character array lcs[] of length equal to the length of lcs plus 1 (one extra to store \0).<br>

2) Traverse the 2D array starting from L[m][n]. Do following for every cell L[i][j]<br>
…..a) If characters (in X and Y) corresponding to L[i][j] are same (Or X[i-1] == Y[j-1]), then include this character as part of LCS.<br>
…..b) Else compare values of L[i-1][j] and L[i][j-1] and go in direction of greater value.<br>

## Working:
If samples are not already present in the system, then the randomwordgenerator() generates a sequence of words that may resemble DNA sequence. <br>

According to the computation power, one may chose the length of the DNA sequence to be generated. <br>

On running through the length of the files containing the DNA sequences, it finds the Longest Common Subsequence and according to the given threshold, checks if there is any match between the two DNA samples. <br>



