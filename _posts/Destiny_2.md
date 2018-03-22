---
layout: post
title: Destiny II Recommender Systems - Gaming Analytics
tags: [Test, Markdown]
---

**Student Group**: Northwestern University Master of Science in Analytics (MSiA) 
**Team Members**: Emma Li, Grace Cui, Rishabh Joshi, Vincent Wang, Varun Gupta

# 1. Problem Statement

In order to improve the levels of player engagement for Massively Multiplayer Online Games (MMOGs), the intelligent information filtering methods were created to offer players weapon recommendations. Currently, robust and accurate recommendation systems for MMOGs is still under exploration. Existing systems on individual player level are not ideal for the PVP mode settings, since consideration needs to be given to the players interacted and variated by team performance. There are opportunities to expand upon the current individual recommendation systems by including team-level performance data where players are segmented by team activities.

# 2. Purpose and Objectives

A hybrid content and knowledge based team-profile recommendation framework for player-versus- player (PvP) is introduced for the online multiplayer shooter game Destiny 2. More accurate systems advise players on how to improve their match performance and enhance their win rate by recommending weapons or character class or performance metrics to them. 

# 3. Project Deliverables 

The NU student group will be responsible for completing the following: 
⋅⋅* Recommender Systems production code in Python
⋅⋅* Final conference paper submitted in May 2018

# 4. Business Benefits

Accurate and actionable recommendation systems will benefit both players and game developers. For persistent online games such as Destiny 2 that are constantly updated, commercial success rests on the game’s ability to keep a community engaged for long periods of time. Having an accurate recommendation system advising players on how to improve will create more incentive to continue playing, since players know that they have a tangible goal to work towards.

# 5. Tools and Methods

Clustering each players according to three different aspects of their performance in the Crucible in Destiny 2. 

The three dimensions are:
1. weapon performance/preference
2. other performance metrics not tied to weapons (e.g. orb pickups, assists, combat rating)
3. class

Based on the clustering results, each player will be given a series of labels, which characterize their behavior and game play style. 

After labeling each player, the baseline recommendation is then to look at the team we want to give a recommendation, take each player and cluster them, building the team across the three dimensions and the win/loss ratio, and possibly other team performance metrics like total wins, average combat rating, etc. According to the clusterings, we can then find teams with the same combination of player label series but with higher win/loss ratio (or other team performance feature) from the data, and recommend against them. We could find 3-5 teams that come from different areas of the combination of clusters as the team we are recommending for, to give a few varied examples. We can at any time exclude one or two dimensions from the recommendation if needed.

# 6. Scope

The NU student group will complete the items outlined in Project Deliverables. The NU student group will review and analyze PVP play data in Destiny 2 extracted through Destiny 2 API. Additional information such as PVE, player geographical, or any other data that is considered irrelevant for the analysis will not be considered.

The NU student group will perform analysis of data using appropriate analytical techniques, present the findings in reports and presentations, and provide recommendations on how the players’ data is clustered and labeled in team-level. The NU student group will provide an analysis and model to facilitate future analysis that incorporates all relevant data sets. 

# 7. Timeline

* Winter Quarter (Jan 10, 2018 – March 24, 2018) 
Review and confirm project scope and problems
⋅⋅* EDA and identify the data sources for analysis
●	Data cleansing and integration
●	Feature selection and engineering
●	Provide initial observations
●	(Perform clustering on players)
●	Label players based on the clustering results/three dimensions 


* Spring Quarter (April 3, 2018 – June 16, 2018) 
●	Aggregate the players’ labels into team level
●	Cluster labeled teams
●	Build and evaluate recommender systems 
●	Reddit feedback analysis 
●	Paper drafting










Jekyll supports the use of [Markdown](http://daringfireball.net/projects/markdown/syntax) with inline HTML tags which makes it easier to quickly write posts with Jekyll, without having to worry too much about text formatting. A sample of the formatting follows.

Tables have also been extended from Markdown:

First Header  | Second Header
------------- | -------------
Content Cell  | Content Cell
Content Cell  | Content Cell

Here's an example of an image, which is included using Markdown:

![Image of a glass on a book]({{ site.baseurl }}/assets/img/pexels/book-glass.jpeg)

Highlighting for code in Jekyll is done using Base16 or Rouge. This theme makes use of Rouge by default.

{% highlight js %}
// count to ten
for (var i = 1; i <= 10; i++) {
    console.log(i);
}

// count to twenty
var j = 0;
while (j < 20) {
    j++;
    console.log(j);
}
{% endhighlight %}

Type on Strap uses KaTeX to display maths. Equations such as $$S_n = a \times \frac{1-r^n}{1-r}$$ can be displayed inline.

Alternatively, they can be shown on a new line:

$$ f(x) = \int \frac{2x^2+4x+6}{x-2} $$
