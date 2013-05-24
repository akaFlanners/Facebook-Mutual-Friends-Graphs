Facebook-Mutual-Friends-Graphs
==============================

Using a Faceook json file (instructions for obtaining contained within) display a graph of mutual friends.

Note: Most browsers will require the files to be hosted on a sever due to local file system access restrictions.

A sample json file has been created which shows the graph usage with a minimal amount of data: friends_mr_men.json
This file is read by rankByMutualFriendsMrMen.html.

A standalone version with real data obtained from my profile has been added. 
(The results of the json tally are included as an array hardcoded in the javascript).

This shows that the scales in the real data need to be much larger.
A single result of 1 friend having over 200 mutual friends in common creates a much larger span of data.
