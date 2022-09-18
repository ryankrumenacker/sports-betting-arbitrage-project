# Statistical Arbitrage for Sports Betting Project

<p align="center">
  <img src="https://user-images.githubusercontent.com/113403062/190924275-629eaf18-183c-4781-81a2-fd0337143ba9.jpg" alt="animated"/>
</p>

*Above is an example of what the output Excel file may look like.*

This project was made in March 2022. In this project, I utilize the **Live Sports Odds API** (https://the-odds-api.com/) to find statistical arbitrage opportunities in upcoming sporting events across the world. For sports betting purposes, an arbitrage opportunity is when two books are offering such distinct odds that if a bettor makes a particular bet with one book and another particular bet with another book, they can hedge their bets in such a way that they will be guaranteed to make a profit. 

The **Live Sports Odds API** is a free, open source API that tracks the current odds of essentially any given sporting event that is offered by books across the United States. With data from the API, the program is able to find all possible artbitrage opportunities across the eight nearest upcoming sporting events. Once the program finds these opportunities and makes the necessary calculations for the user to understand the output, it writes all findings to an Excel file for the user to access. This file includes the **ID** and **Sport Key** (both of which are specific metrics to the Live Sports Odds API), along with the **Expected Earnings, Bookmaker, Name, Odds**, and **Amount to Buy** with each book for each respective bet. Each row in the file represents one artbitrage opportunity.

All of the code for this program is included in the **Arbitrage.ipynb** file. Each chunk of code is commented so that the user knows exactly what is happening in each step of the program. Please note that the API does not update instantaneously, and since all books are constantly altering their odds as to eliminate such opportunities for bettors, the program will occasionally output odds that are slightly inaccurate due to the fact that they have already been updated on the book's website. 

The **Books.txt** file contains a list of all of the US bookmakers that are supported by the **Live Sports Odds API** as of 3/17/22 for reference. This information is also on the documentation website for the API listed above.

NOTE: In order to use this project, you will need to acquire an API key from the website linked above. It is entirely free. Once you have done this, add your API key to the **API_KEY.txt** file.
