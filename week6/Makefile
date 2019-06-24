all : heaploop stackloop

heaploop : heaploop.c
	gcc -Wall -g -o heaploop heaploop.c
stackloop : stackloop.c
	gcc -Wall -g -o stackloop stackloop.c

traces: heaploop stackloop
	./runit heaploop
	./runit stackloop

clean : 
	rm heaploop stackloop tr-stackloop.ref tr-heaploop.ref marker tmp
