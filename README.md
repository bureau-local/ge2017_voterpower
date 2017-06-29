# Voter Power GE2017
*A Bureau Local Investivation*

**Which group of voters can determine the election’s outcome**

#### Hypothesis:
The ‘first past the post’ electoral system in place in the UK doesn’t grant every voter the same power. The datasets contained in this repositery were put together with this in mind by the Bureau Local in order to understand the demographics of the UK electorate ahead of the 2017 General Election and to discover which constituencies, and which groups within them, held the most sway.

From education, to age, to those registered and not, we set out to find out who had the power to determine the result in their local constituency and how that reflected national trends.

#### Voter Power Hack Day:
Assembling the combined effort of local journalists across the country for a hack day, the aim was to dig into the data together and break on the same day to create a national and local discussion on voter power.

At the hack day everyone had a chance to dig into a vast dataset of variables related to demographics - from income and education levels to past vote, marginality and past registration. The model also used data on England and Wales from the Office of National Statistics, the Cabinet Office and the British Election Study to estimate the number registered voters seat by seat - something not available in a central database.

Throughout the hackday 65 participants in Glasgow, Cardiff, Bournemouth, Birmingham and London each dug into the data differently in order to find stories for their own communities. Two journalists in London - Matty Edwards and Ed Fairhead - started looking at how our estimated registration numbers compared to the margin in the seats they cover, Croydon Central and Colchester respectively. They found these seats to have an increase in voter registration larger than the 2015 margin. They also looked at the size of past UKIP voters in Colchester where the party was no longer standing in 2017.

The Bureau worked with them and expanded their measures across the country. We found there to be 71 seats where these 'partyless' voters were larger than the margin in the last election - 19 due to increase in new voters alone.

We then rang up local authorities to get actual registration numbers for over 50 constituencies - in doing do, finding that our model was very close (if over-estimated registration figures by less than 1% on average) and we used exact numbers in our piece.

#### The Methodology:
There is a lot of data in our database - over 600 variables actually!
Here’s how we obtained the variables:
 
1.	% vote share for each party in the 2015 and 2010 elections: We divided the number of votes each party received by the total number of people that voted in that constituency.
1.	The number of registered voters in 2017: we derived the number of registered voters in each constituency for the coming elections, using data from several sources and carrying out several procedures:
    1.	We used data from the ONS that reported the exact number of registered voters on the 31st of December 2016 for each constituency
    1.	We used the number of registration applications received UK wide between the 1st of January 2017 and the 22nd of May 2017. This was        obtained from the Cabinet Office via: https://www.gov.uk/performance/register-to-vote.
    1.	We apportioned this total number of applications to England + Wales and to Scotland proportional to their respective population            sizes. Following this, we apportioned these numbers to individual constituencies proportional to their size (this assumes that the        rate of registration is similar across constituencies – in reality this might be a strong assumption).
    1.	We computed the total number of registered voters for the 2017 elections for each constituency by adding up the number of people          registered at the end of 2016 with the apportioned number of those registered in 2017. 
    1.	We subtracted the number of people that are likely to have fallen of the register (e.g. died) in the first five months of 2017. (We        did this by comparing December 2015 to December 2016 registration numbers after subtracting the number of registrations received          between the two months).
    1.	We then rescaled these estimates according to the likelihood of being registered, obtained using a statistical model based on the          British Elections Study data from 2016 and age, education and gender.

1.	The number and proportion of those who are likely to turnout in 2017: This was obtained using a statistical model based on the British Elections Study data from 2016 and age, education and gender data from Census data projected to 2016 and rescaled to match proportionally the 2015 turnout level for each constituency.
 
1.	The number and proportion of those who are NOT likely to turnout in 2017: This was computed by subtracting those that are likely to turn out from the number of people that are registered.
 
1.	The number and proportion of those who are likely NOT to be registered in 2017: This was obtained using a statistical model based on the British Elections Study data from 2016 and age, education and gender data from Census data projected to 2016 and rescaled to match the total number of registered voters. This estimate was floored at 0.
 
1.	The number and proportion of those who are eligible to vote 2017: This was computed by subtracting from the general population of each constituency the number of persons aged 0 to 17. This number was obtained from the 2011 Census and updated using a growth factor of 0.03053 for England and Wales and 0.01379 for Scotland. The growth factor was obtained by comparing mid-year ONS population estimates for 2011 and 2015 (most recent available) (https://www.ons.gov.uk/peoplepopulationandcommunity/populationandmigration/populationestimates)
 
1.	The general population of each constituency: This was obtained from the 2011 Census and updated using the same growth factors as mentioned above. The growth factors were applied constantly across constituencies (this assumes that the population in each constituency grew at approximately the same rate).

#### The Datasets
The first two datasets you will find in the ‘Data’ sections are the ‘Voter Power Story Data’ containing the data we ended up using in our piece and a spreadsheet of survey responses.

The other datasets are split in two folders, one for England and Wales (with the files marked ‘EW’) and one for Scotland (with the files marked ‘S’).

Each of these contains the four datasets:
1.	 **Basic** - a smaller sample of the political, electoral and demographic data that you can take a look at to get familiar with the data.
1.	**Political Electoral Modelled** - to get detailed political and electoral data.
1.	**Demographic** - to get detailed demographic data.
1.	**Powergroups** - to get up-to-date modelled data for 72 precise demographic groups.

Some of this data is as recent as this year but many are from the 2011 Census, which may also come in handy.

#### Finding your constituency
For all datasets (except for the survey responses), each row is a constituency. This allows you to filter just for one constituency and easily get the data in the columns that accompany it, but also allows you to access all constituencies if you want to compare one or more constituencies to the whole.

Filtering the region column can help you find the constituencies you are interested in.

Alternatively, this constituency explorer map can also help you find the names of the constituencies in your area if you are unsure what they are all called. 
Click “Enlarge Map” and then the region you are interested in, the map will zoom on that part of the UK and you will be able to search for constituencies names more visually.

