# El-MBR
## ¿Qué es el MBR?
- El MBR *(Master Boot Record)* es el “Sector Cero” del disco duro, este sector contiene la información necesaria para poder arrancar el Sistema Operativo que hay instalado. 

## ¿Qué contiene el MBR?
###  El MBR casi siempre se refiere al sector de arranque de 512 bytes. En el que esta el primer sector físico del disco (pista cero).

- Con 446 bytes. El **Código máquina** *(gestor de arranque)*
- Con 64 bytes.	La **tabla de particiones** *(4 registros que definen cada una de las particiones primarias)*
- Con 2 bytes. La **Signature** *("55h AAh" en hexadecimal)*

## Código Máquina

- El código máquina pesa 446 bytes, y es el proveniente de la tarea de compilación efectuada directamente sobre el Código Fuente, con el que se obtiene posteriormente el Código de Bytes

## Tabla de particiones

- La tabla de particiones pesa 64 bytes, y es la encargada de guardar toda la información de las particiones y la estructura del disco.

## Signature

- La Signature pesa 2 bytes, y es 

