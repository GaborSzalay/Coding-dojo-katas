# Kata 001 - Pricing in a supermarket

## Background story

You work for a supermarket chain. You have to write a text parsing logic that can handle shopping carts of customers.

An example shopping cart looks like this (each bullet point supposed to be represented as strings):
* football - 2 pieces
* apple  - 1 kg
* orange juice - 3 pieces
* pasta - 4 pieces
* chicken breast - 1.5 kg

Cart items have their prices:
* football - 17 EUR / piece
* apple - 0.7 EUR / kg
* orange juice - 1.5 EUR / piece
* pasta - 1.2 EUR / piece
* chicken breast - 5.3 EUR / kg

Keep that in mind that the orders of the stories are **not strict** especially in case of story 1 and story 2.

## User story 1 - *shopping cart lines*
Please parse the lines of shopping cart and return the items cut in pieces.

Actual result: `"football - 2 pieces"`
Expected result: `"football", "2", "pieces"`

## User story 2 - *pricing lines*
Please parse the lines of price list and return the items cut in pieces.

Actual result: `"football - 17 EUR / piece"`
Expected result: `"football", "17", "piece"`

## User story 3 - *Total price*
Please write a logic that is capable to parse shopping carts like the one above and calculates the **total price.**

Expected result in case of the given list and prices: 51.95 EUR

## User story 4 - *Action 3 for 2*
It turned out that there is a 3 for 2 action on orange juice. Every third piece of juice you buy is for free.
Please enable the list of items that have 3 for 2 action and create discounted price next to total price:
* orange juice

Total price: 51.95 EUR - Discounted price: 50.45 EUR

## User story 5 - *Percentage discount*

## User story 6 - *Bigger and smaller*
Our boss initiated to have new type of quantities in the customers' shopping carts. I'm sorry, I really do.
Please create a new shopping cart with the following items:
* chicken breast - 500 g
* football - 2 packages
* pasta - 2 pieces
* apple  - 2 kg

The prices are the same as above, please apply the already parsed data on this set as well.
Please convert the quantities based on the following list:
* package - 5 pieces
* kg - 1000 g

Finally please calculate the total price of the new list. It should be 176.45 EUR

## User story 7 - *Currency exchange*