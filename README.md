# El-MBR
## ¿Qué es el MBR?
- El MBR *(Master Boot Record)* es el “Sector Cero” del disco duro, este sector contiene la información necesaria para poder arrancar el Sistema Operativo que hay instalado. 

## ¿Qué contiene el MBR?
### El MBR casi siempre se refiere al sector de arranque de 512 bytes. En el que esta el primer sector físico del disco (pista cero).

- Con 446 bytes. El **Código máquina** *(gestor de arranque)*
- Con 64 bytes.	La **tabla de particiones** *(4 registros que definen cada una de las particiones primarias)*
- Con 2 bytes. La **Signature** *("55h AAh" en hexadecimal)*

## Código Máquina

- El código máquina pesa 446 Bytes, y es el proveniente de la tarea de compilación efectuada directamente sobre el Código Fuente, con el que se obtiene posteriormente el Código de Bytes

## Tabla de particiones

- La tabla de particiones pesa 64 Bytes, y es la encargada de guardar toda la información de las particiones y la estructura del disco.

## La Signature 

- La signature pesa 2 Bytes, es un numero identificador para diferenciar el disco duro.

## Las Reglas de las particiones MBR

1. Como máximo hay **4 particiones primarias**
2. Una de las primarias puede ser **extended** .
3. Dentro de la extended (si existe) pueden haber **'n' lógicas**
4. Es obligatorio que una primaria sea **Active** .

- Si es el sistema operativo es **Windows**, es **obligatorio** la norma de que una partición primaria sea Active para que el S.O pueda arrancar.
- Pero si es **Linux** , puede iniciarse sin ninguna particion Active porque puede poner el grub donde sea.
- El máximo tamaño por partición son de **2T**, como son 4 particiones en total serán 8T.

## El FAT32

- El FAT32 es un sistema de archivos utilizado para dispositivos de alamcenamiento, como un disco, un pen formateado.
- El FAT32 es de 32 bits por lo cual tiene como máximo 4GB. 
Por lo cual si tienes por ejemplo un pen formateado y es FAT32, el máximo de memória es de 4GB, y no podras poner una peli de 6GB un sistema operativo de más de 4GB, etc, porque como es fat32 el límite es de 4GB
