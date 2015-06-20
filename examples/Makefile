CC=gcc
all:
	$(CC)  -L.. -I../includes ledBlink.c -lfirmatac -o ledBlink.ex
	$(CC)  -L.. -I../includes servoTest.c -lfirmatac -o servotest.ex
 

clean:
	rm *.ex

re: clean all

distclean: clean
