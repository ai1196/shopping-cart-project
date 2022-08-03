# shopping-cart-project

# Shopping Cart Project

This is a python application that will help store owners to enhance the checkout process. 

# Setup 
Optionally fork or clone this [repository](https://github.com/ai1196/shopping-cart-project) that will allow you to create your own copy. You can then proceed to download the remote repository or "clone" it on your local. You can then navigate to where you have downloaded the repo in Terminal.

```
cd ~/desktop/shopping-cart-project
```
Create a virtual environment:
```
conda create -n shopping-env python=3.8
```
Activate the virtual environment:
```
conda activate shopping-env
```
Install package dependencies within the virtual environment:
```
pip install -r requirements.txt
```
Within the active virtual environment of choice, you should be able to run the following Python script from the command line:
```
python shopping_cart.py
```
If you successfully see the "products" data structure, you can proceed with development. 

# Requirements 

Once you have completed the setup steps above, you can continue with the rest of the exercise implementation. 

## Capturing User Inputs

The application should prompt the user to input a product identifier or select 'DONE' if they have no other items to enter, via command-line interface. 

## Look-up Products

Based on the user input, the applications should be able to do a product "look up" to display the product name and price of all the product identifiers that the user has entered.

## Printing the Receipt

Once all user inputs and data have been collected, we need to ensure that we display a receipt that includes, products, price, taxes, total prices and farewell message. 

Here is more detail on the custom receipt components:
+ A grocery store name of your choice
+ A grocery store phone number and/or website URL and/or address of choice
+ The date and time of the beginning of the checkout process, formatted in a human-friendly way (e.g. 2020-02-07 03:54 PM)
+ The name and price of each shopping cart item, price being formatted as US dollars and cents (e.g. $3.50, etc.)
+ The total cost of all shopping cart items (i.e. the  "subtotal"), formatted as US dollars and cents (e.g. $19.47), calculated as the sum of their prices
+ The amount of tax owed (e.g. $1.70), calculated by multiplying the total cost by a New York City sales tax rate of 8.75% (for the purposes of this project, groceries are not exempt from sales tax)
+ The total amount owed, formatted as US dollars and cents (e.g. $21.17), calculated by adding together the amount of tax owed plus the total cost of all shopping cart items
+ A friendly message thanking the customer and/or encouraging the customer to shop again

## Example output
``` 
(shopping-env) Samuels-MacBook-Air:shopping-cart-project samuelkurian$ python shopping_cart.py
Please input a product identifier: 3
Please input a product identifier: 4
Please input a product identifier: 5
Please input a product identifier: done
----------------------------
ASHA'S GROCERY STORE
----------------------------
Web: www.ashasgrocery.com
Phone: 123.456.7890
Checkout Time: 2022-08-03 01:10 AM
----------------------------
Shopping Cart Items:
- Robust Golden Unsweetened Oolong Tea 2.49
- Smart Ones Classic Favorites Mini Rigatoni With Vodka Cream Sauce 6.99
- Green Chile Anytime Sauce 7.99
----------------------------
SUBTOTAL: $17.47
TAX: $1.53
TOTAL: $19.00
----------------------------
Thanks for shopping with us! Hope to see you soon.
----------------------------
(shopping-env) Samuels-MacBook-Air:shopping-cart-project samuelkurian$ python shopping_cart.py
Please input a product identifier, or 'DONE' if there are no more items: 4
Please input a product identifier, or 'DONE' if there are no more items: 3
Please input a product identifier, or 'DONE' if there are no more items: done
#> ----------------------------
#> ASHA'S GROCERY STORE
#> ----------------------------
#> Web: www.ashasgrocery.com
#> Phone: 123.456.7890
#> Checkout Time: 2022-08-03 01:15 AM
#> ----------------------------
#> Shopping Cart Items:
#> - Smart Ones Classic Favorites Mini Rigatoni With Vodka #> Cream Sauce 6.99
#> - Robust Golden Unsweetened Oolong Tea 2.49
#> ----------------------------
#> SUBTOTAL: $9.48
#> TAX: $0.83
#> TOTAL: $10.31
#> ----------------------------
#> Thanks for shopping with us! Hope to see you soon.
#> ----------------------------
```

# Usage
Run the program:
```
python shopping_cart.py
```