include /home/ssobhani/Cantera/cantera/Install_dir/include/cantera/Cantera.mak

CC=mpicc
CXX=mpicxx
RM=rm -f
CCFLAGS=-g
CPPFLAGS=$(CANTERA_INCLUDES)
LDFLAGS=
LDLIBS=$(CANTERA_LIBS)

SRCS=rankine.cpp
OBJS=$(subst .cpp,.o,$(SRCS))

all: rankine

rankine: $(OBJS)
	$(CXX) $(LDFLAGS) -o rankine $(OBJS) $(LDLIBS)

clean:
	$(RM) $(OBJS)

dist-clean: clean
	$(RM) *~ 
