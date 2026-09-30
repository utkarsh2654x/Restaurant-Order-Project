# Restaurant Order System

This is a simple restaurant ordering program that I made in python. You can see the menu, order food, and get an order summary with the bill and discount. It keeps running with a menu until you choose to quit.

I made it using only basic python, so there are no functions and no modules in it. It uses loops, a dictionary and a list.

## What it does

- Shows a main menu with 4 options
- Displays the food menu with prices
- Lets you order items by typing the item number and quantity
- Adds the quantity if you order the same item again
- Generates an order summary with total items, bill, discount and final amount
- Asks for confirmation before placing the order
- Checks the input so wrong values do not crash the program

## How to run

1. Open the notebook (restaurant_order_final.ipynb) in jupyter or vscode
2. Run the first cell (it stores the menu)
3. Run the second cell (the main program)
4. Type a number from 1 to 4 and press enter
5. Follow the instructions on the screen

## Main menu

```
WELCOME TO THE RESTAURANT
1) Display Menu
2) Order Food
3) Generate Order Summary
4) Quit
```

## Food menu

| No. | Item              | Price (Rs) |
|-----|-------------------|------------|
| 1   | Paneer Tikka      | 180        |
| 2   | Veg Burger        | 90         |
| 3   | Margherita Pizza  | 250        |
| 4   | White Sauce Pasta | 150        |
| 5   | Dal Makhani       | 170        |
| 6   | Butter Naan       | 40         |
| 7   | Cold Coffee       | 80         |
| 8   | Gulab Jamun       | 60         |

## How the bill is calculated

- Total = sum of (quantity x price) for every item ordered
- Rs 500 or more = 10% discount
- Rs 1000 or more = 20% discount
- Less than Rs 500 = no discount
- Amount to pay = total - discount

## Example

```
Enter your choice: 2

Item number (0 to stop): 1
Quantity of Paneer Tikka: 2
Paneer Tikka added
Item number (0 to stop): 6
Quantity of Butter Naan: 4
Butter Naan added
Item number (0 to stop): 7
Quantity of Cold Coffee: 2
Cold Coffee added
Item number (0 to stop): 0

Enter your choice: 3

      ORDER SUMMARY      
Paneer Tikka : 2 x 180 = 360
Butter Naan : 4 x 40 = 160
Cold Coffee : 2 x 80 = 160

Total items = 8
Bill = Rs 680
Discount 10 % = Rs 68.0
To pay = Rs 612.0
Confirm order? (y/n): y
Order placed, thank you!
```

## What I used

dictionary, list, while loops, for loops, range(), if/elif/else, input(), int(), isdigit(), len(), round() and print()

## Problems / things to add later

- The order is lost if you quit without confirming it
- You cannot remove an item or change the quantity after adding it
- The menu is fixed, so a new item has to be added in the code
- The bill is not saved in a file
- Can add functions, a way to remove items and payment options later
