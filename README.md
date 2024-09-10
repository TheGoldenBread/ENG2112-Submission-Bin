# ENG2112-Submission-Bin :grinning:
## Programming Assignment 1
### Alphabet Soup Problem
<strong>[This takes sentences or words and then alphabetically arranges the letters.]<br></strong>
To solve this problem, I was looking at the Python cheat sheet our professor gave us. There, I found the .join() and .sort() and used them. I first created a function that would take strings, sort them using Python's built-in sorting function, and then join them all together with Python's join function. I was having an issue with capital letters always going first until I got a suggestion from our professor to use the .lower() function to lowercase all letters, and thus, the problem was solved.

### Emoticon Problem :thinking:
<strong>[From a set list of words in a dictionary, if an appropriate word is found, it is replaced by an emoticon :D].<br></strong>
We were tasked with creating a function where it is given a sentence, and if there is an appropriate word found in that sentence from the dictionary, it would replace that with an emoticon.<br> 
Firstly, I created a dictionary where I just put keywords and faces I could think of. Once I've done that, I put it inside a function, then I used the .splitter() function, which takes the sentence and splits it into words, then it checks if any of those words are in the dictionary, and if they are, they'll get replaced, and lastly, they'll get joined back together as a sentence again.<br>
The problem I had that with this is that when punctuations marks are include in the word it also gets included when it gets split and since it doesn't recognize it from the dictionary it doesn't get replaced. It was suggested that I find a fix for this, but I couldn't, so I gave up.

### Unpacking list problem
<strong>[A given list "writeyourcodehere" was given, and it was split into 3 parts: the first containing the first word on the list, the last containing the last word, and the middle which contained the words that were not in the aforementioned.<br></strong>
We were tasked on unpacking the list writeyourcodehere into 3 different variables being first, middle, last. First having the first element and last having the last element and middle having any in between.<br>
I created the list write your code here. Using Python's unpacking syntax, I put the first element in first, the last element in last, and everything in between in *middle (the asterisk operator gets everything in the middle) and just printed that.

## Programming Assignment 2
### Normalization Problem
<strong>[Normalization is one of the most basic preprocessing techniques in data analytics. Create a random 5x5 array using Numpy and normalize it]<br></strong>
Here we were tasked to create a random 5x5 array and normalize it. Below is the formula for the normalization.
![alt text](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSkf7umgE7G9H2BujLnpmdkDAftT3zt_iH6Qg&s)<br>
Where Z is the normalized data, x is the data, μ being the mean, and σ being the standard deviation.<br>
I first created the random 5x5 array and assigned it to a letter. Then, using NumPy's .std() and .mean() functions, I recreated the formula to get a normalized array and show the results.

### Divisible by 3 Problem
<strong>[Create a 10x10 array containing the first squared 100 positive integers]<br></strong>
I needed to create a 10x10 array containing the squared 100 positive integers. To do that I first had to create a 1d array and squared that. Using NumPy's reshape function, I reshaped it to a 10x10. Then through a modulo, it figured out what elements where divisible by 3 if the remainder returned a 0, then those elements got put into a list and was showed.

# Version History
* v.01
   - Added a lower function on the alphabet soup problem, ensuring capital letters don't go first, and added more test cases with special characters.
   - Added a test case in the emotify problem where a word in the dictionary was typed with mixed cases and could still recognize the word properly and replaced.
   - Scrapped the previous code to add a function (as per suggestion) that checks if the length of the list is more than 3 if not then properly addresses it then still uses previous logic to unpack and show the result. Added test cases to see how it handles more than 3 elements and less than 3 elements.

<br><hr>
[:arrow_up: Back to top](#ENG2112)
