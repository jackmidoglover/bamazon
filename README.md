# bamazon
## What is bamazon?
Bamazon is a command line interface for a fictional store, "Selene's Books". Bamazon allows 3 different functionalities
depending on whether the user is a customer, a store manager, or a store supervisor. 

## How it works
Bamazon utilizes the node packages inquirer, mysql, and cli-table. By answering different inquirer prompts, the user can access data related
to the store's inventory to accomplish different actions.

### Bamazon customer application

![customer menu](/bamazonscreenshots/main_menu.png)

This menu allows customers to choose whether they want to purchase an item from the store or exit the application.

![inventory in sql](/bamazonscreenshots/stock_before_buy.png)

The app pulls data from mysql and populates a list of available inventory for the customer to buy.

![show customer inventory](/bamazonscreenshots/buy_options.png)

When the customer buys the inventory, the app calculates the amount of items purchased and the item's price and gives the customer a total.

![customer buy](/bamazonscreenshots/customer_buy.png)

The inventory is then subtracted from the stock_quantity in sql.

![inventory in sql after buy](/bamazonscreenshots/stock_after_buy.png)


### Bamazon manager application
![manager menu](/bamazonscreenshots/main_menu_man.png)

Managers are first presented with this main menu of options: View current inventory, view low inventory, add inventory, and add products.

![view all products](/bamazonscreenshots/view_inventory.png)

Above is an example of the list that is populated from the database giving managers information about the total inventory.

![view low inventory](/bamazonscreenshots/low_inventory_command.png)

The manager can also search the database for inventory with a stock_quantity of 5 or less.

![add to inventory](/bamazonscreenshots/add_inventory.png)

They can add inventory to products in the database.

![add to inventory](/bamazonscreenshots/add_inventory_choices.png)

First they are shown the inventory available so they can choose what to add to.

![add to inventory department list](/bamazonscreenshots/add_product_dept.png)

Managers are also able to add new products to the database. They are shown a list of departments they can add products to.

![add to inventory](/bamazonscreenshots/add_product.png)

They can then add a product.

![validation](/bamazonscreenshots/valid_example.png)

The program checks that the manager input is valid- not NaN or 0.

![inventory added](/bamazonscreenshots/quantity_update.png)

This shows both: the new product added (rune stones) and the inventory added (tarot cards, which in the above example is only 45 and is now 52).


### Bamazon supervisor application
![supervisor main menu](/bamazonscreenshots/main_menu_sup.png)

The main menu for a supervisor gives them the option to view product sales and over all profits by department.

![view departments](/bamazonscreenshots/view_depts.png)

This table uses the cli-table node module to populate a table based on the database information, and calculates a temporary table called total profits.

![add department](/bamazonscreenshots/add_dept.png)

Supervisors are also able to add a department.

![department added](/bamazonscreenshots/dept_added.png)

## Contributers
jackmidoglover
