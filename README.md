# APUNTES M4 #

## Minidom ##
_¿Qué es?_

DOM es un modelo de manipulación de objetos de un documento que te permite acceder al contenido de un documento teniendo en cuenta una estructura de _arbol_. DOM te permite *acceder, cambiar, añadir o borrar* elementos del documento.

### Propiedades
1. x.nodeName --> Nombre de X
2. x.nodeValue --> Valor de X
3. x.getElementsByTagName("name)--> Saca todos los elementos que se llamen como el nombre que se ha especificado. 

### Acceder a nodos
Se puede acceder a todos los nodos del documento usando las relaciones del árbol de nodos o usando *getElementsByTagName()*.

>nodo.getElementsByTagname("titulo") 
> Devolverá todos los elementos <titulo> que haya dentro del nodo 'nodo'
---
 Se puede crear una lista guardando la lista que getElementsByTagName() te devuelve en una variable, a la que puedes acceder mas tarde mediante índices.

### Propiedades de los nodos

Cada nodo es un objeto que cuenta con propiedades como:
* NodeName: Especifica el nombre de un nodo y es una propiedad read only. El NodeName es, grosso modo, la etiqueta, y si hablamos de un nodo de texto, siempre será texto. 
* NodeValue: Especifica el valor de un nodo. Para los nodos elemento está indefinido mientras que para los nodos de texto es el propio texto.
* NodeType: Especifica el tipo de nodo, por ejemplo, _elemento, atributo, texto, comentario o documento_

### Lista de nodos
Cuando usas propiedades como *childnodes* o *getElementsByTagName* obtienes una lista de nodos, ordenada como está en el xml. Al ser una lista puedes acceder a ella mediante índices.  

## XPATH
XPATH es un elemento básico del estándar xsl, en el cual encontramos nodos que se relacionan entre sí. Tenemos varios tipos de nodo, como pueden ser *elementos*, *atributos* o *texto*. Entre ellos también se encuentra el nodo raiz. 

Todos los elementos y atributos tienen un elemento padre, que  a su vez puede tener varios hijos. Cuando dos o más nodos comparten elemento padre decimos que son _hermanos_.

##