all : folders int

folders :
	if [ ! -d "./bin/elf/" ]; then mkdir -p bin/elf; fi
	if [ ! -d "./bin/pe/" ]; then mkdir -p bin/pe; fi


int : src/int.c
	gcc -m32 -o bin/elf/int-x86.elf src/int.c
	gcc -o bin/elf/int-x64.elf src/int.c


.PHONY : clean

clean :
	rm -rf bin/*
