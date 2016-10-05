include /home/ssobhani/Cantera/cantera/Install_dir/include/cantera/Cantera.mak

CC=mpicc
CXX=mpicxx
RM=rm -f
CCFLAGS=-g
CPPFLAGS=$(CANTERA_INCLUDES)
LDFLAGS=
LDLIBS=$(CANTERA_LIBS)

SRCS=kinetics1.cpp
OBJS=$(subst .cpp,.o,$(SRCS))

all: kinetics1

kinetics1: $(OBJS)
	$(CXX) $(LDFLAGS) -o kinetics1 $(OBJS) $(LDLIBS)

clean:
	$(RM) $(OBJS)

dist-clean: clean
	$(RM) *~ 
