[Amount] 
count    100000.000000
mean       2497.092666
std        1442.415999
min           1.050000
25%        1247.955000
50%        2496.500000
75%        3743.592500
max        4999.770000

[MerchantID]
 461    149
 188    134
 192    129
 517    128
 820    126
       ... 
 119     75
 936     74
 968     73
 635     71
 512     69

[IsFraud]
0    99000
1     1000

RangeIndex: 100000 entries, 0 to 99999
Data columns (total 7 columns):
 #   Column           Non-Null Count   Dtype  
---  ------           --------------   -----  
 0   TransactionID    100000 non-null  int64  
 1   TransactionDate  100000 non-null  object 
 2   Amount           100000 non-null  float64
 3   MerchantID       100000 non-null  int64  
 4   TransactionType  100000 non-null  object 
 5   Location         100000 non-null  object 
 6   IsFraud          100000 non-null  int64

[Location]
Chicago         10193
San Diego       10111
Dallas          10076
San Antonio     10062
New York         9993
Houston          9991
Phoenix          9960
Los Angeles      9936
Philadelphia     9873
San Jose         9805
Name: count, dtype: int64

fraud['Location'].value_counts()
New York        116
San Diego       115
Houston         105
Phoenix          99
Dallas           99
San Antonio      99
Chicago          95
Los Angeles      95
Philadelphia     90
San Jose         87

rateOfPurchase = (orgDf['Location'].value_counts()) / 100000
Chicago         0.10193
San Diego       0.10111
Dallas          0.10076
San Antonio     0.10062
New York        0.09993
Houston         0.09991
Phoenix         0.09960
Los Angeles     0.09936
Philadelphia    0.09873
San Jose        0.09805

rateOfFraud = (fraud['Location'].value_counts()) / 1000
New York        0.116
San Diego       0.115
Houston         0.105
Phoenix         0.099
Dallas          0.099
San Antonio     0.099
Chicago         0.095
Los Angeles     0.095
Philadelphia    0.090
San Jose        0.087