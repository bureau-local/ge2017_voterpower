# Voter Power GE2017
*A Bureau Local Investivation*
<br></br>
**Which group of voters can determine the election’s outcome**
<br></br>
### In brief
Ahead of the 2017 General Election, the Bureau Local pulled together a robust database of demographics of the UK electorate and worked with two statisticians to estimate and verify registration figures.

From education to age, to those registered and not, the Bureau Local set out to find who had the power to determine the result in their local constituency and how that reflected national trends.
<br></br>
### Voter Power Hack Day
The Bureau Local organised a hack day so that physical and digital attendees could dig into the data and find and break stories together. This aim resulted in collaborative journalism and a national and local discussion on voter power.

At the hack day everyone had a chance to dig into a vast dataset of variables related to demographics - from income and education levels to past vote, majority and past registration. A model was built ahead of time and used data on England and Wales from the Office of National Statistics, the Cabinet Office and the British Election Study to estimate the number registered voters in each seat - something not available in a central database. 

Throughout the hack day 65 participants in Glasgow, Cardiff, Bournemouth, Birmingham and London each dug into the data in order to find stories for their own communities. Two journalists in London - Matty Edwards and Ed Fairhead - started looking at how our estimated registration numbers compared to the margin in the seats they cover - Croydon Central and Colchester respectively. They found these seats had an increase in new voters larger than the 2015 margin. They also looked at the number of past UKIP voters in Colchester, where the party was no longer standing in 2017. 

The Bureau worked with Edwards and Fairhead and expanded their measures across the country. We found there were 71 seats where the number of 'partyless' voters - newly-registered, or former Green and UKIP voters whose party wasn't standing this time around - was larger than the margin in the last election. In 19 seats this was due to the increase in new voters alone. 


We then rang up local authorities to get actual registration numbers for over 50 constituencies, and in doing do, found that our model was very accurate - it over-estimated registration figures by less than 1% on average. We used exact numbers - not estimates - in our piece.

* **_The Bureau Local’s pre-election assessment:_**
“How new voters could dent Theresa May’s election majority”
https://www.thebureauinvestigates.com/stories/2017-06-06/new-voters-hold-the-power-to-swing-the-election-shows-new-analysis

“The analysis has found 50,000 new voters in 19 seats where the increase in voter registration is greater than the majority won by the victorious candidate in the last election.

Less than 7,000 of these newly-registered voters have the power to swing six key Conservative seats: Derby North, Thurrock, Croydon Central, Twickenham, Plymouth Sutton & Devonport, and Crewe & Nantwich.

If Theresa May loses six seats without winning any new ones, she will no longer have a parliamentary majority.
Three further Tory-controlled seats - Colchester, Telford and Bedford - also have more new voters than the margin…

Both the Green Party and UKIP no longer have candidates standing which adds an additional 3,000 UKIP and nearly 2,500 Green voters to fight for.”

**_At the bottom of this document you will find links to some of the local stories published._**

* **_The Bureau Local’s response to the election result:_**
“How new voter power identified by the Bureau damaged Theresa May”
https://www.thebureauinvestigates.com/stories/2017-06-09/how-new-voter-power-identified-by-the-bureau-damaged-theresa-may

The wins and losses confounded all forecasts by pollsters in the run-up, who looked at voting patterns and intentions to predict a Tory majority of anything from the dozens to more than 100. Instead, they lost 12 seats.

However many of these losses fell in line with modelling carried out by the Bureau’s data journalism team the Bureau Local.

Following our hack day we identified two large groups of voters who had the power to swing 71 constituencies in England and Wales: people registered to vote for the first time, and people who voted UKIP or Green in 2015 whose party was not standing a candidate this time around. And 20 of those constituencies changed hands.

Of those 71 seats, 35 were Conservative, 32 were Labour and four were Lib Dem. The Tories lost 16 of them, the Lib Dems lost two and Labour held on to all but two.

Across the whole of England and Wales, 44 seats changed hands - meaning our modelling identified nearly half of them.
<br></br>
### The Methodology:
There is a lot of data in our database - over 600 variables actually!
Here’s how we obtained the variables:
 
1.	**% vote share for each party in the 2015 and 2010 elections:** We divided the number of votes each party received by the total number of people that voted in that constituency.
1.	**The number of registered voters in 2017:** we derived the number of registered voters in each constituency for the coming elections, using data from several sources and carrying out several procedures:
    1.	We used data from the ONS that reported the exact number of registered voters on the 31st of December 2016 for each constituency.
    1.	We used the number of registration applications received UK wide between the 1st of January 2017 and the 22nd of May 2017. This was        obtained from the Cabinet Office via: https://www.gov.uk/performance/register-to-vote.
    1.	We apportioned this total number of applications to individual constituencies in England, Wales and Scotland proportional to the          distribution that was observed between the number of registered voters on the 31st of December 2014 for each constituency (as              reported by the ONS) and the number of registered voters for the 2015 General Election for each constituency (as reported by the          Electoral Commision). This assumes that the rate of registration in individual constituencies would be the same as in the last            General Election – in reality this might be a strong assumption.
        1. Originally, we apportioned the total number in proportion to the population (not the past election distribution) but this                  didn’t take into account the student population - which can register either at home or where they go to university - so we used            the above model instead.
    1.	We computed the total number of registered voters for the 2017 elections for each constituency by adding up the number of people          registered at the end of 2016 with the apportioned number of those registered in 2017. 
    1.	We subtracted the number of people that are likely to have fallen of the register (e.g. died) in the first five months of 2017. (We        did this by comparing December 2015 to December 2016 registration numbers after subtracting the number of registrations received          between the two months).
    1.	We then rescaled these estimates according to the likelihood of being registered, obtained using a statistical model based on the          British Elections Study data from 2016 and age, education and gender.

1.	**The number and proportion of those who are likely to turnout in 2017:** This was obtained using a statistical model based on the British Elections Study data from 2016 and age, education and gender data from Census data projected to 2016 and rescaled to match proportionally the 2015 turnout level for each constituency.
 
1.	**The number and proportion of those who are NOT likely to turnout in 2017:** This was computed by subtracting those that are likely to turn out from the number of people that are registered.
 
1.	**The number and proportion of those who are likely NOT to be registered in 2017:** This was obtained using a statistical model based on the British Elections Study data from 2016 and age, education and gender data from Census data projected to 2016 and rescaled to match the total number of registered voters. This estimate was floored at 0.
 
1.	**The number and proportion of those who are eligible to vote 2017:** This was computed by subtracting from the general population of each constituency the number of persons aged 0 to 17. This number was obtained from the 2011 Census and updated using a growth factor of 0.03053 for England and Wales and 0.01379 for Scotland. The growth factor was obtained by comparing mid-year ONS population estimates for 2011 and 2015 (most recent available) (https://www.ons.gov.uk/peoplepopulationandcommunity/populationandmigration/populationestimates)
 
1.	**The general population of each constituency:** This was obtained from the 2011 Census and updated using the same growth factors as mentioned above. The growth factors were applied constantly across constituencies (this assumes that the population in each constituency grew at approximately the same rate).
<br></br>
### The Datasets
The first two datasets you will find in the ‘Data’ sections are the ‘Voter Power Story Data’ containing the data we ended up using in our piece and a spreadsheet of survey responses.

The other datasets are split in two folders, one for England and Wales (with the files marked ‘EW’) and one for Scotland (with the files marked ‘S’).

Each of these contains the four datasets:
1.	 **Basic -** a smaller sample of the political, electoral and demographic data that you can take a look at to get familiar with the data.
1.	**Political Electoral Modelled -** to get detailed political and electoral data.
1.	**Demographic -** to get detailed demographic data.
1.	**Powergroups -** to get up-to-date modelled data for 72 precise demographic groups.

Some of this data is as recent as this year but many are from the 2011 Census, which may also come in handy.

This very detailed dataset can be used for multiple purposes - beyond this story - and we encourage you to do so!
<br></br>
### Finding constituencies
For all datasets (except for the survey responses), each row is a constituency. This allows you to filter just for one constituency and easily get the data in the columns that accompany it, but also allows you to access all constituencies if you want to compare one or more constituencies to the whole.

Filtering the region column can help you find the constituencies you are interested in.
<br></br>
### The demographic info
* As we mentioned earlier, you can also find demographic information for England and Wales in the data folder by going to ‘EW Demographic’ found in the ‘England and Wales’ folder of the ‘Data’ section.

* A lot of these are from the 2011 census, but there’s also some more recent datasets we’ve incorporated in there. 

* We’ve used this ourselves for the statistical model we used to break down the register and turnout data by gender, age and education.
<br></br>
### The Stories Derived from the Data
* Plymouth Herald
“Revealed: 3,000 new voters could swing general election in Plymouth's tightest seat”
http://www.plymouthherald.co.uk/revealed-3-000-new-voters-could-swing-election-in-plymouth-s-tightest-seat/story-30374982-detail/story.html

* The Bristol Cable
“Data leaves Bristol, dark ads arrive: how microtargeting is changing elections”
https://thebristolcable.org/2017/07/data-leaves-bristol-dark-ads-arrive-microtargeting-changing-elections/

* Daily Gazette/Essex County Standard
“Some 6,000 new voters register for Thursday's election - more than in any other marginal constituency”
http://www.gazette-news.co.uk/news/15329028.More_than_9_000_new_registered_voters_forecast_for_town_s_election/

* Oxford Mail
“Revealed: New data shows who could tip the battle for Oxford West and Abingdon”
http://www.oxfordmail.co.uk/news/yourtown/oxford/15330177.Revealed__New_data_shows_who_could_tip_the_battle_for_Oxford_West_and_Abingdon/

* Ham&High
“Influx of new voters in Hampstead and Kilburn could swing the election”
http://www.hamhigh.co.uk/seasonal/election/influx-of-new-voters-in-hampstead-and-kilburn-could-swing-the-election-1-5052678

* Chester Chronicle
“Could Chester's former UKIP voters decide city's next MP?”
http://www.chesterchronicle.co.uk/news/chester-cheshire-news/could-chesters-former-ukip-voters-13149238

* East London Lines
“Young voters could sway Croydon”
http://www.eastlondonlines.co.uk/2017/06/young-voters-could-sway-croydon/

* Richmond & Twickenham Times
“New voters could decide Twickenham in general election”
http://www.richmondandtwickenhamtimes.co.uk/news/15331489.New_voters_could_decide_Twickenham_in_general_election/

* digitalWestie GitHubGist
“What matters in predicting voter turnout?”
https://gist.github.com/digitalWestie

* Sutton Coldfield Local
“Why 17000 UKIP voters could hold the balance of power in Erdington, Edgbaston and Northfield”
http://suttoncoldfieldlocal.co.uk/17000-ukip-voters-hold-balance-power-erdington-edgbaston-northfield-4237642342/

* New-West Evening Mail
“New voters hold power to decide crucial Barrow and Furness constituency”
http://www.nwemail.co.uk/news/barrow/New-voters-hold-power-to-decide-crucial-Barrow-and-Furness-constituency-22d6f880-9854-4054-ad7b-b77d7e47fdcd-ds

* Croydon Advertiser
“​1,800 new voters could swing Croydon Central vote, new data reveals”
http://www.croydonadvertiser.co.uk/8203-1-800-new-voters-could-swing-croydon-central-vote-new-data-reveals/story-30376525-detail/story.html

* Devonlive.com
“Calls made for an inquiry into postal vote 'cock-up' in Plymouth”
http://www.devonlive.com/calls-made-for-an-inquiry-into-postal-vote-cock-up-in-plymouth/story-30376026-detail/story.html

* Clacton Gazette
“It's all over bar the voting... YOU go to the polls today to vote for your MP in the UK General Election 2017”
http://www.clactonandfrintongazette.co.uk/news/north_essex_news/15333536.ELECTION__It_s_all_over_bar_the_voting____YOU_go_to_the_polls_today_to_vote_for_your_MP/

* Daily Gazette
“It's all over bar the voting... YOU go to the polls today to vote for your MP in the UK General Election 2017.”
http://www.gazette-news.co.uk/news/local/15333536.ELECTION__It_s_all_over_bar_the_voting____YOU_go_to_the_polls_today_to_vote_for_your_MP/

* Oxford Herald
“Revealed: New data shows who could tip the battle for Oxford West and Abingdon”
http://www.heraldseries.co.uk/news/15330177.Revealed__New_data_shows_who_could_tip_the_battle_for_Oxford_West_and_Abingdon/

* Your Local Guardian
“First time voter Oliver Finney says he was denied his chance to vote in Twickenham 'because his name had already been crossed”
http://www.yourlocalguardian.co.uk/news/15339514.This_first_time_voter_says_he_was_denied_his_chance_to_vote_in_Twickenham__because_his_name_had_already_been_crossed_off_/

* Your Local Guardian
“New voters could decide Twickenham in general election.”
http://www.yourlocalguardian.co.uk/news/15331489.New_voters_could_decide_Twickenham_in_general_election/

