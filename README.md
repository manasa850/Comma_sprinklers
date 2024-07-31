Input

The input contains one line of text. Each character is either a lowercase letter, a comma, a period, or a space. And: The text begins with a word. Between every two words in the text, there is either a single space, a comma followed by a space, or a period followed by a space (denoting the end of a sentence and the beginning of a new one). The last word of the text is followed by a period with no trailing space.

Example:

Input: please sit spot. sit spot, sit. spot here now here. Output: please, sit spot. sit spot, sit. spot, here now, here.

Rules for adding commas to an existing piece of text are as follows:

1.If a word anywhere in the text is preceded by a comma, find all occurrences of that word in the text, and put a comma before each of those occurrences, except in the case where such an occurrence is the first word of a sentence or already preceded by a comma.

2.If a word anywhere in the text is succeeded by a comma, find all occurrences of that word in the text, and put a comma after each of those occurrences, except in the case where such an occurrence is the last word of a sentence or already succeeded by a comma.

3.Apply rules 1 and 2 repeatedly until no new commas can be added using either of them.
