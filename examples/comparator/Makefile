CXX=g++
CXXFLAGS=-I../../ -W -Wall
LDFLAGS=-lads1015 -L../../
EXEC=Comparator
SRC=comparator.cpp
OBJ=$(SRC:.cpp=.o)

all: $(EXEC)

$(EXEC): $(OBJ)
	$(CXX) -o $@ $^ $(LDFLAGS)

$(OBJ): $(SRC)
	$(CXX) -o $@ -c $< $(CXXFLAGS)

clean:
	rm -f $(OBJ)

mrproper: clean
	rm -f $(EXEC)
