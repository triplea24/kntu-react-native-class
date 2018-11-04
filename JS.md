# Javascript

## Basics

### Variables

	x = { 
		a: 12,
	};
	
	x[a] = 3;
	
	x.a = 4;

### Logging

	console.log('Hello world');

### Constants

	const x = 2;
	x = 3; // NOT Permitted!

### functions

	function makeDouble(x){
		return 2*x;
	}


## ES6 specific codes

### Arrow functions

	const makeDouble = (x) => {
		return x * 2;
	}
Or

	const makeDouble = x => {
		return x;
	}
Or

	const makeDouble = x => x * 2;