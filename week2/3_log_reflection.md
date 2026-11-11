# court verdict:
 1. clean = raw.copy() 
 verdict: keep - original file not modified

 2. clean["price"] = pd.to_numeric(clean["price"], errors="coerce")
 verdict: keep  - data type changed from obj to float
 
 3. clean["date"] = pd.to_datetime(clean["date"], errors="coerce")
 verdict: keep - data type changed from obj to datetime 

 4. print(clean.dtypes)
 verdict: keep - print

 5. print(raw.isna().sum())
    print(clean.isna().sum())
 verdict: keep - print

 6. print(clean[clean["price"].isna()])
 verdict: keep - print

 7. clean["price_missing"] = clean["price"].isna()
 verdict: modify - creates a new row that shows total missing values which is not needed

 8. print(clean["price_missing"].sum())
 verdict: keep - shows total missing values 


# check:
 Was any valid observation removed? No
 Were any labels or numbers changed without your knowing? No
 After cleaning, does every item appear the same number of times you expect? No, missing prices increased by 1

# reflection
 Almost all of my decisions were the same as the one suggested by AI, except 7. which in my opinion is a unnecessary addition which will not serve any purpose, as we can find out the total missing values using code directly.

# log rows 
Date and task: 11/12 , clean code 
Prompt or excerpt: "Described my file (6 columns: date, item, city, price, unit, data label) and the problems I found; asked for cleaning code that works on a copy."
How you verified it: Compared it to the clean code we wrote in class
Accepted / modified / rejected: Accepted
Reason: seemed accurate according to what we learnt in class
What could have gone wrong if I had not checked: errors="coerce" could have changed the data without me knowing 