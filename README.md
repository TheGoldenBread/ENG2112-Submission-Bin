# ENG2112-Submission-Bin :grinning:
## Programming Assignment 1
### Alphabet Soup Problem
<strong>[This takes sentences or words and then alphabetically arranges the letters.]<br></strong>
To solve this problem, I was looking at the Python cheat sheet our professor gave us. There, I found the .join() and .sort() and used them. I first created a function that would take strings, sort them using Python's built-in sorting function, and then join them all together with Python's join function. I was having an issue with capital letters always going first until I got a suggestion from our professor to use the .lower() function to lowercase all letters, and thus, the problem was solved.

### Emoticon Problem :thinking:
<strong>[From a set list of words in a dictionary, if an appropriate word is found, it is replaced by an emoticon :D].<br></strong>
We were tasked with creating a function where it is given a sentence, and if there is an appropriate word found in that sentence from the dictionary, it would replace that with an emoticon. Firstly, I created a dictionary where I just put keywords and faces I could think of. Once I've done that, I put it inside a function, then I used the .splitter() function, which takes the sentence and splits it into words, then it checks if any of those words are in the dictionary, and if they are, they'll get replaced, and lastly, they'll get joined back together as a sentence again.

### Unpacking list problem
A given list "writeyourcodehere" was given and it was split into 3 parts the first containing the first word on the list, last containing the last word, and middle which contained the words that were not in the aformentioned.
