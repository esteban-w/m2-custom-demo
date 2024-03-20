# Magento 2 Module and Theme Demo
This is the content of a Module and Themes for a Magento 2 demo project.

## Dependencies
* A fresh local installation of the latest Magento 2 Community version, 
which at the moment of writing this code is v.2.4.6-p4

## Common Usage

### Installing via Composer
You can easily install this code via Composer:
1. First, with your local Magento installation running, cd into your Magento's root directory and run:
`composer require ew/magento2-module-demo`, after running make sure you get a success message, otherwise please refer 
to the **Installing Manually** instruction below.
2. Then, right after you run that command it is necessary that you refresh the storefront homepage 
and login into your admin area, that allows the themes included to get automatically registered 
and added to the database.
3. Finally, from your Magento's root directory run: `bin/magento setup:upgrade` so the new included module gets 
registered and all its setup patches with automated processes and configurations are performed. After running 
make sure you get a success message, otherwise please refer to the **Installing Manually** instruction below.

### Installing Manually
If you attempted installing via Composer and for some reason installation failed, run: 
`composer remove ew/magento2-module-demo` to make sure you can start a manual installation fresh. 
To manually install you can either fork this repo. or download its content as a zip 
and then copy to your local Magento installation the following directories:
* `app/design/frontend/EW/`.
* `app/code/EW/`.

After copying those files:
1. First, with your local Magento installation running, refresh the storefront homepage and login into your admin area, 
that allows the themes included to get automatically registered and added to the database.
2. Then, run `bin/magento setup:upgrade` so the new included module gets registered and 
all its setup patches with automated processes and configurations are performed.

After taking those steps you should find on your local Magento installation:
* Some base configurations made to the main website, like for example currency defined as EUR. 
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
