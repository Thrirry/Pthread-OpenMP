
CC := gcc

assignment2: $(OBJ)
	$(CC) -o gauss gauss.c
	$(CC) -o gauss_pthread gauss_pthread.c -pthread
	$(CC) -o gauss_openmp gauss_openmp.c -fopenmp
	$(CC) -o gauss_pthread_openmp gauss_pthread_openmp.c -pthread -fopenmp

%.o: %.c
	$(CC) -g -c $<

run: assignment2
	./gauss 32

clean:
	rm -rf gauss gauss_pthread gauss_openmp gauss_pthread_openmp *.o
