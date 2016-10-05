include /home/ssobhani/Cantera/cantera/Install_dir/include/cantera/Cantera.mak

F90=gfortran
RM=rm -f
F90FLAGS=-g
F90MODDIR=$(CANTERA_FORTRAN_MODS)
LDFLAGS=
LDLIBS=$(CANTERA_FORTRAN_LIBS)

SRCS=demo.f90
OBJS=$(subst .f90,.o,$(SRCS))

all: demo

demo: $(OBJS)
	$(F90) $(LDFLAGS) -o demo $(OBJS) $(LDLIBS)

%.o : %.f90
	$(F90) -c $< -J$(F90MODDIR) $(F90FLAGS)

clean:
	$(RM) $(OBJS)

dist-clean: clean
	$(RM) *~
