# video08

+++ title = "Tutorial 8" description = "" weight = 9 +++    


Welcome to the eighth tutorial in the InterMine python tutorial series! This very short tutorial will talk about how to access your saved templates and lists if you have your login information \(username and password\). If you don’t have an account, you can create one at flymine.org

Once you have made an account, you can use the web service to create a query of your choice and save it as a template. This template can be used through Python API or through the web service.

To login and access your templates through Python, you can provide your login information as shown below. The code shown below is in comments because it needs to be specific to your account. Change the username and password to match yours, uncomment the code, and then run it.

If you are not comfortable using your username and password, check out tutorial 14 where we show you another way to authenticate using an API token.

Then you can play around with this saved template like any of the existing templates on FlyMine.

To view the names of all the available templates you can view the templates dictionary and iterate through it. This can be done as follows.

Here we print all names of templates in FlyMine.

This dictionary contains all the information about all the available templates including the exact name and description. If you want to view the details about a particular template name, this can be done as shown below, using the name of the template in quotes and square brackets.

You can also view the templates on the FlyMine user interface at [https://www.flymine.org/flymine/templates.do](https://www.flymine.org/flymine/templates.do), or by visiting flymine.org and clicking the templates tab.

You can scroll through the list of templates. If you find an interesting template, click on the template and click on the Python tab \(in blue\). This would show you how to call the template in Python using the exact name.

Also, you can try our latest BlueGenes platform\([http://bluegenes.apps.intermine.org/flymine](http://bluegenes.apps.intermine.org/flymine)\) where you can search all the templates.

In the next tutorial, we will talk about how you can create and save lists in your account.

Thank you for watching!

## Screenshots showing how to get a template you are interested in on the flymine website:

![](https://i.imgur.com/AV3S7Lk.png)

![](https://i.imgur.com/1YTQQA7.png)

