---
title: "How to Load and Manipulate Astronauts CSV Data in Python Pandas"
date: 2020-04-21T12:45:58-07:00
---

First watch these two videos of the Apollo 11 mission. It's awe inspiring. Also notice the gleam in Buzz Aldrin's eyes, humble but confident.

{{< youtube 3Co8Z8BQgWc >}}

___


{{< youtube NgUYurzK-tM >}}



Pandas stands for “Python Data Analysis Library ”. According to the Wikipedia page, pandas is a software library written for the python programming language for data manipulation and analysis. In particular, it offers data structures and operations for manipulating numerical tables and time series. It is free software released under the three-clause BSD license. The name is derived from the term "panel data", an econometrics term for data sets that include observations over multiple time periods for the same individuals.

In tutorial we will load the "astronauts.csv" into Pandas in Google Colab and perform some data filtering and sorting. Goto Colab, create a new note book and give it a name:

![Google Colab](/img/colab01.jpg)
![Google Colab](/img/colab05.jpg)

Copy and paste these 4 lines of python code into the first cell of your Colab notebook Make sure that you have the exact linebreak as seen below. Now **delete and retype** the two " " of line 2url = . This is because if you keep the original " formatting it will give you error. Execute and run. 

import pandas as pd  
url = "https://www.valuableknowledge.tk/videosforastr1/astrpandas/astronauts.csv"  
df = pd.read_csv(url)  
df.head()

![Google Colab](/img/colab07.jpg)

What these statements say is that import the python pandas library into our notebook with an abbreviation pd. The second line assigns to the variable url the string containing the link the excel file astronauts.csv . The third line uses pandas (pd) to read the astronauts.csv data into a df (data frame) so we can manipulate the data. The fourth line check to see if everything works correctly. df.head() by default will display the first five rows in the data frame. Notice that the indexing starts with row 0. Btw check out Buzz Aldrin. He went to MIT :smiley:! 

Again make sure you delete and retype the two " " in line 2 url = ... Otherwise the original formatting will give you an error like this:

![Google Colab](/img/colab08.jpg)

Once you load the data into your notebook with pandas you can sort and filter the date like Microsoft Excel or Google Sheet and a lot more. Think of pandas as Excel or Sheet on steroid! 

For this lab: 
1) Watch the 3 videos I posted in Canvas starting with "1 - Pandas Intro". 
2) **Repeate all of the step** in the 3 videos except for the first step in the first cell. We just did that here. You can also skip the next two steps about using delimiter or typing df to get the whole thing. This is because these two steps are redundant.
3) Answer the math question and a few other below in your notebook.
4) Create a shareable link to your notebook. Make sure it is public, and submit that link to Canvas.

![Google Colab](/img/colab04.jpg)

Make sure to save your notebook regularly. Here is an example of the next two steps you should have in your notebook. Notice I used Canva to draw the arrow and text:

![Google Colab](/img/colab10.jpg)

Math question (2 points): If the Apollo 11 has a speed of 25,000 mph (miles per hour) how long does it take to get to the Moon. Give your answer in day and hour format. Show your calculation in your Colab notebook.