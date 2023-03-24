Hello World Tutorial!

## itemdatabase

> A gamemaker asset for easily making an item database and item handling system.

## What it is

This constructor initializes and creates an item database. It has many static functions that handle everything related to the database.

## Features
- One single function handles everything related to items
- All functions can be accessed via the database
- All code related to the items can be written inside the database
- Two global variables store the items database and the actual inventory

## Examples
First the database must be called to initialize all the static functions within it. The script asset holding the function already does this:
```gml
item_database();
```

Now we can call any static functions inside this constructor by simply dot accessing the function itself:
```gml
var index = item_database.item_index("Donut");
```
Most static functions require the name of the item to execute its code.

Here's a few more uses:
```gml
show_debug_message("The search result is {0}:", item_database.item_index("Onigiri"));
show_debug_message("The sell price for {0} is: {1}","Magical Tome",item_database.get_item_sell_price("Magical Tome"));
show_debug_message("The description for {0} is: {1}","Donut",item_database.get_item_description("Donut"));
```

## Donate

Want to donate? You can [buy me a kofi](https://ko-fi.com/gamedevtosh). :heart: