CXX= mpicxx
HDRS= solver.h solver.hpp processors.h processors.hpp complex_matrix.h complex_matrix.hpp complex_matrix_io.hpp scalapack.h quantum_system.h

first: my_test

my_test: test.cpp $(HDRS)
	$(CXX) test.cpp -o my_test -lscalapack -llapack -lblas -lgfortran

matrix_test: matrix_test.cpp $(HDRS)
	$(CXX) matrix_test.cpp -o matrix_test -lscalapack -llapack -lblas -lgfortran

experiment: experiment.cpp $(HDRS)
	$(CXX) experiment.cpp -o experiment -lscalapack -llapack -lblas -lgfortran

clean:
	rm -f my_test matrix_test experiment

.PHONY: first clean
