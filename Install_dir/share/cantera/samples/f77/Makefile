include /home/ssobhani/Cantera/cantera/Install_dir/include/cantera/Cantera.mak

FC=gfortran
RM=rm -f
FFLAGS=-g
LDFLAGS=
LDLIBS=$(CANTERA_FORTRAN_LIBS)
CPPFLAGS=$(CANTERA_INCLUDES)

OBJS=isentropic.o demo_ftnlib.o

all: isentropic

isentropic: $(OBJS)
	$(F77) $(LDFLAGS) -o isentropic $(OBJS) $(LDLIBS)

clean:
	$(RM) $(OBJS)

dist-clean: clean
	$(RM) *~
