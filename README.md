# Python_Django


Django is a Python-based web framework which allows you to quickly create web application without all of the installation or dependency problems that you normally will find with other frameworks. Django is based on MVT (Model View Template) architecture and revolves around CRUD (Create, Retrieve, Update, Delete) operations. CRUD can be best explained as an approach to building a Django web application. In general CRUD means performing Create, Retrieve, Update and Delete operations on a table in a database. Let’s discuss what actually CRUD means,
 

Create – create or add new entries in a table in the database. 
Retrieve – read, retrieve, search, or view existing entries as a list(List View) or retrieve a particular entry in detail (Detail View) 
Update – update or edit existing entries in a table in the database 
Delete – delete, deactivate, or remove existing entries in a table in the database
 

Django CRUD (Create, Retrieve, Update, Delete) Function Based Views
Illustration of How to create and use CRUD view using an Example. Consider a project named geeksforgeeks having an app named geeks. 

After you have a project and an app, let’s create a model of which we will be creating instances through our view. In seeks/models.py, 

Create View

Create View refers to a view (logic) to create an instance of a table in the database. It is just like taking an input from a user and storing it in a specified table. 
In geeks/views.py, 


To check complete implementation of Function based Create View, visit Create View – Function based Views Django.
 

Retrieve View

Retrieve view is basically divided into two types of views Detail View and List View. 
 

List View
List View refers to a view (logic) to list all or particular instances of a table from the database in a particular order. It is used to display multiple types of data on a single page or view, for example, products on an eCommerce page. 
In seeks/views.py, 


Create a template in templates/list_view.html, 


To check complete implementation of Function based List View, visit List View – Function based Views Django 
 

Detail View
Detail View refers to a view (logic) to display a particular instance of a table from the database with all the necessary details. It is used to display multiple types of data on a single page or view, for example, profile of a user. 
In seeks/views.py, 


Let’s create a view and template for the same. In seeks/views.py,

Create a template in templates/Detail_view.html, 

To check complete implementation of Function based Detail View, visit Detail View – Function based Views Django
 

Update View

Update View refers to a view (logic) to update a particular instance of a table from the database with some extra details. It is used to update entries in the database for example, updating an article at geeksforgeeks. 
In seeks/views.py,


Now create following templates in templates folder, 
In geeks/templates/update_view.html,

Let’s check if everything is working, visithttp://localhost:8000/1/update. 

To check complete implementation of Function based update View, visit Update View – Function based Views Django
 

Delete View

Delete View refers to a view (logic) to delete a particular instance of a table from the database. It is used to delete entries in the database for example, deleting an article at geeksforgeeks. 
In sheek/views.py 

Now a url mapping to this view with a regular expression of id, 
In sheek/urls.py 

Template for delete view includes a simple form confirming whether user wants to delete the instance or not. In sheek/templates/delete_view.html, 

Everything ready, now let’s check if it is working or not, visit http://localhost:8000/2/delete 

 
