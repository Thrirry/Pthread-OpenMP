# Pthread-OpenMP
Shared Memory Programming with pthread and openMP

Compilation Steps:

	Method 1: Run make command.
	
		eg: $ make

	Method 2: complie each code individually.

		$gcc -o gauss gauss.c
		$gcc -o gauss_pthread gauss_pthread.c -pthread
		$gcc -o gauss_openmp gauss_openmp.c -fopenmp
		$gcc -o gauss_pthread_openmp gauss_pthread_openmp.c -pthread -fopenmp

Execution steps:

	Sequential Code:
		$./gauss <matrix_dimension> [random seed]
	Pthread Code:
		$./gauss_pthread <matrix_dimension> [random seed]
	OpenMp Code:
		$./gauss_openmp <matrix_dimension> [random seed]
	Combined Code:
		$./gauss_pthread_openmp <matrix_dimension> [random seed]
