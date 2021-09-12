###################################################
#Archivo de desripción para compilar el proyecto miinodo
#$ld$
#$Author: Anonimos
#################################################

##################################################
# Definición de macros
##################################################
COMPILADOR=gcc -g

FUENTE = miinodo.c stub.c

OBJS=$(FUENTE:.c=.o)

HEADER=$(RUTA_INCL)miinodo.h

PROG=$(RUTA_BIN)miinodo
CC: $(OBJS)
	$(COMPILADOR) $(OBJS) -lm -o $(PROG)
	@- echo "Compilación terminada”
LIMPIA:
	@- rm -f $(OBJS)
	@- echo "Borrado de objetos terminado”
BORRA:
	@- rm -f $(OBJS) $(PROG)
	@- echo "Borrado de archivos terminado”
.c.o:
	$(COMPILADOR) -c -I$(RUTA_INCL) $*.c -o $*.o
$(OBJS): $(RUTA_INCL)$(HEADER) 
