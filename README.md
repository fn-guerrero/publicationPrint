# publicationPrint

Script to generate publication-ready figures in Matlab

```Matlab
function publicationPrint(fig,ancho,alto,nombre_archivo,tipo,fsz, fName)
```
Asigna un tamaño en cm a la figura, cambia letra a Times New Roman 11 y
exporta una imágen del tipo pedido. Opcionalmente se puede cambiar fsz 
y fName para modificar el tipo de letra. 

### ARGUMENTOS:

- fig:      handle a la figura (h1 = handle(1) gcf recupera el handle actual)
- ancho:    ancho en cm
- alto:     alto en cm o array vacío [] para relación 1.6
- nombre:   nombre del archivo
- tipo:     Tipo de archivo a generar: 'png' , 'eps', 'pdf'

OPCIONAL: 

- fsz:      tamaño de letra (default 11)
- fName:    Tipografía (default Times New Roman)

## EJEMPLO TIPICO: 

```Matlab
publicationPrint6(gcf,8.6,[],'Figura1','pdf')
```

guarda la figura actual en el directorio actual, con ancho 8.6 
y alto 8.6/1.6
