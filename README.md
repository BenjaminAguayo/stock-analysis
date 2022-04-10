# Module 2 Challenge: Stock Analysis
# **1. Overview of the project**
The purpose of this project is refactor a previous code to offer an **optimized code solution** in order to analyze the entire stock market over the last few years. Steve's parents will be able to make informed decisions once they have the summarized information.

# 2. Results
### 2.1 Data Analysis

>***Picture 1.*** *2017 All stocks analysis*

![Captura de Pantalla 2022-04-09 a la(s) 22 16 45](https://user-images.githubusercontent.com/102047412/162599853-9c837509-392c-4756-9eeb-6a22818875ec.png)

>***Picture 2.*** *2018 All stocks analysis*

![Captura de Pantalla 2022-04-09 a la(s) 22 17 51](https://user-images.githubusercontent.com/102047412/162599895-bcaa6e56-6a34-4d20-a8c0-0510b26b3074.png)

### 2.2 Coding Analysis

*Picture 3* shows the piece of code used in the "green_stocks" file.

- Array is only used for storing the tickers name.
- The total volume is calculated and printed along with the return value after after each data loop.
- Switch between worksheets every loop.
- Processing time is 1.094 *(See Picture 4)*

>***Picture 3.*** *Piece of AllStocksAnalysis macro.*

![Captura de Pantalla 2022-04-09 a la(s) 21 43 21](https://user-images.githubusercontent.com/102047412/162599161-ef70b0ef-4ff2-4751-a045-651b201fc20d.png)


>***Picture 4.*** *Processing time without refactoring.*

![Captura de Pantalla 2022-04-09 a la(s) 22 06 29](https://user-images.githubusercontent.com/102047412/162599551-75c2d809-c0e1-4d11-a65a-de32b2b7bed5.png)


In contrast, in *Picture 5* is shown how the code uses arrays for all variables to calculate and store the information before printing the outputs just once.

  - Uses four different arrays to perform analysis
  - Calculations and storing is done prior to print the outputs.
  - Aditional loop to print outputs, switch between worksheets once.
  - Processing time is 0.961 *(See Picture 5)*


>***Picture 5.*** *Piece of code of Refactored AllStocks Analysis macro.*

![Captura de Pantalla 2022-04-09 a la(s) 23 05 39](https://user-images.githubusercontent.com/102047412/162601016-2d4441c7-1039-434b-ad6c-9786b854176e.png)


>***Picture 6.*** *Processing time with a refactored code.*

![Captura de Pantalla 2022-04-09 a la(s) 22 08 21](https://user-images.githubusercontent.com/102047412/162599605-a2096561-69b5-42b7-931d-d774554edfd3.png)


# 3. Summary

1. According to results described in *Picture 1* and *Picture 2*, we can suggest Steve's parents that the most interesting **stock tickers are ENPH and RUN**, because last two years managed to close with a positive return number, in contrast with all other stocks. This might change next years, however is a good start to learn more about this companies in order to make a good decision.

2. On the other hand, refactoring the code allows to perform analysis of thousands of stocks tickers and reducing time significantly. The difference is very clear as is shown in *Picture 4* and *Picture 6*.
***Time is reduced in 16% thanks to the use of arrays and switching worksheets only once, in the refactored code.***

3. Maybe a disadvantage of refactoring is that an aditional effort needs to be done in order to acknowledge the need for optimizing the code performance. The array item needs to be taken in account to succeed in refactoring process.
4. Another disadvantage is that an aditional loop is needed in order to print the outputs, but is still faster than the non refactored code.
