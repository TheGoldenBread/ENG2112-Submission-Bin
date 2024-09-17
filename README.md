<h1 align="center">ENG2112-Submission-Bin</h1><br>

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

## Programming Assignment 3
### Problem 1
<strong>[Load the given cars.csv file and display the first and last 5 rows.]<br></strong>
For this problem, I had to load the given cars.csv file through Panda's read function. After that, I used the .head() and .tails() functions; however, it only outputted the last 5 rows. So I tried using print, and the results were unsatisfactory, so I asked ChatGPT what to use, and it said to use the concat function, and lo and behold, it now works.

### Problem 2
<strong>[Load the given cars.csv file and extract the following information.]<br></strong>
#### a. Display the first five rows with odd-numbered columns (columns 1, 3, 5, 7...) of cars.
For this, I had no idea what to do, I tried doing it manually, like getting the location of each column, but it was way too long, so I asked ChatGPT what to do, and it said to use the :: operator paired with a 2 to take every two columns which corresponds to its odd columns.

#### b. Display the row that contains the ‘Model’ of ‘Mazda RX4’.
I just had to display the row containing the model mentioned, so I used the .loc function and specified what label it should look for and what name in that label to find and show its row.

#### c. How many cylinders (‘cyl’) does the car model ‘Camaro Z28’ have?
It has the same principle as the previous one, but instead of showing the whole row, I added a specification to only output the number of cylinders.

#### d. Determine how many cylinders (‘cyl’) and what gear type (‘gear’) do the car models ‘Mazda RX4 Wag’, ‘Ford Pantera L’ and ‘Honda Civic’ have.
This one was hard for me; it was easy to output one of the models with the specified cylinders and gear but to output all 3, I had no idea what to do, so once again, I asked ChatGPT for some advice and it said to me to use the "|" OR operator to combine all the conditions into one, and it works. (I love you ChatGPT ❤️)

## Programming Assignment 4
### ECE Board Exam Problem
<strong>[With the given board2.csv file create the following.]<br></strong>
#### 1. Using the given dataset sent, create the following data frames based on the format provided.
##### a. Filename: Instru = [“Name”, “GEAS”, “Electronics >70”]; where track is constant as Instrumentation and hometown Luzon
So, I first had to take all the necessary elements and put them all into the data set. I took all the columns with the Instrumentation track, the same with Luzon as the hometown. Then, I filtered out all the elements where the grade in Electronics was above 70. After that, I only had to show the needed labels: Name, GEAS, and the filtered-out Electronic scores.

##### b. Filename: Mindy = ["Name", "Track", "Electronics", "Average >=55"]; where hometown is constant as Mindanao and gender Female
I used the same trick as the previous one, but I needed to add to the data set the average of all the scores combined and then filter out that, too. Same process as last time, I only showed the needed labels, which this time were Name, Track, Electronics, and the filtered-out Average.

#### 2. Create a visualization that shows how the different features contributes to average grade. Does chosen track in college, gender, or hometown contributes to a higher average score?
Now this... I kept mulling and looking at the Matplotlib and Seaborn Cheat Sheet. I'm not going to sugarcoat it; I don't get it. So, I completely just copied what ChatGPT said.

# Version History
* v.01
   - Added a lower function on the alphabet soup problem, ensuring capital letters don't go first, and added more test cases with special characters.
   - Added a test case in the emotify problem where a word in the dictionary was typed with mixed cases and could still recognize the word properly and replaced.
   - Scrapped the previous code to add a function (as per suggestion) that checks if the length of the list is more than 3 if not then properly addresses it then still uses previous logic to unpack and show the result. Added test cases to see how it handles more than 3 elements and less than 3 elements.

<br><hr>
[:arrow_up: Back to top](#ENG2112-Submission-Bin)
