<strong>How similar are these texts? A Golang implementation.</strong>

I perform a lot of scripting tasks in my line of employment.

I started in Python, then moved to C# (not an ideal language for throwaway code), and a few months ago I finally settled on Go. Go is a brilliant language to implement many complex algorithms (due to ease of implementation and compilation time, in my opinion.), and one I find myself using frequently is the Levenshtein Distance Algorithm (“LDA”).

The Levenshtein Distance “a measure of dissimilarity between two strings”. What this means in human terms, is it is a calculation of how many changes need to be made between two pieces of text to make them the same.

As an example, let’s take the words “kitten” and “sitting”. If I want to determine how different these two words are, I could take word, and determine how many changes need to be made to make these words identical, as below:

K I T T E N<br>
S I T T I N G

To make them identical, I would have to change the first character (K-S), then the next three characters remain the same (ITT), then the fifth character changes (E-I), the sixth stays the same (N), and the seventh needs changing, or rather, adding (null-G).

This algorithm is featured in almost all spellchecks I’ve ever observed. I also use it frequently on larger bodies of text, and it still remains the fastest algorithm for string comparison I’ve encountered, that isn’t a direct comparison between the two. 
