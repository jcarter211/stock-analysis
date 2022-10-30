# Stock Analysis

## Overview of Project 
Steve recently graduated with a degree in finance. His parents are showing their support of his academics and education by becoming his first clients. They have a special interest in green energy. While Steve's parents wanted to invest all of their money into one company, Steve wanted to research a few more green energy stocks. In order to look at all of the stocks Steve has chosen, we used VBA to perform functions that give us a better understanding of each company. Steve can easily analyze the dataset with the use of the code in VBA. The code we originally built processed the 12 stocks Steve chose to further research; however, we realized that it would not be ideal if we wanted to analyze much larger sets of stock data. In order to make this code more friendly to large data sets, we refactored the code. 

## Results 
There are a few key results after refactoring the original code. The time to run the code to perform an analysis of both the 2017 and 2018 stocks was reduced. 

### 2017 Run Times
<p align="center">
  <img width="400" height="300" src="https://github.com/jcarter211/stock-analysis/blob/main/Resources/Green_Stocks_2017.png">
</p>


* As you can see in the image above, it took .265625 seconds to run the original code for the year 2017. 
<p align="center">
  <img width="400" height="300" src="https://github.com/jcarter211/stock-analysis/blob/main/Resources/VBA_Challenge_2017.png">
</p>

* In the refactored code, the code ran in .0703125 seconds. 

### 2018 Run Times 
<p align="center">
  <img width="400" height="300" src="https://github.com/jcarter211/stock-analysis/blob/main/Resources/Green_Stocks_2018.png">
</p>


* The original 2018 code ran in .265625 seconds, which is the same as the 2017 code. 
<p align="center">
  <img width="400" height="300" src="https://github.com/jcarter211/stock-analysis/blob/main/Resources/VBA_Challenge_2018.png">
</p>

* The refactored run time for 2018 stayed the say as the 2017 refactored run time of .0703125 seconds. 
### Analysis of the 2017 and 2018 Run Times 
While the original and refactored run times are both quick, it is important to note that we are looking at a dataset of 12 stocks. If we were to have 100 stocks, this time difference would help our work and analyzation move forward at the most efficient pace. Trading and buying stocks can be realtively fast-paced in the real-world. We would want the quickest run time possible. 

To refactor the code, there are a few changes we needed to make. Below is an image of the original code used to produce the total return for each ticker. 
<p align="center">
  <img width="600" height="400" src="https://github.com/jcarter211/stock-analysis/blob/main/Resources/Original_Code.png">
</p>
To analyze each stock or ticker in the original code, we found the total volume and the return percentage. To find the return, the code found the starting price and ending price. After finding these two values, we divided the ending price by the starting price and then subtracted 1 to find the percentage. We also color coded the results to more easily identify positive vs. negative return values. 

<p align="center">
  <img width="600" height="400" src="https://github.com/jcarter211/stock-analysis/blob/main/Resources/Refactored_Code.png">
</p>
In the refactored code, we created a ticker index. We then related the ticker volume, starting price, and ending price to the ticker index. This allows the code to be more easily applied to the dataset. 

## Summary 
### Advantages and Disadvantages to Refactoring Code in General 
  * Advantages
    * Refactoring code can make the execution run more quickly as we can see in the example above. 
    * It can also be used to analyze a larger dataset more easily. 
  * Disadvantages 
    * Refactoring code can be difficult. It can produce errors if not written correctly, which does not allow the code to produce the outcome.
    * Refactoring code can be time consuming. Depedning on the task, it may not be worth the additional time. 
### How These Advantages and Disadvantages Related to This Dataset 
  * Advantages 
    * This dataset benefited from both of the advantages listed above. The execution ran more smoothly and can be used to analyze a larger amount of stocks. Steve will be able to apply this code when gaining new clients and for his parents. 
  * Disadvantages 
    * I would say that the two disadvantages listed above also applied to this dataset. It was diddifult thinking through how to refactor the code, and it took time to implement the changes needed. I had to go through trial and error to make sure I used to correct steps and coding statements. 
