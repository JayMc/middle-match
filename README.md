Middle-match
==========
Finds a price point overlapping halfway between a min and max from both parties (buyer and seller).

## Example

- Paul is selling his car for $10,000. is prepared to take a little less but wants the most for it he can get, range 8,000 - 15000
- Bill wants to buy Pauls car and has a budget of $13,000. Of course he wants the best bargin he can get; range 5,000 - 13,000

Middle-match finds the halfway point between what Paul is prepared to reduce his asking price to and what Bill is prepared to increase his bid to. Both without stepping outside of their ranges.

the resulting price is: $10,500

## Install

npm install middle-match --save

## Usage

var middle = require('middle-match');


var buyer = {
	min: 5000,
	max: 13000
};


var seller = {
	min: 8000,
	max: 15000
}


console.log(middle.match(buyer,seller))

## Testing

With Mocha and Chai
run: npm test
