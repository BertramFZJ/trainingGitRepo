CXX = gcc
COMPILER_OPTIONS = -fopenmp -O2

TARGET = gitProject

SOURCES = main.c f1.c f2.c f3.c

OBJECTS = $(patsubst %.c, %.o, $(SOURCES))

%.o : %.c
	@echo "compiling $^ ..."
	@$(CXX) $(COMPILER_OPTIONS) -c $^ -o $@

all : $(OBJECTS)
	@echo "building $(TARGET) ..."
	@$(CXX) $(LINKER_OPTIONS) $(OBJECTS) -o $(TARGET).exe

clean :
	@rm -f $(TARGET).exe $(OBJECTS)
