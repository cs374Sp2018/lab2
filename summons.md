<div id="table-of-contents">
<h2>Table of Contents</h2>
<div id="text-table-of-contents">
<ul>
<li><a href="#org1cfc31c">Objective</a></li>
<li><a href="#org8eb9c86">Background</a>
<ul>
<li><a href="#org6ea14d5">Minimal Context</a></li>
</ul>
</li>
<li><a href="#org59c0faa">Problem</a></li>
<li><a href="#org70b7c05">Task 1</a></li>
<li><a href="#org0a119e2">Task 2</a></li>
</ul>
</div>
</div>


<a id="org1cfc31c"></a>

Objective
=========

This assignment will demonstrate your proficiency with objected oriented design patterns and 
python syntax while introducing you to some of the challenges in processing criminal summonses
in NYC.  


<a id="org8eb9c86"></a>

Background
==========

Context is available from Misdemeanor Justice Project report on summons which students are
encouraged to read in its entirety. The report is available at:

[<https://www.jjay.cuny.edu/sites/default/files/news/Summons_Report_DRAFT_4_24_2015_v8.pdf>](https://www.jjay.cuny.edu/sites/default/files/news/Summons_Report_DRAFT_4_24_2015_v8.pdf)


<a id="org6ea14d5"></a>

Minimal Context
---------------

As a minimum students should know

> What is a summons? A summons is issued when an authorized law
> enforcement agent, most commonly a member of the New York City Police
> Department, encounters an individual who is engaged in conduct that
> allegedly violates certain provisions of the administrative code,
> penal law, or health code. This is a high-volume enforcement activity
> in New York City. In the decade covered by this report, on average
> about a half million summonses were issued each year. On a daily
> basis, the number of summonses issued ranged from a high of about
> 1,600 in 2006 to a low of about 1,200 in 2013. The vast majority (over
> 97 percent) was issued by the New York City Police Department.  These
> summonses are issued for a variety of law violations. As is documented
> in this report, the five most frequent charges in 2013 were public
> consumption of alcohol, disorderly conduct, public urination, park
> offenses, and riding a bicycle on the sidewalk.


<a id="org59c0faa"></a>

Problem
=======

How can we model the issuance and resolution of accusatory instruments?


<a id="org70b7c05"></a>

Task 1
======

Create several classes.  We are going to embed them in the summons class. 

-   Defendant
-   Officer
-   Prosecutor
-   Judge

For our purposes now, we will assume that all summons are issued in
Manhattan. We will now create a summons class.  Make sure the class
keeps track of the number of objects instantiated. Also use the count 
to assign a number called the id to the summons.

A summons will also need an issuance date. Three months after the issuance
there will be a hearing date. (Just and 3 months, do not use the more complicated
date or datetime objects).

Every summons will need a decision.  Set the random seed equal to 42. Every charge 
has a 95% probability of conviction. Use python's random library to determine innocence 
or guilt.


<a id="org0a119e2"></a>

Task 2
======

-   You will print out of all defendants for each judge.
-   You will print out a notification for each defendant of when their court date is.
-   If the defendant is found guilty you will print out a bill charging them $100.

