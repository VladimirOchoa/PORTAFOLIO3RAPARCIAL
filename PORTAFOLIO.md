# Presentacion 
## Problemas resueltos en clase con DFD
## Adrian Vladimir Ochoa Ramirez
### Ejercicio 1. Utilizando 2 vectores capture edad y semestre de n estudiantes.
#### 1.1 Analisis. 
En el presente DFD se pretende realizar un logaritmo que capturar la edad en un vector y el semestre en otro vector de n cantidad de alumnos.
#### 1.2 DFD
[![6.jpg](https://i.postimg.cc/sD0rYc0H/6.jpg)](https://postimg.cc/HV5RHQmb)
#### 1.3 Prueba de escritorio 
corrida|valor i|VE|VS|i=n?|
|-|-|-|-|-|
|1|0|VE[0]=16|VS[0]=3|no|
|2|1|VE[1]=17|VS[1]=5|no|
|3|2|VE[2]=18|VS[2]=7|no|
|4|3|VE[3]=17|VS[3]=5|Si, impr VE y VS|

|Edad|Semestre|
|-|-|
|16|3|
|17|5|
|18|7|
|17|5|
#### 1.4 Entradas.
ne,
ed,
se.
#### 1.5 Salidas.
Ae, AS
### Ejercicio 2. Utilizando una matriz capture edad y semestre de n estudiantes.
#### 2.1 Analisis. 
En el presente DFD se pretende realizar un logaritmo que capturar la edad y el semestre dentro de una matriz de n cantidad de alumnos.
#### 2.2 DFD
[![7.jpg](https://i.postimg.cc/vm0kyHFq/7.jpg)](https://postimg.cc/2qB2FY5h)
#### 2.3 Prueba de escritorio
|corrida|valor i|valor j|matriz|i=n?|
|-|-|-|-|-|
|1|0|0|M[0,0]=16|no|
|2|1|0|M[1,0]=17|no|
|3|2|0|M[2,0]=17|no|
|4|3|0|M[3,0]=16|Si, entonces sig contador|

|corrida|valor i|valor j|matriz|i=n?|
|-|-|-|-|-|
|1|0|0|M[0,1]=3|no|
|2|1|0|M[1,1]=5|no|
|3|2|0|M[2,1]=5|no|
|4|3|0|M[3,1]=3|Si, entonces impr [M]|

|Edad|Semestre|
|-|-|
|16|3|
|17|5|
|17|5|
|16|3|
#### 2.4 Entradas.
ne, ed,se.
#### 2.5 Salidas.
M.
### Ejercicio 3. Rellenar una matriz cuadrada de [n*n], con un numero leido del teclado.
#### 3.1 Analisis. 
En el presente DFD se pretende realizar un logaritmo que rellenar una matriz cuadrada, con el numero leido por el teclado.
#### 3.2 DFD
[![8.jpg](https://i.postimg.cc/FsnYY0bN/8.jpg)](https://postimg.cc/RNKS86bD)
#### 3.3 Prueba de escritorio
|matriz|numero|i|j|m[i,j]=numero|j<matriz|j++|i<matriz|i++|
|------|------|-|-|-------------|--------|---|--------|---|
|2*2   |7     |0|0|m[0,0]=7     |0<2     |1  |        |   |
|      |      |0|1|m[0,1]=7     |1<2     |   |0<2     |1  |
|      |      |1|0|m[1,0]=7     |0<2     |1  |1<2     |   |
|      |      |1|1|m[1,1]=7     |1<2     |   |        |   |
#### 3.4 Entradas.
n, num.
#### 3.5 Salidas.
M.
### Ejercicio 4. Rellenar una matriz cuadrada con numeros consecutivos de n*n.
#### 4.1 Analisis. 
En el presente DFD se pretende realizar un logaritmo que rellenar una matriz cuadrada, con numeros consecutvos (de uno en uno).
#### 4.2 DFD
[![9.jpg](https://i.postimg.cc/RF6Bbn6Q/9.jpg)](https://postimg.cc/gXWQxjKn)
#### 4.3 Prueba de escritorio
|matriz|c     |i|j|m[i,j]=c     |j<matriz|j++|i<matriz|i++|c=c++|
|------|------|-|-|-------------|--------|---|--------|---|-----|
|2*2   |0     |0|0|m[0,0]=0     |0<2     |1  |        |   |     |
|      |1     |0|1|m[0,1]=1     |1<2     |   |0<2     |1  |2    |
|      |      |1|0|m[1,0]=2     |0<2     |1  |1<2     |   |     |
|      |3     |1|1|m[1,1]=3     |1<2     |   |        |   |     |
#### 4.4 Entradas.
n,.
#### 4.5 Salidas.
M.
### Ejercicio 5. Rellenar una matriz cuadrada con numeros consecutivos, que cada renglon tenga un mismo numero de n*n.
#### 5.1 Analisis. 
En el presente DFD se pretende realizar un logaritmo que rellenar una matriz cuadrada con numeros consecutivos, de la forma que el primer renglon tenga puros 1, el segundo renglon tenga puros 2 y asi susecivamente.
#### 5.2 DFD
[![10.jpg](https://i.postimg.cc/52YSy4CK/10.jpg)](https://postimg.cc/ZWmdDhj6)eba de escritorio
#### 5.3 Prueba de Escritorio.
|matriz|i|j|m[i,j]=j+1   |j<matriz|j++|i<matriz|i++|
|------|-|-|-------------|--------|---|--------|---|
|2*2   |0|0|m[0,0]=1     |0<2     |1  |        |   |
|      |0|1|m[0,1]=1     |1<2     |   |0<2     |1  |
|      |1|0|m[1,0]=2     |0<2     |1  |1<2     |   |
|      |1|1|m[1,1]=2     |1<2     |   |        |   |
#### 5.4 Entradas.
n,.
#### 5.5 Salidas.
M.
### Ejercicio 6. OBTENER O GENERAR UNA MATRIZ CUADRADA DONDE LA DIAGONAL PRINCIPAL SEA LOS NUMEROS CONSECUTIVOS EMPEZANDO CON 1 Y EL RESTO SEA 0.
#### 6.1 Analisis. 
En el presente DFD se pretende realizar un logaritmo que rellene una matriz cuadrada con numeros 0, ecepto la diagonal principal, la diagonal principal tiene que tener numeros concecutivos emppezando con el numero 1.
#### 6.2 DFD
[![111.jpg](https://i.postimg.cc/tJjfbrCk/111.jpg)](https://postimg.cc/vg0XLtnx)
#### 6.3 Prueba de escritorio.
|matriz|i|j|j=i|m[i,j]=j+1   |j<matriz|j++|i<matriz|i++|
|------|-|-|---|-------------|--------|---|--------|---|
|2*2   |0|0|✓  |m[0,0]=1     |0<2     |1  |        |   |
|      |0|1|x  |m[0,1]=0     |1<2     |   |0<2     |1  |
|      |1|0|x  |m[1,0]=0     |0<2     |1  |1<2     |   |
|      |1|1|✓  |m[1,1]=1     |1<2     |   |        |   |
#### 6.4 Entradas.
Ninguna
#### 6.5 Salidas.
M[i,j]
### Ejercicio 7. 
[![12.jpg](https://i.postimg.cc/gkk1jZ4z/12.jpg)](https://postimg.cc/DmHxYmtH)
#### 7.1 Analisis. 
En el presente DFD se pretende realizar un logaritmo, para rellenar una matriz cuadrada con numeros consecutivos al cuadrado, despues convertir la matriz a un vector respetando los valores asignados.
#### 7.2 DFD
[![5.jpg](https://i.postimg.cc/4NgVQ6jG/5.jpg)](https://postimg.cc/mhmPbHbp)
#### 7.3 Prueba de escritorio.
|matriz|c     |i|j|m[i,j]=c*c   |c=c+1|j<matriz|j++|i<matriz|i++|i    |v[i]=c*c|i<2*2|i++|
|------|------|-|-|-------------|-----|--------|---|--------|---|-----|--------|-----|---|
|2*2   |1     |0|0|m[0,0]=1     |2    |0<2     |1  |0<2     |   |0    |v[0]=1  |0<4  |1  |
|      |2     |0|1|m[0,1]=4     |3    |1<2     |0  |0<2     |1  |1    |v[1]=4  |1<4  |2  |
|      |3     |1|0|m[1,0]=9     |4    |0<2     |1  |1<2     |   |2    |v[2]=9  |2<4  |3  |
|      |4     |1|1|m[1,1]=16    |     |1<2     |   |        |   |3    |v[3]=16 |3<4  |
#### 7.4 Entradas.
Ninguna
#### 7.5 Salidas.
M[i,j]
A[i]
### Ejercicio 8. EL 1°B QUIERE CONOCER EL PROMEDIO POR PERSONA Y POR MATERIA, ADEMAS DE LA MATERIA CON MEJOR PROMEDIO GRUPAL Y AL ALUMNO CON MEJOR PROMEDIO. SON 7 MATERIAS Y 32 ALUMNOS, MENCIONE LOS ALUMNOS EN RIESGO DE REPROBACION.

#### 8.1 Analisis. 
En el presente DFD se pretende realizar un logaritmo, para que el 1°B conozca el promedio que saco cada alumno, y el promedio que obtuvimos por materia, ademas la materia con mejor promedio y al alumno con mejor promedio, finalmente conocer los alumnos con rieso de reprobar.
#### 8.2 DFD
[![4.jpg](https://i.postimg.cc/7ZcLmDbz/4.jpg)](https://postimg.cc/18GP3kGR)
#### 8.3 Prueba de escritorio.
|corridas|i|j|M|j+1|
|-|-|-|-|-|
|1|0|0|M 0,0=Materia|j+1|
|2|0|1|M 0,1=Materia|j+1|
|3|0|2|M 0,2=Materia|j+1|
|4|0|3|M 0,3=Materia|j+1|

|Quimica|Matemáticas|Etica|Lengua materna|
|-|-|-|-|
|5|4|3|9|
|8|6|4|7|
|9|7|7|6|
|7|9|8|7|
#### 8.4 Entradas.
Ninguna
#### 8.5 Salidas.
VM[i],
VA[i],
AR.
### Ejercicio 9. PREGUNTAR LAS DIMENCIONES DE UNA MATRIZ, EL RANGO ES [5,5], VALIDA QUE SEA CUADRADA Y OBTENGA LA SUMA DE LA DIAGONAL PRINCIPAL Y LA  INVERSA, DETERMINE CUAL ES MAYOR.
#### 9.1 Analisis. 
En el presente DFD se pretende realizar un logaritmo para rellenar una una matriz cuadrada, donde la matriz tiene que ser cuadrada y no ser mayor de [5*5], para despues obtener la suma de la diagonal principal y de la diagonal inversa y decir cual es mayor.
#### 9.2 DFD
[![3.jpg](https://i.postimg.cc/XJ61KGbz/3.jpg)](https://postimg.cc/p9kBRdyf)
#### 9.3 Prueba de escritorio.
|matriz|dp|di|i|j|m[i,j]       |j<matriz|j++|i<matriz|i++|i|di=di+m[i,i]|i<matriz|i++|
|------|--|--|-|-|-------------|--------|---|--------|---|-|------------|--------|---|
|2*2   |0 |0 |0|0|m[0,0]=4     |0<2     |1  |        |   |0|0+4=4       |0<2     |1  |
|      |  |  |0|1|m[0,1]=5     |1<2     |   |0<2     |1  |1|4+7=11      |1<2     |   |
|      |  |  |1|0|m[1,0]=3     |0<2     |1  |1<2     |   |     
|      |  |  |1|1|m[1,1]=7     |1<2     |   |


|i|di=di+m[i,i]|i<matriz|i++|
|-|------------|--------|---|
|0|0+4=4       |0<2     |1  |
|1|4+7=11      |1<2     |   |

|i|j|i+j=matriz-1|di=di+m[i,j]|j<matriz|j++|i<matriz|i++|
|-|-|------------|------------|--------|---|--------|---|
|0|0|0+0=1 x     |            |0<2     |1  |
|0|1|0+1=1 ✓     |di=0+5      |1<2     |0  |0<2     |1|
|1|0|1+0=1 ✓     |di=5+3      |0<2     |1  |
|1|1|1+1=1 x     |

|dp<di|di es mayor|dp es mayor|
|-----|-----------|-----------|
|11<8 |x          |✓          |
#### 9.4 Entradas.
M[i,j]
#### 9.5 Salidas.
DP, DI


### Ejercicio 10. ALMACENAR EN UN ARRAY LA SUMA DE LOS NUMEROS DESDE 1 HASTA N, EN CADA POSICION DEL ARRAY. EJEMPLO: SI N=3, EL ARRAY DEBERIA SER 1,3,6.
#### 10.1 Analisis. 
En el presente DFD se pretende realizar un logaritmo, para almacenar en un array la sumatoria de los numeros consecutivos desde 1 hasta n en cada posicion de array, por ejemplo en la primea posicion ira el 1, en la segunda ira 1+2 que es 3, en la tercera ira 1+2+3 que es 6 y asi sucesivamente.
#### 10.2 DFD
[![1.jpg](https://i.postimg.cc/MGcBtdDs/1.jpg)](https://postimg.cc/DWTmwQRs)
#### 10.3 Prueba de escritorio.
|c|s|cuantos numeros|i|a[i]=s+c|s=s+c|c=c+1|i<numeros|i++|
|-|-|---------------|-|--------|-----|-----|---------|---|
|1|0|4              |0|a[0]=0+1|1    |2    |0<4      |1  |
|2|1|               |1|a[1]=1+2|3    |3    |1<4      |2  |
|3|3|               |2|a[2]=3+3|6    |4    |2<4      |3  |
|4|6|               |3|a[3]=4+6|10   |5    |3<4      |4  |

#### 10.4 Entradas.
Ninguna
#### 10.5 Salidas.
A[].
### Ejercicio 11. DADA UNA MATRIZ DE N*M ALMACENAR EN UN VECTOR LOS NUMEROS MAYORES POR RENGLON.
#### 11.1 Analisis. 
En el presente DFD se pretende realizar un logaritmo, donde dada una matriz ver que numero de cada renglon es mayor para almacenarlo en un vector.
#### 11.2 DFD
[![2.jpg](https://i.postimg.cc/gkR9fZzN/2.jpg)](https://postimg.cc/PPtFDN8w)
#### 11.3 Prueba de escritorio.
|mayor|renglones|columnas|matriz|i|j|m[i,j]  |mayor>m[i,j]|mayor=m[i,j]|j<c|j++|a[i]=mayor|i<r|i++|
|-----|---------|--------|------|-|-|--------|------------|------------|---|---|----------|---|---|
|0    |3        |2       |3*2   |0|0|m[0,0]=6|0>6 x       |mayor=6     |0<2|1  |
|     |         |        |      |0|1|m[0,1]=4|6>4 ✓       |            |1<2|0  |a[0]=6    |0<3|1  | 
|     |         |        |      |1|0|m[1,0]=5|0>5 x       |mayor=5      |0<2|1 |
|     |         |        |      |1|1|m[1,1]=7|5>7 x       |mayor=7      |1<2|0|a[1]=7      |1<3|2|
|     |         |        |      |2|0|m[2,0]=3|0>3 x       |mayor=3      |0<2|1|
|     |         |        |      |2|1|m[2,1]=1|3>1 ✓       |             |1<2| |a[2]=3


#### 11.4 Entradas.
Ninguna
#### 11.5 Salidas.
A[].
