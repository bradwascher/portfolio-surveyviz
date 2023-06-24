# About
This script processes and visualizes survey results from the [Cooperative Election Study (CES/CCES)](https://cces.gov.harvard.edu), demonstrating how different demographic coalitions voted in the 2008–2020 presidential elections. The first half of the code wrangles the survey microdata, while the second half outputs various charts. This was originally a project I did in graduate school.


# Output
### Whose Destiny Did Demographics Decide?: Visualizing the 2020 Cooperative Election Study (CCES)
Originally 5/17/2021

Joe Biden’s victory over Donald Trump in the 2020 election came thanks
to a broad coalition…sort of. But what exactly did that coalition look
like? And how did it compare to that of Hillary Clinton in 2016, or
previous Democratic presidential candidates? These answers and more can
be found in the [Cooperative Election
Study](https://cces.gov.harvard.edu/).

The Cooperative Election Study, also known as the Cooperative
Congressional Election Study or CCES, is a comprehensive survey of over
50,000 respondents across the United States, administered online via
YouGov as part of a joint effort between dozens of different academic
and research institutions. Although the CCES is conducted annually, its
election-year installments are special in that they’re fielded in two
waves: one before the election, and one after. Due to its large sample
size and vote validation after the fact, the CCES is [considered to
be](https://fivethirtyeight.com/videos/be-wary-of-exit-polls-this-year-well-and-all-years/)
a more rigorous alternative to the exit polls taken on Election Day. At
the very least, [it is widely
agreed](https://centerforpolitics.org/crystalball/articles/another-look-back-at-2016/)
that the CCES is a reliable reference for anyone curious about who voted
for whom on the Tuesday next after the first Monday last November.

The following visualizations will seek to give additional context to the
recently released [2020 Cooperative Election Study post-election
wave](https://dataverse.harvard.edu/dataset.xhtml?persistentId=doi%3A10.7910/DVN/E9N6PH)
by analyzing support for Biden and Trump across various demographic
groups, and then comparing those to the equivalent estimates from the
2016 Cooperative Congressional Election Study. All data has been
reweighted using the information provided by the CCES.

## CCES Estimates vs. 2020 Results

Before diving in, it’s important to remember that the Cooperative
Election Study is still just a poll. As a result, its estimates don’t
always line up with the real outcome of the election. The first map
compares the state-level estimates from the 2020 CCES to the true
results, whereas the second map compares the proportion of a state’s
respondents to its contribution to the national popular vote:

![alt text](https://github.com/bradwascher/portfolio-surveyviz/blob/main/images/1.png)
![alt text](https://github.com/bradwascher/portfolio-surveyviz/blob/main/images/2.png)


As demonstrated above, the CCES was far from flawless last November. On
average, the state-level results overestimated support for Joe Biden by
approximately 2 to 4 points, ultimately overshooting his actual vote
share in 35 states and the District of Columbia. But that kind of error
wasn’t unique to this one survey; by and large, [most pollsters had a
rough go in
2020](https://fivethirtyeight.com/features/the-death-of-polling-is-greatly-exaggerated/).
While it will still [take
time](https://www.aapor.org/Publications-Media/Press-Releases/AAPOR-Convenes-Task-Force-to-Formally-Examine-Poll.aspx)
for experts in the field to more critically diagnose what went wrong,
projects such as the CCES help to facilitate this work with its own
demographic estimates of the electorate. Interestingly, the
state-by-state breakdown of CCES sample matched closely to each state’s
eventual share of the national popular vote (For example, California
comprised 8.4% of the CCES sample while contributing to 11% of the
national popular vote — this discrepancy of 2.6 points was by far the
largest recorded).

## Election Results by Gender

Although politics in the United States have become increasingly
polarized [over the last two decades
especially](https://www.pewresearch.org/politics/2019/12/17/in-a-politically-polarized-era-sharp-divides-in-both-partisan-coalitions/),
one demographic gap has been drawn out along party lines for the better
part of the [past 40
years](https://www.pewresearch.org/politics/2019/12/17/in-a-politically-polarized-era-sharp-divides-in-both-partisan-coalitions/).
Indeed, women continued to vote for Democrats at higher rates than they
did for Republicans in 2020, even more so than in 2016 — while support
among men improved for both Trump and Biden. Per the 2016 CCES, Hillary
Clinton earned 53 percent of women voters, compared to 42 percent for
Donald Trump. Joe Biden further built on this advantage four years
later, earning a slightly larger share (56-43) over Trump relative to
Clinton. In both 2016 and 2020, Trump earned more support among men.

![alt text](https://github.com/bradwascher/portfolio-surveyviz/blob/main/images/3.png)
![alt text](https://github.com/bradwascher/portfolio-surveyviz/blob/main/images/4.png)


## Election Results by Education

One of the [big
stories](https://www.brookings.edu/research/americas-electoral-future_2018/)
of the 2016 election was Donald Trump’s strong support among voters
without a college degree: the 2016 CCES approximates that he won this
group 51-44 — and he did even better among white voters without a
college degree in particular. Likewise, Hillary Clinton was
substantially more popular than Trump (55-38) among those who said they
had at least a bachelor’s degree.

According to the 2020 CCES, these gaps grew even larger. While Trump’s
support among voters without a college degree hovered at a similar
position in both 2016 and 2020, Joe Biden’s advantage among voters with
a college degree grew to around 20 points, a marked improvement from
Clinton’s already impressive showing four years earlier. These
differences raise questions about the long-term trajectory of this
educational divide: in the span of just a few cycles, the gap has gone
from a [relative non-factor in
elections](https://www.pewresearch.org/fact-tank/2016/09/15/educational-divide-in-vote-preferences-on-track-to-be-wider-than-in-recent-elections/)
to one of the [most important demographic trends of
all](https://www.nytimes.com/2020/05/12/upshot/polls-2020-trump-biden.html).

![alt text](https://github.com/bradwascher/portfolio-surveyviz/blob/main/images/5.png)
![alt text](https://github.com/bradwascher/portfolio-surveyviz/blob/main/images/6.png)


## Election Results by Race

While Donald Trump ultimately fell short of a second term, he managed to
win [12 million more
votes](https://uselectionatlas.org/RESULTS/index.html) in 2020 than he
did in 2016. Part of this increased support might have come from
minority voters. Compared to Hillary Clinton’s performance in 2016, and
especially Barack Obama’s showings in 2008 and 2012, Joe Biden failed to
make serious gains among most groups — and it appears he may have lost
voters overall.

Many of the differences between the 2016 and 2020 CCES are too close to
tell for certain, but there’s other evidence in favor of the theory that
Trump gained support among certain minority voters. Areas including
[Miami-Dade County in
Florida](https://twitter.com/xxxneonslavexxx/status/1328853223214559233)
and [the Rio Grande Valley in
Texas](https://www.theguardian.com/commentisfree/2020/nov/24/the-10-swing-state-counties-that-tell-the-story-of-the-2020-election),
both of which are areas with high Hispanic populations, veered toward
Trump by as much as 20 or 30 points last November; the latest CCES
estimates, on the other hand, showed Trump gaining just a few points
among Hispanic voters overall between 2016 and 2020. To be sure, the
possibility that Hispanic voters were underrepresented in 2020
pre-election polls is [one that pollsters
recognize](https://www.nytimes.com/2020/11/10/upshot/polls-what-went-wrong.html)
— it also doesn’t help that the CCES lists only ‘Hispanic’ as an answer
on its questionnaire, rather than providing more specific choices (such
as nationality) that might more faithfully capture the contours of this
demographic group.

![alt text](https://github.com/bradwascher/portfolio-surveyviz/blob/main/images/7.png)
![alt text](https://github.com/bradwascher/portfolio-surveyviz/blob/main/images/8.png)


## Election Results by Age

In the lead-up to the 2020 election, there was much
[chatter](https://www.brookings.edu/blog/the-avenue/2020/10/28/older-voters-may-secure-a-biden-victory-in-2020s-swing-states/)
online about Joe Biden’s strong support among older voters. Although the
2016 CCES suggested that Donald Trump carried voters over the age of 65
by 13 points nationwide against Hillary Clinton, [some state-level
polling](https://int.nyt.com/data/documenttools/flpa-0930-crosstabs/16c21b7ab34ed4d1/full.pdf)
conducted weeks before the 2020 race showed Joe Biden ahead among this
group. But in the end, that support didn’t fully materialize, as the
2020 CCES post-election survey suggested Trump won among voters over 65
by 9 points against Biden, continuing a streak of sorts for Republican
presidential candidates.

That said, relative to Clinton four years before, Biden still made
improvements among older voters, and among *most* age groups for that
matter. This boost was particularly prominent among voters aged 18-34:
Clinton won them by 20 points, Biden won them by approximately 30
points.

![alt text](https://github.com/bradwascher/portfolio-surveyviz/blob/main/images/9.png)
![alt text](https://github.com/bradwascher/portfolio-surveyviz/blob/main/images/10.png)


## Closing Thoughts

The 2020 election certainly had its surprises. But six months later,
more information has allowed some of those questions to be answered.

Using data from the 2016 and 2020 post-election waves of the Cooperative
Election Study, the preceding visualizations have compared support for
Hillary Clinton, Joe Biden, and Donald Trump by gender, educational
attainment, race, and age. This preliminary analysis suggests that Biden
improved upon Clinton’s margins in groups such as younger voters and
voters with a college degree. While certain other estimates from the
CCES do not appear to be substantively different between both elections
years, these findings are not conclusive, and future research could
serve to establish clarity on these issues.
