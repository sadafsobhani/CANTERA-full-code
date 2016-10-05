include /home/ssobhani/Cantera/cantera/Install_dir/include/cantera/Cantera.mak

CC=mpicc
CXX=mpicxx
RM=rm -f
CCFLAGS=-g
CPPFLAGS=$(CANTERA_INCLUDES)
LDFLAGS=
LDLIBS=$(CANTERA_LIBS)

SRCS=NASA_coeffs.cpp
OBJS=$(subst .cpp,.o,$(SRCS))

all: NASA_coeffs

NASA_coeffs: $(OBJS)
	$(CXX) $(LDFLAGS) -o NASA_coeffs $(OBJS) $(LDLIBS)

clean:
	$(RM) $(OBJS)

dist-clean: clean
	$(RM) *~ 
