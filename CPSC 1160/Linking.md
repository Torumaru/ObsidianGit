	Combines all object files and produces desired output file
	Linkers also ensure all cross-file dependancies are resolved properly. For example if you define something in one .cpp file, and then use a different .cpp file, the linker will connect the two files

- If the linker is unable to create a connection then you will get a link error
- Linkers are also able to link libraries, a library file with precompiled code for reuse in other programs