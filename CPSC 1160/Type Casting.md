	int i;
	double d;
- This declaration allocates memory for an integer (typically 4 bytes)
- Because i is declared to be an int, the value stored is going to be interpreted as a whole number
- associates i with the location (address) of the memory allocated
- i is not initialized
- i has a value although not meaningful
- allocates memory for a double d (8 bytes)
	d=5.89;
- assigns 5.89 to the location associated with d
	i=d;
- i and d are different types but it will still compile, at most a warning from the compiler
- there is a loss of information but is will work, i gets the value 5
- where in widening (d=i;)
- there is no loss of information outputting 5

Type cast takes a value of one data type and produces a value of another data type

int y=7;
double d_y
d_y = static_cast <double>(y)

"old" notation for casting (same as java)
(double) y   From C and Java

We could have done the casting automatically
d_y=y;
instead of calling a explicit cast or, easier

cout <<y/2.0<<" is a double\n";
to obtain 3.5

If both operands are integer, the division is integer division
	14/5=2
so the fractional part of the answer is truncated
If at lesat one operand is a double, the resultant is a double and the division is "decimal" division

const int A=14;
const int B=5;

What is the output?
cout<<static_cast <double> (A/B) <<endl;

output
2

How can output 2.8 if I am starting with A and B?
cout << static_cast<double>(A)/B<<endl;
output
2.8

How can I get an integer (int)
resultant that is rounded (up or down)
correctly using type casting

14/5 I want 3 not 2

const int A=14;
const int B=5;

cout<< static_cast<int>static_cast<double>(a)/b+05<<endl;

