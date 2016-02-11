You will eventually find 3 files there:

1. The "darkstat.pid" file:
	It contains the pid of the program processus. You will need it to kill the program.
	Use the following command to do so: sudo kill `sudo cat darkstat.pid`
2. The "darkstat.log" file:
	It contains the program logs
3. The "darkstat.db" file:
	It is the database of the program. This file will always be there, unless you delete it at the end of your execution.
	Basically, this is our main output. At each second, the program write in this file the data of the previous second.
	These datas are in a specific format, which contains the current date, in addition to the in/out datas
	The file is in the following format: <day>;<month>;<year>;<hour>;<min>;<sec>;<in>;<out>
