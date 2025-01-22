input stream std::cin is for standard input/console input

but the stream can be "user defined"

	#include <fstream>
	using std::ifstream;
	ifstream fin;
	fin.open("input.txt");
	// input.txt only has 5 and 6
	int x;
	fin>>x;
	//fin is ture
	fin >>x;
	// fin is true
	fin >> x;
	//fin is false because we run out of data after 6
	fin.clear();
	fin.close();