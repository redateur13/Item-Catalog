

# Item Catalog project
**by ٌReda Zerrougui**


 ## Project  Description:

This is the 4th project for the Udacity Full Stack Nanodegree , called " Item Catalog"
The Item Catalog project consists of developing an application that provides a list of items within a variety of categories, as well as provide a user registration and authentication system. 
This project uses  data storage to create a RESTful web app that allows users to perform (CRUD)Create, Read, Update, and Delete operations.

A user does not need to be logged in in order to read the categories or items uploaded. However, users who created an item are the only users allowed to update or delete the item that they created.

####   the Computer Books Catalog app  represent the Item Catalog 
## Project contents

Within the download you'll find the following files:

```
Item-Catalog.zip/
├── static/
│   └── css/
│       └──styles.css
│
├── screenshot/
│   └── add.jpg
│   └── book.jpg
│   └── bookJSON.jpg
│   └── catalog.jpg
│   └── catalogJSON.jpg
│   └── categories.jpg
│   └── categoryBooksJSON.jpg
│   └── delete.jpg
│   └── edit.jpg
│   └── login.jpg
│   └── login2.jpg
│
├── templates/
│   └── addBook.html
│   └── base.html
│   └── book.html
│   └── categories.html
│   └── category.html
│   └── deleteBook.html
│   └── editBook.html
│   └── login.html
│   
├── app.py
├── books_catalog.db
├── client_secrets.json
├── database_setup.py
├── fill_database.py
└── README.md
```
## Requirements

-   [VirtualBox](https://www.virtualbox.org/)
-   [Vagrant](https://www.vagrantup.com/)
-   [Python 2.7](https://www.python.org/)](https://www.python.org/)
-   [sqlalchemy_utils](http://initd.org/psycopg/docs/install.html)  `pip install sqlalchemy_utils`(if you want to run the  ``fill_database.py``)
-   [Bash terminal(for windows machine)](https://git-scm.com/downloads)

## Installation

1.  Install Python2.7 , VirtualBox and Vagrant
    
2.  Clone or download the Vagrant VM configuration file from  [fullstack-nanodegree-vm repository](https://github.com/udacity/fullstack-nanodegree-vm)
    
3.  Clone Or download this repository to your desktop , Unzip and  Paste all the files  from this project  `Item-Catalog` into the ```fullstack-nanodegree-vm-master\vagrant\catalog ``` sub-directory
    


## Steps to run this project

1.  Open terminal and go to the folder where you saved the fullstack repository then :  `cd vagrant`.
2.  Launch Vagrant to set up the virtual machine and then log into the virtual machine.:  `vagrant up`  `vagrant ssh`
    
3. Then move inside the catalog folder:
`cd /vagrant/catalog`
    
4. Then run the application:
`python app.py`

5. finally Access and test your application by visiting  [http://localhost:5000](http://localhost:5000/).:
`http://localhost:5000/`
   
    

## The expected program output is as the following : 

http://localhost:5000/ or http://localhost:5000/catalog 
 Returns catalog page with all categories and recently added books without login
 ![alt text](screenshots/catalog.jpg "home page, show categories and latest books .")
 
 
 ```/catalog/<int:catalog_id>```
 ```/catalog/<int:catalog_id>/books```
http://localhost:5000/catalog/1/books
 Returns number of  books in  category 
  ![alt text](screenshots/categories.jpg " show Returns number of  books in  category .")
  
  
```/catalog/<int:catalog_id>/books/<int:book_id>```
http://localhost:5000/catalog/3/books/7
show a Book information
![alt text](screenshots/book.jpg "show a Book information .")


http://localhost:5000/login
login with google api
![alt text](screenshots/login.jpg "login ")
![alt text](screenshots/login2.jpg "login with google .")


http://localhost:5000/catalog/add
Allows user to add a new book
![alt text](screenshots/add.jpg "add a new book ")

``` /catalog/<int:catalog_id>/books/<int:book_id>/edit```
Allows user to edit  his book
![alt text](screenshots/edit.jpg "edit ")


```/catalog/<int:catalog_id>/books/<int:book_id>/delete```
Allows user to delete his book
![alt text](screenshots/delete.jpg "delete ")

## JSON Endpoints
http://localhost:5000/catalog/JSON
![alt text](screenshots/catalogJSON.jpg "json categories")
return categories information

```/catalog/<int:catalog_id>/JSON```
http://localhost:5000/catalog/3/JSON
return category books information
![alt text](screenshots/categoryBooksJSON.jpg " category books ")

```/catalog/<int:catalog_id>/books/JSON```
http://localhost:5000/catalog/2/books/2/JSON
return a book detail
![alt text](screenshots/bookJSON.jpg "  book detail ")


 ## Licence

The MIT License ([MIT](https://choosealicense.com/licenses/mit/#))
Copyright (c) [2018] [Reda Zerrougui]
