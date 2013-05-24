Facebook-Mutual-Friends-Graphs
==============================

Using a Faceook json file (instructions for obtaining contained within) display a graph of mutual friends.

Note: Most browsers will require the files to be hosted on a sever due to local file system access restrictions.

In order to create your own json file from Facebook:
Visit: https://developers.facebook.com/tools/explorer

Use query: YOUR_FACEBOOK_ID?fields=friendlists.limit(800).fields(id,list_type,name,members.limit(800).fields(id,name)),friends.limit(800).fields(id,name,first_name,last_name,gender,relationship_status,birthday,hometown,location,locale,username,picture,mutualfriends.limit(250).fields(id,name))

NOTES: Works on the assumption that you have less than 800 friends and no friends have more than 250 mutual friends.
(This query can take a while).
You will probably have to ensure this json file is saved in UTF-8 format if you have friends with international characters in their names.

A sample json file has been created which shows the graph usage with a minimal amount of data: friends_mr_men.json
This file is read by rankByMutualFriendsMrMen.html.

A standalone version with real data obtained from my profile has been added (not included my actual .json data).
(The results of the json tally are included as an array hardcoded in the javascript).

This shows that the scales in the real data need to be much larger.
A single result of 1 friend having over 200 mutual friends in common creates a much larger span of data.
