+++
title = "Tutorial 13"
description = ""
weight = 14
+++
{{< lead >}}
<br/>


Welcome to the thirteenth tutorial in the InterMine python tutorial series! This tutorial will tell you about the Query Manager and how you can take advantage of it to make better use of queries. We hope at this stage you have the 'intermine' package installed.

We start by importing the module from the InterMine package.

The next step will be to access the account we want to manage:
save_mine_and_token is a method to access an account from a particular mine. We can see here the first variable is flymine, which is a particular mine we want to access an account from. The second variable is the API token linked to your account. You can get the token in your account details.

<br/>
<br/>
<img src="https://i.imgur.com/W9ASC36.png" width="700" height="600" />

<br/>

There are now **four functions** 
that we can utilise:

First, post_query - it posts a query with name and other information as shown in the form of string. If the name is already existed, it will print “The query name exists”.

Here we can see test is posted.

Second, get_all_query_names - it returns all queries that are saved in your account.

Third, get_query - it returns information about the query whose name is 'test’’.

Last, delete_query - it 'deletes the query whose name is 'test’' from user's account.


Now that we have made dealing with queries easier, the next tutorial will have details of how we can visualise the data using the Python client.

Thank you for watching!
