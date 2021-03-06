# Stock Analysis
An analysis of green stocks to determine buying behavior, including the number of purchases and rate of return.

# Overview of Project
This analysis is to help determine the best green stock to recommend based on past performance.

## Results

Below are the stock summaries for various green stocks in 2017 and 2018, along with the execution time for the script.

![VBA_Challenge_2017](https://github.com/TRACIE-F/stock-analysis/blob/main/Resources/VBA_Challenge_2017.png)
![VBA_Challenge_2018](https://github.com/TRACIE-F/stock-analysis/blob/main/Resources/VBA_Challenge_2018.png)

**Daily Volume**
Between 2017 and 2018, there seemed to be a spiked interest in Environmental, Social, and Governance (ESG) investing. As illustrated in the image below, "AY" had a significantly higher total daily volume than any other stock in 2017, but in 2018 there were 5 stocks ("RUN","SEDG","SPWR","TERP","VSLR") that outpaced "AY" in total daily volume.

**Return**
In 2017, the rate of return looks stable to high, ranging from -7.9% up to 202%. In 2018, the rate of return is markedly down for these green stocks, which are ranging from -61.1% up to 97.9%. The two stocks that catch my eye are "RUN" and "ENPH." These two both yielded a return, while every other green stock took a loss. "RUN" was one of many stocks to see a lot of popularity growth from 2017 to 2018, but still maintained gains, while "ENPH" stayed low volume, but had a relatively steady rate of return.

![VBA_Original_2017](https://github.com/TRACIE-F/stock-analysis/blob/main/Resources/VBA_Original_2017.png)
Original Code for 2017: 0.8242188 seconds

*Versus*

Refactored Code for 2017: 0.1210938 seconds

Time saved: 0.703125 seconds

![VBA_Original_2018](https://github.com/TRACIE-F/stock-analysis/blob/main/Resources/VBA_Original_2018.png)
Original Code for 2018: 0.7890625 seconds

*Versus*

Refactored Code for 2018: 0.1015625 seconds

Time saved: 0.6875 seconds

**How did the code change?**

The greatest change from the initial practice code created throughout our modules and the refactored code was the consolidation of multiple macros, as pictured below. Sub DQAnalysis, Sub AllStocksAnalysis, and Sub formatAllStocksAnalysisTable were consolidated into our refactored macro.

![Original_Code_1](https://github.com/TRACIE-F/stock-analysis/blob/main/Resources/VBA_Original_1_to_3_Comparison_2.png)
![Original_Code_2](https://github.com/TRACIE-F/stock-analysis/blob/main/Resources/VBA_Original_1_to_3_Comparison_3.png)
![Original_Code_3](https://github.com/TRACIE-F/stock-analysis/blob/main/Resources/VBA_Original_1_to_3_Comparison_4.png)

Rather than one macro to create the worksheet and table, one to enter data, and one to format the table, I consolidated it into a single macro, Sub AllStocksAnalysisRefactored.

![VBA_Refactored_Macro](https://github.com/TRACIE-F/stock-analysis/blob/main/Resources/VBA_Refactored_Macro.png)


## Summary of Advantage and Disadvantage of VBA Re-factoring

The **advantage** of refactoring code is efficiency. Depending on the volume of the data, slight improvements in efficiency could save significant time in the long run, especially if the code will be used repeatedly for varying data sets.

The main **disadvantage** I see is that for smaller data sets, it might be a waste of time to refactor code to only shave fractions of seconds off the run time. Losing a day of work to make a code run slightly more efficiently for a small data set might not be the most efficient way to work.

When it comes to this specific data set, refactoring the data does not feel advantageous. The small fraction of time did not seem beneficial, but for larger data sets, I would see a benefit.
