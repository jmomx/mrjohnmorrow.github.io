---
layout: post
title:  "Google Foobar Challenge 2: The Scheduling Problem"
date:   2014-11-18 22:01:33
categories:
---

After completing my [first challenge]({% post_url 2014-11-17-google-foobar-1 %}), I was given a slightly harder second challenge - the famous [Interval Scheduling Problem](http://en.wikipedia.org/wiki/Interval_scheduling).

The task was as follows:

* I input is a list of start and end times, e.g. `[[1,2][3,4], ... ]`
* The times are between 1 and 1000000, and there are never more than 100 appointments.
* You must create a function where the return value must equal the maximum number of appointments that can be scheduled
* I was given three days to complete the task

# If at first you don't succeed ...

I decided to try to solve the puzzle without looking up the right answer. I first thought that because the number of appointments was limited by the conflicts, and a graph was a good data structure to represent conflicts, that a graph based approach might be fruitful. I quickly made simple Node and Graph data structures, and tested it out. It worked on some tests provided by google, but not all of them.  

# try again

As I was debugging, I began to think that this had to be an over-complicated solution to the problem. I went to Wikipedia and found that the much simpler "Earliest Finishing Time" algorithm was the optimal solution:


