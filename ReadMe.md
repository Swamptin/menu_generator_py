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

Add feature to reduce food waste. Have carrots etc in all meals in a week means you get through the bag of carrots. 

Special occasion flag? 
A special flag should be present as certain meals are only viable at certain times of the year. These meals would be, for example, Christmas Dinner, or are kept for known special occasions like anniversary meals etc.

### Nuts and bolts: backend

Database with menu items linked to ingredients and a value for how many days each meal will last for. Another column for when it was last picked and also its rotation weighting. A special occasions column. If there is a date present then that meal is placed on that date. Otherwise it is ignored. 

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


