all: 

	swig -c++ -python -o LN_Class_wrap.cpp LN_Class.i
	gcc -c -fPIC LN_Class_wrap.cpp -o LN_Class_wrap.o -I/usr/include/python2.7 -I../first -I ../second
	g++ -fPIC -shared LN_Class_wrap.o -I../first -I../second -L../first -L../second -lLN_Class -lLongNumber -o _LN_Class.so
