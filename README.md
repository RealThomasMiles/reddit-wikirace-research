

RESEARCH ON THE POSSIBILITY TO

PLAY THE WIKI RACE GAME USING

SUBREDDITS

Dmitry Milya, 3530903/80302





INTRODUCTION

A Wikirace is a race between any number of participants,

using links to travel from one Wikipedia page to another.

The first person to reach the destination page, or the

person that reaches the destination using the fewest

links, wins the race. Intermediary pages may also be

required.

The goal of this research is to find out whether it is

possible, and if yes then if it is easy enough for a human,

to play the Wikirace game on Reddit with subreddits

instead of pages using crossposts as links between

them.





METHODOLOGY

SNAP: Social Network: Reddit Hyperlink Network

<https://snap.stanford.edu/data/soc-RedditHyperlinks.html>

The hyperlink network represents the directed connections

between two subreddits. The network is extracted from

publicly available Reddit data of 2.5 years from Jan 2014 to

April 2017 containing 571928 crossposts.

The method is to calculate the fraction of nodes in the

largest connected component and the mean shortest path

length of the network along with the mean weight of these

paths to decide whether it is possible and easy enough for a

human to play the Wikirace game using crossposts as links

between subreddits.





The directed connections between

two subreddits were represented

as a weighted edge csv-list with

weight calculated as inverse of the

number of crossposts between the

connected subreddits in order to

help calculate the “difficulty” of

traversion.

EXPERIMENTAL SETUP

The resulting network consists of:

• 234792 edges

• 2135 nodes





CALCULATION RESULTS

The network is not connected, the fraction of vertices in

the weakly connected component is 74.8% and the

fraction of vertices in the strongly connected component is

5.6%.

The mean shortest path length of the network is 5.884 and

the mean weight of these paths is 2.667.





DISCUSSION

The network under consideration is not connected, although the fraction of

vertices in the weakly connected component is 74.8% which is high enough for

the game to be possible, however the fraction of vertices in the strongly

connected component is only 5.6% which does not guarantee that the game

will have a large variety of starting and destination subreddits.

The mean shortest path length of the network is 5.884 and the mean weight of

these paths is 2.667 which means that on average the best playthrough is

going to be around 6 steps long but on this path each subreddit will have only

around 2 crossposts leading to the next subreddit which, considering that the

data spans over 2.5 years, may be very hard to find depending on the

frequency of new posts on the subreddit.

In conclusion, the results above may be interpreted as such: it is possible to

play the game although the difficulty of each run depends heavily on the

frequency of new posts on the subreddits that lay on the path between the

starting and destination subreddits. The result could be more certain if the data

contained such information.

