the assignment operator is =
- on the left hand side we have lvalue
- on the right hand side we have rvalue

example
	int w=1; (initializes the variable at declaration time)
	int x{}, y, z; (initialies x to 0)
	const int FACTOR = 5;
	cin>>x>>y;
	z=FACTOR*(x+y)-w;
	z=(y=FACTOR);
	y gets the value of 5 and the assignment returns the value of 5 and this returned value is assigned to x

	>> extraction operator
Must input into a variable, not a constant
- skips blanks, end of lines
- it stops reading (possibly entering the fail state) when it encounters a character in the input stream that could not be part of the right data type

cin>>x>>ch

input 53 b

output
	x 53
	ch b

FAIL STATE

	char ch;
	int x;
	cin >>x>>ch;
input 53b
output x=53 ch=b

stream = a sequence of characters

	char ch;
	int x;
	cin >>x>>ch;
input A B
	cin enters the fail state
output

Augmented assignment operators

Binary operator has 2 operands
x + y (x and y are operands)(+ is operator)

unary operators has 1 operand

examples
	x++
	x--
	+9
	-2

bool dusty = true;
cool salty = false;

	negation is ! (for NOT, has high precedence = high priority)
because unary operators have high precedence

	!salty && dusty
evaluated salty first
