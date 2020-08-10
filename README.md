# IIC2133 - Estructuras de Datos y Algoritmos
## 2020-2

Bienvenido al sitio web del curso de Estructuras de Datos y Algoritmos. En esta página podrás encontrar la información administrativa del curso. En el repositorio podrás encontrar código ya preparado por tus ayudantes, junto con los eventuales enunciados de las tareas y las diapositivas de clases.

## Tabla de contenidos
 * [Equipo](#equipo)
     * [Profesores](#profesores)
     * [Ayudantes](#ayudantes)
 * [Evaluaciones](#evaluaciones)
     
## Equipo

### Profesores

| Nombre               |  Sección         |  Email         |
|:-------------------- |:--------------|:--------------|
| Yadran Eterovic | 1,2 | yadran@ing.puc.cl |


### Ayudantes

| Nombre                | Email       | Github |
|:--------------------- |:-------------| :---------|
| Vicente Errázuriz | verrazuriz@uc.cl | [@vichoeq](https://www.github.com/vichoeq) |
| Cristóbal Espinoza | caespinoza5@uc.cl | [@caespinoza5](https://www.github.com/caespinoza5) |
| Yerko Chávez | yachavez@uc.cl | [@yerkko](https://www.github.com/yerkko) |
| Nicolás Lahsen | nflahsen@uc.cl | [@NicolasLahsen](https://www.github.com/NicolasLahsen) |
| Luciano Aguilera | lbaguilera@uc.cl | [@arbiocanpion](https://www.github.com/arbiocanpion) |
| Benjamín Domínguez | bidominguez@uc.cl | [@B-Dominguez](https://www.github.com/B-Dominguez) |
| Brayan Moreno | bbmoreno@uc.cl | [@brayanmoreno](https://www.github.com/brayanmoreno) |
| Florencia Ferrer | fpferrer@uc.cl | [@fpferrer](https://www.github.com/fpferrer) |
| Paula Yoma | pbyoma@uc.cl | [@pbyoma](https://www.github.com/pbyoma) |
| Kristine Droppelmann | kkdroppelmann@uc.cl | [@kdroppelmann](https://www.github.com/kdroppelmann) |
| Federico Hurtado | fthurtado@uc.cl | [@fthurtado](https://www.github.com/fthurtado) |
| Trinidad Vargas | mtvargas1@uc.cl | [@TrinidadVargas](https://www.github.com/TrinidadVargas) |
| Cristóbal Jones | cjones2@uc.cl | [@cjones27](https://www.github.com/cjones27) |
| Ignacio Zúñiga | inzuniga@uc.cl | [@inzuniga](https://www.github.com/inzuniga) |
| Ian Fieldhouse | ifieldhouse@uc.cl | [@ifieldhouse](https://www.github.com/ifieldhouse) |
| Diego Campos | dacampos1@uc.cl | [@dacampos](https://www.github.com/dacampos) |
| Matías Quezada | moquezada@uc.cl | [@moquezada](https://www.github.com/moquezada) |
| Kyle Bossonney | kbossonney1@uc.cl | [@kylevon](https://www.github.com/kylevon) |
| Manuel Munoz | mimunoz11@uc.cl | [@mimunoz11](https://www.github.com/mimunoz11) |
| Lothar Droppelmann | ldroppelmann@uc.cl | [@lothardp](https://www.github.com/lothardp) |
| Jacques Hasard | jnhasard@uc.cl | [@jnhasard](https://www.github.com/jnhasard) |

## Evaluaciones

El curso consta de una parte teórica, evaluada mediante evaluaciones escritas (interrogaciones), y una parte práctica, evaluada mediante tareas de programación en C.

### Evaluaciones Escritas

Habrá 3 interrogaciones, donde se evaluarán los aspectos más teóricos del contenido. Las interrogaciones serán subidas a las 14.00 del día de evaluación, con entrega hasta las 23.59 del mismo día. Cada interrogación tendrá 4 preguntas, de las cuales el alumno debe elegir 3 a contestar. Las interrogaciones están pensadas para ser contestadas en menos de 2 horas cada una. La nota de interrogaciones será el promedio de las 3 interrogaciones.

| Evaluación | Fecha |
|:----------|:----------|
| Interrogación 1 | 5 de octubre |
| Interrogación 2 | 16 de noviembre |
| Interrogación 3 | 11 de diciembre |


### Tareas

Habrá 5 tareas de programación en C, donde deberán resolver un problema complejo y analizarlo en un informe escrito. Las fechas a continuación son tentativas y están sujetas a cambios.

| Evaluación | Fecha de anuncio | Fecha de entrega |
|:----------|:----------|:----------|
| Tarea 0 | 12 de agosto | 29 de agosto|
| Tarea 1 | 31 de agosto | 14 de septiembre |
| Tarea 2 | 7 de octubre | 22 de octubre |
| Tarea 3 | 26 de octubre | 10 de noviembre |
| Tarea 4 | 17 de noviembre | 1 de diciembre |

La nota final del curso se calcula de la siguiente manera:

```c++
double nota_final()
{
    /* La nota de cada tarea */
    double T0,T1,T2,T3,T4;    
    /* La nota de cada interrogación*/
    double I1,I2,I3;

    /* Promedio de tareas */
    double NT = (T0 + T1 + T2 + T3 + T4) / 5;
    /* Promedio de interrogaciones */
    double NI = (I1 + I2 + I3) / 3;
    
    /* Nota final */
    double NF = (NT + NI) / 2;
    
    /* Es necesario tener sobre 3.7 en las evaluaciones escritas y las tareas por separado para aprobar el curso */
    if(NI < 3.7 || NT < 3.7)
    {
       return min(3.9, NF);
    }
    else
    {
       return min(NF, 7);
    }
}
```
