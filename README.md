# Model-View-Controller

## Overview
We've already explored separation of concerns in the web part of the prework where a website had it's structure (HTML), style (CSS) and interactivity (JavaScript) in three different files. As we build full web applications - websites that store, manipulate and show data in response to user actions, we will need to use a separation of concerns framework called MVC, or Model-View-Controller.


## Objectives
1. Define the three components of web-apps
2. Understand the value of placing logic in expected places.
3. Know what *presentation logic* is and how it differs from *business
   logic*.

## Separation of Concerns
Separation of Concerns is a design principle that helps us keep code logically organized by ensuring that each part of an application concerns itself with a specific job. In web applications, we will separate our code by three main parts - the model, view and controller.

Model-View-Controller style frameworks allow developers to connect data to front-end displays. Essentially, MVC is an architectural principle of software design, where developers have broken down the roles of an application into three main portions. The idea is to separate the ‘logic’ of a program from the ‘aesthetics’ of an application, with a sort of ‘middleman’ connecting the two. Let’s talk about each of these:

### Models
These files are the ‘logic’ of your program. Models are Python classes that connect to a database and allow for data to be created, read, updated and deleted. For example, most applications will have a ‘User’ model with attributes such as name, email, and password.

### Views
Views are the pages that users see when they visit your site. They are written in HTML, with data injected into them dynamically.

### Controllers
Controllers are the middlemen between the models and the views. When a user requests a page (a GET request) it is sent to a controller, that ‘routes’ the browser to the correct view. For example, if a user goes to www.rottenpotatoes.com/WarStores, the controller looks for a ‘/WarStores’ route, and if it is found will return the appropriate view (html page) to the user. If a user submits a form (a POST) request, the controller receives the data and sends it to the appropriate model, where an instance of the model is created/read/updated/deleted/saved.


## The Restaurant Analogy
A good analogy for the MVC model is a restaurant - where there is a separation of concerns among the staff - A *server* takes your order, a *cook* prepares your order, a *food runner* brings it to your table, and a *busser* cleans up after you - and all of them work together to provide the cohesive experience of eating out.

Sure, the cook could do everything. In a small restaurant with only a few customers, it might be manageable for the same person who takes your order to be the one that cooks it. But, if that restaurant is bigger than say, a food truck, there's a good chance that things would get out of control and the cook would never know what she or he is supposed to do at any given time. Likewise, nobody else at the restaurant would know what the cook is supposed to be doing, and everyone would go looking at the cook for *everything*, which seems like kind of a nightmare!

## Conclusion
The Model-View-Controller paradigm helps us separate our concerns and know where to put certain kinds of code.

We could put all of our code in one file, but then the file is in the same spot as that overworked cook - doing so much that nobody knows what it's supposed to be doing. In a tiny application with only one developer, this might work for a while, but as the application and the team grow, everyone needs to know where to go to find certain kinds of code. MVC is present in most app framework and the last technical part of this prework will walk through how Google App Engine maps out each component.
