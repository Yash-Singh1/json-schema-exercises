# Problem 01 - Putting it all together - Hard

This problem combines everything

## Problem

This schema is a bit complicated. First of all, it is an object. The first property is called odd, and it is any odd number. The second property is called transactions, and it is an object that contains properties that have the key of the date format of MM/DD/YY with a value that are arrays. The arrays contain objects. The objects has multiple properties. The first property is a price property that is a float that goes to 2 decimal places or a whole number. The second property is the product, which is a object containing an 5 digit ID (named id) and a name. Another property is the name of the person who bought it. Also, there can be a max of 2 transactions per day. If there are more transactions, then there should be another required property called toomuch, assigned with true. The next property contains a favorite color and can be one of:

- red
- green
- blue
- yellow

Here is an example:

```json
{
  "odd": 5,
  "transactions": {
    "04/23/19": [
      {
        "name": "John Doe",
        "price": 78.98,
        "product": {
          "name": "Hand Sanitizer",
          "id": 15698
        }
      },
      {
        "name": "John Carter",
        "price": 0.01,
        "product": {
          "name": "Grain of Rice",
          "id": 78540
        }
      }
    ],
    "11/26/2020": [
      {
        "name": "Anonymous Patel",
        "price": 10,
        "product": {
          "name": "Black Friday Cookie",
          "id": 67349
        }
      },
      {
        "name": "Fake Name",
        "price": 987.54,
        "product": {
          "name": "Website",
          "id": 01577
        }
      },
      {
        "name": "Third Ordering Dude",
        "price": 12.89,
        "toomuch": true,
        "product": {
          "name": "Dog",
          "id": 59248
        }
      }
    ]
  },
  "color": "red"
}
```

## Solution

Click [here](../../solutions/hard/problem-1/) to get the solutions.
