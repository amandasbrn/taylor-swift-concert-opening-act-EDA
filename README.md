# Taylor Swift Concert Opening Acts Exploratory Data Analyst

If you have looked at my latest Taylor Swift concert project, this is like the "spin-off" of that project, because if I put it together the project will be 50 hours long *joke*

## Then, what is this project?
I became intrigued to explore the opening acts more thoroughly, particularly because each world tour featured different opening acts. To dive into this, I did an exploratory data analysis (EDA) using a weighted average approach. This involved calculating ticket sales based on the frequency of each opening act's appearances to kick off the show.

## Why I did weighted average?
In the dataset, there is an "Opening Act(s)" column, which consists of opening acts on each show. However, one row could consist of two, even three opening acts, separated by \r\n delimiter (which later I replaced with a comma). Since I want to generate each of the opening acts, I used .explode() method. But, this method creates new rows for each opening act, which also duplicates Revenue, Ticket Available, and Ticket Sold value.

To overcome this, that is why I used a weighted average. Courtesy to Investopedia.com, the weighted average is a calculation that takes into account the varying degrees of importance of the numbers in a data set. By using this approach, I calculated the number of tickets sold for each opening act, taking into consideration the frequency with which they appeared. This enabled a more accurate assessment of their impact on overall ticket sales.

## Result
Each world tour had its own "main character".
1) Fearless Tour: Gloriana with 79 shows
2) Speak Now World Tour: Needtobreathe with 58 shows
3) The 1989 World Tour: Vance Joy with 48 shows
4) Reputation Stadium Tour: Charli XCX with 36 shows
