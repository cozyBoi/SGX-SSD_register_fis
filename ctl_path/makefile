CC = g++

spm: spm.cpp ctl_path_lib.o KISA_SEED_CMAC.o KISA_SHA256.o 
	$(CC) -o spm spm.cpp ctl_path_lib.o KISA_SEED_CMAC.o KISA_SHA256.o 

ctl_path_lib.o: ctl_path_lib.cpp 
	g++ -c ctl_path_lib.cpp

KISA_SEED_CMAC.o : KISA_SEED_CMAC.c
	gcc -c KISA_SEED_CMAC.c

KISA_SHA256.o : KISA_SHA256.c
	gcc -c KISA_SHA256.c

clean:
	rm -rf spm *.o

# spm

# ctl_path

# KISA_SEED_CMAC

# 이렇게 계단식임