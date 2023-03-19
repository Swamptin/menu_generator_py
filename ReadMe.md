### Basic Idea

You run the program and it outputs a weekly menu

Frequency setting. Each meal has a "date last had" vs cannot be had within a 3 week window. 

### MVP

Command line tool that outputs md file including ingredients

### Completed project

An online end point that could be hit from a url. Either a website or an AWS lambda function. 

A feature to allow for the addition of items to the menu. With or without ingredients. If the item is added without ingredients or if those ingredients are malformed, the input into the database should be 'NULL'

A feature to allow for the removal or change of a menu item. Eg removing or updating ingredients, changing the rating system to increase or decrease the rotation. 

To be fleshed out

Special occasion flag? 
A special flag should be present as certain meals are only viable at certain times of the year. These meals would be, for example, Christmas Dinner, or are kept for known special occasions like anniversary meals etc.

### Nuts and bolts: backend

Database with menu items linked to ingredients and a value for how many days each meal will last for. Another column for when it was last picked and also its rotation weighting. A special occasions column. If there is a date present then that meal is placed on that date. Otherwise it is ignored. 

### Nuts and bolts: Frontend

A web page that will allow you to trigger the generation of a menu and then display the menu back to you. A seperate page that allows you to add/edit items to the menu. The add/edit page should also display the menu and allow you to select which item to edit.

The add/edit page needs a number of protections in place. It will need stored/reflected XSS protections as there is a chance that someone could add malicious HTML to the DB and that be reflected back to a user. It will also need a means of ensuring entered data doesn't allow for DB manipulation, destruction, or escape. 

### Meals we can cook
+ Chilli con carne
+ Beef stroganoff 
+ Spaghetti bolognaise 
+ Salmon broccoli and potato/rice
+ Cottage cheese & pesto salmon & etc
+ Honey & mustard salmon & etc
+ Tuscan salmon 
+ Salmon Wellington
+ Roast chicken with Yorkshire pudding etc
+ Chicken tikka masala
+ Chicken korma
+ Lamb flatbread
+ Spaghetti carbonara
+ Chicken spinach pasta
+ Chicken adobo
+ Beef stir fry
+ Pork stir fry
+ Beef burgers
+ Meatballs
+ Dahl from Ruari


