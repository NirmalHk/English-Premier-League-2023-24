# English-Premier-League-2023-24
Welcome to my personal project! This will be mainly used to practise data analysis and SQL to generate insights on PL data from the 2023/24 season. My favourite team is Chelsea Football club, even though we've been through a lot, I wouldn't give it up for anything in the world! I'll be playing around with data to answer few interesting problems including how teams fared at home V/s away and also we will finally find out whether Anthony Taylor has an agenda against Chelsea! ( Bald ref famous for this thing btw). There will be more questions answered as the days go on, i'll find new questions to answer as I study the data more.

I got the data from : https://football-data.co.uk/mmz4281/2324/all-euro-data-2023-2024.xlsx
The abbrevations are pretty clear to a football nerd like me but there's a txt file below that should help you out:
https://football-data.co.uk/notes.txt
PS. This has some weird betting data that's not gonna be useful for most people (don't gamble mate.)



 




Firstly, let's take a look at Chelsea football club themselves and see where we lost all the points:



Were CFC better at home or away?



Firstly, let's check out all the CFC home games, if the result is:

 A- Away win = LOSS
 
 H- Home win = WIN , 
 
 D= DRAW

 
 Also let's make things more interesting, points scored will be:  win = 3 pts, Draw= 1pt and Loss = 0 pts.

We can see that there's a clear majority of wins at Stamford Bridge (Home) with 11 W's and 4 a piece for losses and draws. Around 37 points were scored at HOME.

![image](https://github.com/NirmalHk/English-Premier-League-2023-24/assets/97601577/daa81dc4-3dd3-4e47-9362-7109f32aaefb)


Now let's do the same for the Away Chelsea matches, here the logic reverse as "H" counts as a LOSS and "A" counts as a WIN.

![image](https://github.com/NirmalHk/English-Premier-League-2023-24/assets/97601577/3c4080e8-2958-4496-8e2c-69b6ea2d5c5d)

7 Wins and 7 losses, with 5 draws. That's where majority of the points were dropped. Total points from away games = 26 points.

Chelsea Football Club performed better at HOME, compared to AWAY.


Now the question is, is this the case with other teams too? Let's find out!


Let's take a look at the whole league and figure out the best performing teams at home and away. Using the same logic we used above, I extended the query to qualify more teams and made use of CTE's and window functions to give them a ranking to find the top performing home teams.

![image](https://github.com/user-attachments/assets/27f84b77-2601-456a-a5f0-085a607a2574)

Arsenal and Liverpool very impressive, followed closely by Manchester City. Meanwhile the likes of Chelsea and Manchester United are lingering around in 7th and 8th. Talk about fallen giants.

Now let's take a look at the away form and find the best visiting teams!

![image](https://github.com/user-attachments/assets/b897b0fc-a694-4ac7-a7fa-0c6abb23728d)

Manchester City impressive away from home, followed by Arsenal and Liverpool. City clearly the best team in the league and has been for a while.

 
