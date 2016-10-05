include /home/ssobhani/Cantera/cantera/Install_dir/include/cantera/Cantera.mak

CC=mpicc
CXX=mpicxx
RM=rm -f
CCFLAGS=-g
CPPFLAGS=$(CANTERA_INCLUDES)
LDFLAGS=
LDLIBS=$(CANTERA_LIBS)

SRCS=combustor.cpp
OBJS=$(subst .cpp,.o,$(SRCS))

all: combustor

combustor: $(OBJS)
	$(CXX) $(LDFLAGS) -o combustor $(OBJS) $(LDLIBS)

clean:
	$(RM) $(OBJS)

dist-clean: clean
	$(RM) *~ 
