# Magento 2 Module and Theme Demo
This is the content of a Module and Themes for a Magento 2 demo project.

## Dependencies
* A fresh local installation of the latest Magento 2 Community version (currently v.2.4.6-p4)

## Common Usage
You can either fork this repo. or download its content as a zip and then copy to your local Magento installation
the following directories:
* `app/design/frontend/EW/`.
* `app/code/EW/`.

After copying those files:
1. First, with your local Magento installation running, refresh the storefront homepage and login into your admin area, 
that allows the themes included to get automatically registered and added to the database.
2. Second, run `bin/magento setup:upgrade` so the new included module gets registered and 
all its setup patches with automated processes and configurations are performed.

After taking those steps you should find on your local Magento installation:
* Two store views, the default store view and an "AT Store View", 
these store views should display all text using the 'Quicksand' font which is set in the custom theme.
  (If you notice that is not the case, it means that the custom themes need to be set via the admin, 
please go to admin **Content > Design > Configuration** and then set the "Theme One" globally 
and "Theme Two" to the "AT Store View").
* A new block on the storefront homepage showing only "Featured" products, which can be added to the cart 
using the product's card "Add To Cart" button.
* When hovering over each product card of the "Featured" products you should get a gray background color,
and when switching to the "AT Store View", you should get a 'golden' type background color.
* After a customer account is created, you should see a "Hobbies" text field for the customer to fill 
in the account information edit form of the customer account, 
and also in the customer account information form of the admin area.
* After adding a product to the cart and navigating to the checkout, 
you should see a "Purpose" text field in the shipping information form to be filled in and after placing the order,
you should see such "Purpose" value included in the shipping information section of the order data in the admin area.

License
----

MIT
