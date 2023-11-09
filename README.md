# SplashPF
Why Splash? Because I spilled my coffee working on Mint replacement... 

## Getting started

When Mint.com decided to shutdown in November 2023 (basically right now as I write), I want something simple and private for my finance data... because break-ins are everywhere at some point, and companies make a lot off my own data. But I couldn't find it with all the startup apps and banks, they instead license your data all over creation as well as your logins in some fashion are stored someplace. Additionally, reading the contractual agreements to several PF apps out there,  you grant power of attorney over to them for your own data.

Ok the fine print got me riled up, I guess. So, 

I'm a simple guy with simple PF (personal finance) needs for charts, and this is basic stuff for Jupyter notebooks and Csv files: 

- Daily or weekly run rate in expenses
- Yearly MoM  expense breakdowns
- two levels of category rollups
- total balances and net worth

## Create my own

This is kind of easy stuff for open source Python Notebooks, so let's give it a try. Using Chatgpt, I  brushed off some of data scientist skills to get this started. 
Now although the first version 1.0 should work for everyone coming from Mint.com who downloaded their transactions into the 'transactions.csv' file, the fact is Mint.com is closing and this file will become your "historical" data, and static.  

In the next versions coming up, I am working on "adapters" for each institution I use, because each institution has a different CSV file format and headers, you need to an "adapter" (just some code) that understands your bank or credit card processor's  CSV format and how to bring it into your format and add it to your history.  I'll show you how you can build your own. For me I use an AMEX card for cashback for some years now, and most of my TXs come through there, so that is my first adapter. 

If this helps anyone get over the bump from Mint.com , then heck... I'll share. 

But it's a geeky solution, not for the light-hearted, but is open source and  gets the job done.

## How it works

The idea is simple here,  you have : 

1. a history of transactions you want to keep ( I have 12 years of Mint.com data in a CSV with over 10k transactions I want to keep)
2. you want to just download CSVs whenever from every credit card or bank, and just chuck them into a folder
3. you don't want to track duplicates at all, but let the app find them and clean up, if say you downloaded the same CSV or transactions that overlap
4. you can use my basic graphics, or have ChatGpt create new ones to your notebook
5. is open source, and free, and totally private to you


## Versions

- Current - Initial version: This is basic POC with my mint data to replicate from the Mint.com transactions.csv download. 

## Coming Next
To fully use this as a rought Mint replacement for how I use it, some key things need added kind of right away:

- consume any number of .csv files  from different institutions
- add more charts

 (I don't use Mint budget much in the past, so that's not top shelf for me yet. )
