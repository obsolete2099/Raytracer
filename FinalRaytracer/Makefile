CXX = g++
CXXFLAGS = -std=c++11


SRCS = raytracer.cpp
OBJS = $(SRCS:.cpp=.o)
EXEC = raytracer

.PHONY: all clean

all: $(EXEC)

$(EXEC): $(OBJS)
	$(CXX) $(CXXFLAGS) -o $@ $^ $(LIBS)

%.o: %.cpp
	$(CXX) $(CXXFLAGS) -c -o $@ $<

clean:
	rm -f $(OBJS) $(EXEC)
