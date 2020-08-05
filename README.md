# IIC2133 - Estructuras de Datos y Algoritmos
## 2020-2

Bienvenido al sitio web del curso de Estructuras de Datos y Algoritmos. En esta página podrás encontrar la información administrativa del curso. En el repositorio podrás encontrar código ya preparado por tus ayudantes, junto con los eventuales enunciados de las tareas y las diapositivas de clases.

## Tabla de contenidos
 * [Equipo](#equipo)
     * [Profesores](#profesores)
     * [Ayudantes](#ayudantes)
 * [Acerca del curso](#acerca-del-curso) 
 * [Contenidos](#contenidos)
 * [Política de Integridad Académica](#política-de-integridad-académica)

## Acerca del curso

Este curso enseña a analizar problemas, descomponerlos y elaborar algoritmos que los resuelvan en un tiempo óptimo. Esto se logra mediante la organización de la información en estructuras de datos y el uso de algoritmos capaces de aprovechar dichas estructuras. En particular se enseñan problemas de optimización en grafos, métodos de ordenación, y estructuración de la información en diccionarios.

El curso utiliza el lenguaje de programación C, ya que éste permite trabajar directa y limpiamente con los algoritmos aprendidos. Dado que este lenguaje trabaja en bajo nivel, se puede lograr escribir un programa que resuelva los problemas en tiempo óptimo no solo en la teoría, si no también en la práctica.
     
## Equipo

### Profesores

| Nombre               |  Sección         |  Email         |
|:-------------------- |:--------------|:--------------|
| Yadran Eterovic | 1 | yadran@ing.puc.cl |


### Ayudantes

| Nombre                | Email       | Github |
|:--------------------- |:-------------| :---------|
| Vicente Errázuriz | verrazuriz@uc.cl | vichoeq |
| Cristóbal Espinoza | caespinoza5@uc.cl | caespinoza5 |
| Yerko Chávez | yachavez@uc.cl | yerkko |
| Nicolás Lahsen | nflahsen@uc.cl | NicolasLahsen |
| Luciano Aguilera | lbaguilera@uc.cl | arbiocanpion |
| Brayan Moreno | bbmoreno@uc.cl | brayanmoreno |
| Florencia Ferrer | fpferrer@uc.cl | fpferrer |
| Paula Yoma | pbyoma@uc.cl | pbyoma |
| Kristine Droppelmann | kkdroppelmann@uc.cl | kdroppelmann |
| Federico Hurtado | fthurtado@uc.cl | fthurtado |
| Trinidad Vargas | mtvargas1@uc.cl | TrinidadVargas |
| Cristóbal Jones | cjones2@uc.cl | cjones27 |
| Ignacio Zúñiga | inzuniga@uc.cl | inizuniga |
| Ian Fieldhouse | ifieldhouse@uc.cl | ifieldhouse |
| Diego Campos | dacampos1@uc.cl | dacampos |
| Matías Quezada | moquezada@uc.cl | moquezada |
| Kyle Bossonney | kbossonney1@uc.cl | kylevon |
| Manuel Munoz | mimunoz11@uc.cl | mimunoz11 |


## Contenidos

A continuación se presentan los contenidos del curso, no necesariamente en el orden en que serán impartidos.

* Estructuras elementales
 * Listas y colas LIFO y FIFO.
 * Heaps binarios.
* Diccionarios
 * Tablas de hash
 * Árboles de búsqueda
* Algoritmos
 * Ordenación
      * Ingenua ( *O*(n<sup>2</sup>) )
      * Inteligente ( *O*(n log(n)) )
      * Especializada ( *O*(n) )
 * Optimización en grafos
      * Orden Topológico
      * Cobertura
      * Búsqueda
      * Flujo
 * Técnicas Algorítmicas
      * Dividir y conquistar
      * Algoritmos Codiciosos
      * Programación Dinámica
      * Backtracking
* Strings

## Evaluación

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
| Tarea 0 | 12 de agosto | 26 de agosto|
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

## Política de integridad académica

Este curso se adscribe a la política de integridad académica de la Escuela de Ingeniería y el Departamento de Computación.

---

Los alumnos de la Escuela de Ingeniería de la Pontificia Universidad Católica de Chile deben mantener un comportamiento acorde a la Declaración de Principios de la Universidad.  En particular, se espera que **mantengan altos estándares de honestidad académica**.  Cualquier acto deshonesto o fraude académico está prohibido; los alumnos que incurran en este tipo de acciones se exponen a un Procedimiento Sumario. Es responsabilidad de cada alumno conocer y respetar el documento sobre Integridad Académica publicado por la Dirección de Docencia de la Escuela de Ingeniería (disponible en SIDING).

Específicamente, para los cursos del Departamento de Ciencia de la Computación, rige obligatoriamente la siguiente política de integridad académica. Todo trabajo presentado por un alumno para los efectos de la evaluación de un curso debe ser hecho individualmente por el alumno, sin apoyo en material de terceros.  Por “trabajo” se entiende en general las interrogaciones escritas, las tareas de programación u otras, los trabajos de laboratorio, los proyectos, el examen, entre otros.

**En particular, si un alumno copia un trabajo, o si a un alumno se le prueba que compró o intentó comprar un trabajo, obtendrá nota final 1.1 en el curso y se solicitará a la Dirección de Docencia de la Escuela de Ingeniería que no le permita retirar el curso de la carga académica semestral.**

Por “copia” se entiende incluir en el trabajo presentado como propio, partes hechas por otra persona.  **En caso que corresponda a “copia” a otros alumnos, la sanción anterior se aplicará a todos los involucrados**.  En todos los casos, se informará a la Dirección de Docencia de la Escuela de Ingeniería para que tome sanciones adicionales si lo estima conveniente. Obviamente, está permitido usar material disponible públicamente, por ejemplo, libros o contenidos tomados de Internet, siempre y cuando se incluya la referencia correspondiente y sea autorizado por los ayudantes.

Lo anterior se entiende como complemento al Reglamento del Alumno de la Pontificia Universidad Católica de 
Chile<sup><a name="pucCLBack">[1](#pucCL)</a></sup>.  Por ello, es posible pedir a la Universidad la aplicación de sanciones adicionales especificadas en dicho reglamento.

<sub>**<a name="pucCL">[1](#pucCL)</a>**: Reglamento del Alumno de la Pontificia Universidad Católica de Chile disponible en: http://admisionyregistros.uc.cl/alumnos/informacion-academica/reglamentos-estudiantiles [&#8593;](#pucCLBack)</sub>
