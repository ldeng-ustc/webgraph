include ../flags.mk

all: compress_webgraph print_webgraph print_webgraph_offline print_webgraph_sequential

compress_webgraph: compress_webgraph.o
	g++ -static -L$(LIBS) -L.. -o compress_webgraph compress_webgraph.o \
			 -lwebgraph -lboost_regex -lboost_program_options -lboost_filesystem

print_webgraph: print_webgraph.o
	g++ -static -L$(LIBS) -L.. -o print_webgraph print_webgraph.o \
			 -lwebgraph -lboost_regex -lboost_program_options -lboost_filesystem

print_webgraph_offline: print_webgraph_offline.o
	g++ -static -L$(LIBS) -L.. -o print_webgraph_offline print_webgraph_offline.o \
			 -lwebgraph -lboost_regex -lboost_program_options -lboost_filesystem

print_webgraph_sequential: print_webgraph_sequential.o
	g++ -static -L$(LIBS) -L.. -o print_webgraph_sequential print_webgraph_sequential.o \
			 -lwebgraph -lboost_regex -lboost_program_options -lboost_filesystem

install:
	cp compress_webgraph ~/random-bin

%.o : %.cpp
	g++ -I$(INCLUDES) $(FLAGS) -c $<

clean:
	rm -f *.o
	rm -f *~
