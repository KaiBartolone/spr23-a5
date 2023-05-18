objects = addition.o division.o main.o multiplication.o subtraction.o

calculator: $(objects)
	gcc -o calculator $(objects) -Ioperations.h

$(objects): %.o:%.c
	gcc -c $< -o $@

clean:
	rm calculator
	rm -rf *.o

.PHONY: clean
