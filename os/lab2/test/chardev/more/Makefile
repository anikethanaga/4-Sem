
obj-m+=devread.o
all:
	make -C /lib/modules/$(shell uname -r)/build/ M=$(PWD) modules
	cc test.c -o test
clean:
	make -C /lib/modules/$(shell uname -r)/build/ M=$(PWD) clean
	rm test