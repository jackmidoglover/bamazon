# bamazon
## What is bamazon?
Bamazon is a command line interface for a fictional store, "Selene's Books and Crafs". Bamazon allows 3 different functionalities
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

![view all products](/bamazonscreenshots/view_inventory.png)

![view low inventory](/bamazonscreenshots/low_inventory_command.png)

![add to inventory](/bamazonscreenshots/add_inventory.png)

![add to inventory department list](/bamazonscreenshots/add_product_dept.png)

![add to inventory](/bamazonscreenshots/add_product.png)

### Bamazon supervisor application
![supervisor main menu](/bamazonscreenshots/main_menu_sup.png)

![view departments](/bamazonscreenshots/view_depts.png)

![add department](/bamazonscreenshots/add_dept.png)
