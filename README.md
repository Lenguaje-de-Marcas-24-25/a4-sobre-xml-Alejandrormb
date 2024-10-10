[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/fGeLcsqO)
# A5-SOBRE-XML5
## 1. Indica las características propias del lenguaje XML.
- Extensible: Permite crear etiquetas personalizadas.
- Legible: Fácil de entender tanto para humanos como para máquinas.
- Estructurado: Define la jerarquía y la relación entre elementos.
- Multiplataforma: Se puede usar en diferentes sistemas y aplicaciones.
- Separa contenido de presentación: A diferencia de HTML, XML no define cómo se debe mostrar la información.

## 2. Identifica la estructura de un documento XML y sus reglas sintácticas.
- Declaración: Siempre comienza con ``<xml version="1.0" encoding="UTF-8">``.
- Nodo raíz: Debe haber un único nodo raíz que contenga todos los elementos.
- Etiquetas abiertas y cerradas: Todo elemento debe tener una etiqueta de apertura y una de cierre o ser un elemento vacío.
- Sensibilidad a mayúsculas: ``<nombre>`` es distinto de ``<Nombre>``.
- Atributos entre comillas: Los valores de los atributos deben estar entre comillas (" " o ' ').

## 3. En XML qué es un nodo raíz
El *nodo raíz* es el elemento que contiene todos los demás elementos del documento XML. Solo puede haber uno por documento.

## 4. Indica qué es un elemento vacío. Ejemplos
Un elemento vacío es un elemento que no contiene contenido ni elementos hijos, se cierra en la misma etiqueta de apertura. Ejemplo: ``< br/>, <img src="image.png" />``.
## 5. Qué sentido tiene crear documentos XML bien formado.
Un documento bien formado sigue estrictamente las reglas de sintaxis de XML, lo que asegura que pueda ser interpretado correctamente por los parsers XML, facilitando su intercambio entre sistemas.

## 6. Qué es un espacio de nombres. Ventajas de uso.
Un espacio de nombres es un identificador único que se usa para evitar conflictos de nombres entre elementos que pueden tener el mismo nombre pero diferentes propósitos. Se define usando el prefijo ``xmlns``
Ventajas:
- Evita colisiones de nombres.
- Facilita la interoperabilidad entre distintos esquemas XML.

## 7. Entidades en XML. Crea un XML con las entidades vistas en clase.
Las entidades son secuencias de caracteres que se representan de manera especial en XML.
```
<?xml version="1.0" encoding="UTF-8"?>
<mensaje>
    El símbolo menor que es &lt; y el mayor que es &gt;.
</mensaje>
```


## 8. Comentarios en XML. Muestra uno de los ejercicios anteriores con el enunciado dentro de un comentario. Dentro del comentario deben aparecer dos guiones.
```
<!--Este es el ejercicio número Vencimiento de UD1 A6. Repaso tipo examen-->
<?xml version="1.0" encoding="UTF-8"?>
<!-- Carta del restaurante "Grande es el Capitán" -->
<restaurante nombre="Grande es el Capitán">

    <contacto>
        <telefono>678123456</telefono>
        <telefono>957224466</telefono>
        <telefono>957987654</telefono>
    </contacto>
    
    <platos>
        <plato tipo="primer">
            <nombre>Croquetas de jamón ibérico</nombre>
            <alergenos>
                <alergeno>Gluten</alergeno>
                <alergeno>Huevos</alergeno>
                <alergeno>Lácteos</alergeno>
            </alergenos>
            <precios>
                <media_racion precio="8" />
                <racion precio="11" />
            </precios>
            <valor_energetico>149 Kcal (1 croqueta, 85g)</valor_energetico>
        </plato>
        
        <plato tipo="segundo">
            <nombre>Gazpacho andaluz</nombre>
            <alergenos>
                <alergeno>Gluten</alergeno>
            </alergenos>
            <precios>
                <vaso precio="4" />
            </precios>
            <valor_energetico>63 Kcal (100g)</valor_energetico>
        </plato>
        
        <plato tipo="tercer">
            <nombre>Rabo de toro</nombre>
            <alergenos>
                <alergeno>Gluten</alergeno>
                <alergeno>Lácteos</alergeno>
                <alergeno>Sulfitos</alergeno>
            </alergenos>
            <precios>
                <racion precio="13" />
            </precios>
            <valor_energetico>217 Kcal (100g)</valor_energetico>
        </plato>
    </platos>
    
    <!-- Elemento vacío -->
    <nota><!-- vacío --></nota>
</restaurante>
```
