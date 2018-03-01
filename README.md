# BikramSambat
Convert between JavaScript Date object to a BikramSambat object representing date in Bikram Sambat calander

## Usage:

### Creating BikramSambat object:
```JavaScript
// Create a BikramSambat with current Date:
let bs = new BikramSambat();

// Create a BikramSambat with given Date:
let date = new Date(1950, 6, 1);
let bs = new BikramSambat(date);

// Create a BikramSambat with specified BikramSambat date:
let bs = new BikramSambat(2000, 6, 1);
```

### Creating a Date object from BikramSambat object:
```JavaScript
// Create a BikramSambat...
let bs = new BikramSambat(2050, 6, 1);
// Get corresponding Date:
let date = bs.toDate();
```

### Setting BikramSambat parameters:
```JavaScript
// Get current BikramSambat:
let bs = new BikramSambat();

// For 'English' - can also be 'ne' for 'Nepali':
bs.language = "en";

// Set month text type to numeric - can also be 'word':
bs.monthType = "number";

// Set month text to short instead of full:
bs.monthTextShort = true;

// Set weekday text to short instead of full:
bs.weekdayShort = true;
```

### Getting text representation of BikramSambat:
```JavaScript
// Create a BikramSambat...
let bs = new BikramSambat(2050, 6, 1);

// Get a full String
console.log(bs.toString()); // Outputs: '१ कार्तिक २०५०'

// Get text of part of BikramSambat:
console.log(bs.getYearText()); // Outputs: '२०५०'
console.log(bs.getMonthText()); // Outputs: 'कार्तिक'
console.log(bs.getDateText()); // Outputs: '१'

// Get values:
console.log(bs.getYear()); // Outputs: '2050'
console.log(bs.getMonth()); // Outputs: '6'
console.log(bs.getDate()); // Outputs: '1'
```
