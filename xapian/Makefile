PROGRAM := notdeft-xapian

default : build

-include local.mk

build : $(PROGRAM)

$(PROGRAM) : notdeft-xapian.cc
	g++ -o $@ -std=c++11 -Wall -I ./tclap/include `xapian-config --cxxflags --libs` $<

clean :
	-rm $(PROGRAM)

install-deps :
	sudo aptitude install libtclap-dev libxapian-dev
