# cbr-scraper
This is my pet project. Currently it is able to get exchange rate info from CBR's (Central bank of Russia) website

By default it scrapes data from the earlisest date to current date 
(though this may be changed via introduction of some changes to exchange_link_generator() function)

This code returns three files:
1) An Excel file with numerical code of a currency, letter code of a currency, currency name (in Russian), units of currency, rate of a ruble, rate of a ruble to one unit of currency
2) A second Excel files with the same data, but also has currency names in Russian in normal form
3) A pdf file with plots of fluctuation of every currency

Libraries used: pandas, tqdm, time, bs4 (BeautifulSoup), requests, matplotlib, datetime, pymorphy3, joblib, pypdf, os, selenium

Approximate runtime - 12-ish hours (if you want to get all the data) or about an hour (if you need data for about a thousand days)

Note: this code doesn't deal with occurence of captchas (fyi)
