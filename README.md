# MiniKeys2
![Serie1 coins](https://user-images.githubusercontent.com/82582647/185912181-afcef4e1-2c4b-4be1-be52-1e5d5a14511c.png)

This is the fastest program to find old Serie1 minikeys in the world :trophy:

## :zap: Quick start

For RTX 2070, 2080</br>
Run: ```MiniKeys2-20xx.exe -bits 24 -a addresses.txt -d 0```</br>

For RTX 3060, 3070, 3080</br>
Run: ```MiniKeys2-30xx.exe -bits 24 -a addresses.txt -d 0```</br>

For RTX 3090, A100, A5000, A6000</br>
Run: ```MiniKeys2-30xx.exe -bits 25 -a addresses.txt -d 0```

[**To RUN Linux, Ubuntu**](https://github.com/phrutis/MiniKeys2/tree/main/Linux)
<hr>

### :hammer_and_wrench: Extra options

-d ? - Card number id</br>
-a ? - Name of BTC address database 1.., 3.., bc... on a new line</br>
-id ? - Telegram bot chat number id</br>
-bot ? - BOT Token (create your bot)</br>
-test Checking the operation of FOUND and sending a message to you in telegram</br>

Addresses for the test:</br>
1Cdr4SMTmm4ViY5nZdrygJ2xAJ1qVi41oM</br>
1NiNKjngcQBnCyw9VZZMa6cW2ngku6KM7G</br>
3E8VWzznxTpesgXoAT24wxsD4fUgHJeSNd</br>
bc1qackhakrjwspscnmsdl93ayrxt52plug8ffjjep</br>

To test, add one of these address (or all) to the database</br>
Run a quick test (18 bits):</br>
```MiniKeys2-20xx.exe -bits 18 -a addresses.txt -id 123456789 -bot 1122334455:ABG5X3XU0upZQ8ELkR-EYR9C4OfBEVHBFKQ -d 0 -test```</br></br>
![test-bot](https://user-images.githubusercontent.com/82582647/185806061-4c7d3471-98d6-4a61-ae9c-83e6c96936c8.png)

| Minikeys2 GPU Speed |
|---------------------------|

| GPU card   | -bits    | Speed    |
|------------|----------|----------|
| A100       | 26       | 11 Gkeys |
| A6000      | 26       | 10 Gkeys |
| 3090       | 25       | 10 Gkeys |
| 3080 Ti    | 24       | 10 Gkeys |
| 3080       | 24       | 8.5 Gkeys |
| 3070 Ti    | 24       | ? Gkeys  |
| 3070       | 24       | 7 Gkeys  |
| 3060       | 24       | ? Gkeys  |
| 2080 Ti    | 24       | 5 Gkeys  |
| 2080 S     | 24       | ? Gkeys  |
| 2070       | 24       | 2 Gkeys  |

## :flying_saucer: Special version 1.1 
For rigs with a lot of cards and little RAM (8 GB)</br>
One GPU consumes only 480 MB of RAM</br>
:warning: The program only supports old addresses 1..</br>
Everything else is the same as in the standard program v1.0</br>

For RTX 2070, 2080</br>
Run: ```M20xx.exe -bits 23 -a addresses.txt -d 0```</br>

For RTX 3060, 3070, 3080</br>
Run: ```M30xx.exe -bits 23 -a addresses.txt -d 0```</br>

For RTX 3090, A100, A5000, A6000</br>
Run: ```M30xx.exe -bits 25 -a addresses.txt -d 0```</br></br>
Run a quick test:</br>
```M30xx.exe -bits 18 -a addresses.txt -d 0 -test```</br></br>
![v1.1](https://user-images.githubusercontent.com/82582647/185807241-0a4b8a62-fb24-47f8-bf31-4d97ad8789e9.png)

## :coin: Minikeys Serie1

Number of minikeys Serie1 = 4907</br> 
Denomination of coins 1, 5, 10, 25, 500, 1000 BTC</br>

In 2011-2012 bitcoin was worth cents.</br>
The coins did not provide crypto value.</br>
Beautiful physical coins were used as souvenirs, given as gifts, lost, thrown away.</br>
Many people simply did not know that there was a mini-key under the holagram.</br>
Suppose the person knew about the key</br>
2011 year 1 btc = $0.08</br>
Where can I spend $0.08?</br>

2012 year 1 btc = $1</br>
In 2013 you can buy pizza :)</br>
Then the rate began to rise.</br>

According to the [**analysis**](https://casascius.uberbills.com) of discoveries, you can see that coins began to be opened until 2017.</br>
When in 2021 the bitcoin rate peaked at 1 btc = $60,000, there were no coins discovered?</br>
This suggests one thing, all possible (available) coins have already been discovered previously.</br>

After 2017, there were only 6 coins discovered!</br>
31.12.2020 and 31.12.2021 [**6 coins were opened**](https://casascius.uberbills.com/?status=opened), of which 3 coins are Serie1 and 3 coins Serie2</br>
Based on these assumptions, we can conclude that 95% (out of 4907) Serie1 coins are losses.</br>
5% are possibly used as collectibles.</br>

There are 22 minikey combinations in total</br>
S + 21 (base58 characters)</br>
Total:</br>
10,764,351,351,569,111,513,009,094,806,216,900,608 combinations.</br>

## :hammer_and_wrench: TURBO+

RTX 3090 Speed = 180,000,000/s</br>
By checking the [validity of keys](https://en.bitcoin.it/wiki/Mini_private_key_format), speed increased to 10,000,000,000/s</br>

When analyzing public minikeys ([see gallery](https://github.com/phrutis/MiniKeys2/issues/1)), as well as generating in the original minikey generator
was defined:

In minikeys (as well as in words) there are no 3 identical letters in a row.</br>
A valid random almost does not give 3 (4, 5, 6) identical letters in a row.

Based on this statement, the TURBO+ algorithm was created, which eliminates 3 (4, 5, 6) identical letters in a row.

Clearly not a valid key:</br>
SSSa58hDA3kpvFQuubBc8Wn</br>
Anything after SSS is not valid range</br>
We exclude the range after.</br>
SSS~~1111111111111111111~~ -> SSS~~zzzzzzzzzzzzzzzzzz~~</br>

Total combinations:</br>
10,764,351,351,569,111,513,009,094,806,216,900,608

The TURBO+ algorithm is subtracted from the total:</br>
SSS.....</br>
-3,199,866,632,452,173,458,088,315,935,260,672</br>
SSs.....</br>
-3,199,866,632,452,173,458,088,315,935,260,672</br>
SsS.....</br>
-3,199,866,632,452,173,458,088,315,935,260,672</br>
Sss.....</br>
-3,199,866,632,452,173,458,088,315,935,260,672</br>

SAAA...</br>
-55,170,114,352,623,680,311,867,516,125,184</br>
SAAa...</br>
-55,170,114,352,623,680,311,867,516,125,184</br>
SAaa...</br>
-55,170,114,352,623,680,311,867,516,125,184</br>
SaaA...</br>
-55,170,114,352,623,680,311,867,516,125,184</br>
SaAa...</br>
-55,170,114,352,623,680,311,867,516,125,184</br>
SAaA...</br>
-55,170,114,352,623,680,311,867,516,125,184</br>
Saaa...</br>
-55,170,114,352,623,680,311,867,516,125,184</br>

Sxaaa.., ScvxXx..., SktbEeE... SDai5WmgdEq5bbB... etc.</br>
In total, more than 220+ variations of replacement combinations along the entire length.

Outcome.</br>
Tatal S + 21 symbols (without turbo):</br>
10,764,351,351,569,111,513,009,094,806,216,900,608

Total S + 21 symbols (TURBO+)</br>
51,281,569,183,509,134,909,325,127,825*

*Approximately (did not count)</br>
Less total - more chances.</br>
There are a lot of combinations, you just need to hope for luck.

The TURBO+ algorithm not only eliminates 3 identical letters, but also replaces "+" with the next letter.</br>
SGayRrR... -> SGayRrT...</br>
SavkTdEee... -> SavkTdEef...</br>

## :rocket: + FULL Random

Minikey S...... -> sha256 = random private key!</br>
Each private key output from sha256 is unique. It is 100% random and valid.</br>

By this, you can find any address 1, 3, bc from the database !!!</br>
Even if the address was generated randomly in bitcoin core.</br> 
It's just that the private key corresponds to the minikey's private key.</br>
This is a feature of the bitcoin algorithm.</br>

## :rocket: + SPEED x2
The program works in two modes Uncompressed + Compressed</br>
RTX 3090 Speed = 180,000,000 valid minikeys (random private keys) per second</br>
Since we are searching in two modes at once, this is 180,000,000 x2 = 360,000,000 addresses per second.</br>
There is also a great chance to find an address collision.</br>
Example</br>
The private key: 
5cdd2f650aa61749a0c0d101bc80c454877ead2b6671654cc9bc99633120704e</br>
UNCOMPRESSED address 1Deho8FnoB6veE5Zq7KcEDmUHoaSm1mVyA</br>

The private key: f418546ef63340cd426083f3d0ddfa48421db5717fa8c97201cc3d4e92507b98</br>
can match COMPRESSED address 1Deho8FnoB6veE5Zq7KcEDmUHoaSm1mVyA</br>

## :rocket: + Collision hex160 x2
Possible collision hex160 (rimpd160)</br>
Since the range of hashes160 is 160 bits, and private keys are 256 bits.</br>

One address from the database (hash160) =</br> 
79,228,162,514,264,337,593,543,950,336 private keys in 256 bits range compressed mode.</br>
+79.228.162.514.264.337.593.543.950.336 uncompressed mode.</br>

We get a total of 158,456,325,028,528,675,187,087,900,672 private keys that correspond to one address in range 256 bits.</br>
There are more than 17,000,000+ addresses in the database.</br>

**This is all in theory, in practice these are very large ranges, you only need to hope for luck.**


## :memo: Frequently Asked Questions<hr>
Where to download the program, how to run it:grey_question:</br>

[**HERE**](https://github.com/phrutis/MiniKeys2/releases/tag/1.0)<hr>

Where can I download the database of OLD BTC addresses 1...:grey_question:</br>

[**HERE**](https://github.com/phrutis/MiniKeys2/releases/tag/1.0)<hr>

Where to download 4907 addresses of coins series1:grey_question:</br>

[**HERE**](https://github.com/phrutis/MiniKeys2/blob/main/Others/serie1.txt)<hr>

How many physical coins were issued and which ones:grey_question:</br>

61,560 coins. List of all addresses from coins and other information [**HERE**](https://raw.githubusercontent.com/phrutis/MiniKeys2/main/Others/Fullist.txt)<hr> 

Does the program require an internet connection:grey_question:</br>
If you use a telegram bot - Yes</br>
If you just search, you don't need internet.<hr>

I launched the program hung (froze) what should I do:grey_question:</br>

The program needs time to create the table.</br>
Wait for start:</br>
For 23 bits = 20 minutes</br>
For 24 bits = 25 minutes</br>
For 25 bits = 35 minutes</br>
For 26 bits = 45 minutes<hr>

If I find the private key can I take all the coins for myself:grey_question:</br>

No, you will find the encrypted key.</br>
Only the organizers  can decrypt this key and pay you a 50%.<hr>

I have a RTX 3060 TI card, and I have a low speed, how can speed up:grey_question:</br>

In the new drivers for 30xx Ti, 20xx Ti, a limiter is installed that slows down the speed by half.</br>
You need to download the old driver from six months ago. 496.13</br>
Delete the new driver, install the old driver, the speed will increase x2</br>
After searching, you can install new drivers.<hr>

I have many GPUs. How to start:grey_question:

Run each GPU separately. Add your card id -d ?</br>
Run: ```MiniKeys2-30xx.exe -bits 24 -a addresses.txt -d 0```</br>
Run: ```MiniKeys2-30xx.exe -bits 24 -a addresses.txt -d 1```</br>
Run: ```MiniKeys2-30xx.exe -bits 24 -a addresses.txt -d 2```</br>
Run: ```MiniKeys2-30xx.exe -bits 24 -a addresses.txt -d 3```</br>
Run: ```MiniKeys2-30xx.exe -bits 24 -a addresses.txt -d 4```</br></br>
To run one gpu in ```MiniKeys2``` you need 4-6 GB of RAM!</br>
If you are low on RAM, use the ```M30xx``` program.</br>
It only needs 500 MB of RAM to run.<hr>

Why didn't you do a Serie2 30 character minikey search:grey_question:</br>

These are new coins (2013)</br>
Very large search range.</br>
Many coins are nominal, the amounts are small.</br>
They can also be found in random.<hr>

How to find out that the program has found the key:grey_question:</br>

A message about the find will appear in the program window.</br>
The program will also write the address and key to the text file FOUND.txt</br>
If a telegram bot is connected, it will send you a message.<hr>

How to create a bot and get id:grey_question:</br>

Find information on the Internet.<hr>

Why did the program open the browser:grey_question:</br>

Sending API telegram bot requests goes only through the browser.<hr>

What is the chance to find:grey_question:</br>

Just like winning the lottery.<hr>

Is this theft:grey_question:

This is a very controversial issue!</br>
Almost all coins are lost.</br>
Coins (Serie1) are 12 years old, with a high rate of bitcoin, they were not used.</br>
Or do you think that the owner of the coin is waiting for the rate to fall at all?</br>
If you find a gold coin on the beach (in a landfill)?</br>
Is this theft or a find?</br>
After all, the found coin has (was) an owner, you didn’t physically steal it.</br>
It's just that the lost coin has a new owner.</br>
As the unspoken rule of bitcoin says:</br>
Whoever has the private key is the owner.</br>
Try to find it first :-)<hr>

If I find a large amount (more than 1 btc), what are the guarantees that I will receive my 50%:grey_question:

At the moment there is no way to give you a guarantee.</br>
Suggest your way.</br>
The payment is based on trust.</br>
If the amount is large and there is no trust, you can fly to Belarus Minsk and meet in person.</br>
Import and send coins will be in your presence at the hotel.<hr>

I didn't find the answer to my question:grey_exclamation:</br>

Write your question [**HERE**](https://github.com/phrutis/MiniKeys2/issues)<hr>

### Disclaimer
PROGRAM AND INFORMATION ARE FOR EDUCATIONAL PURPOSES ONLY. USE IT AT YOUR OWN RISK. THE DEVELOPER WILL NOT BE RESPONSIBLE FOR ANY LOSS, DAMAGE OR CLAIM ARISING FROM USING THIS PROGRAM
