# Introducción a la versión en español

Esta traducción incluye todos los capítulos de la obra "Platform Design" compartidos a través del [repositorio de Github de la misma](https://github.com/dcuartielles/platform-design) , pero no constituyen la obra completa.

Tal y como se puede leer en el fichero README.md del repositorio original, estos capítulos corresponden a una versión de pre-impresión y no incluyen índice actualizado, sección de agradecimientos, imágenes e incluso alguna errata en las referencias, aunque no se hace explícito a que referencia se refiere, por lo que no se ha podido corregir.

El texto original de la tesis incluye en los anexos las obras incluidas en la compilación, que suman más de 300 páginas adicionales. De las 517 páginas que componen la tesis, la traducción en español sólo cubre el texto principal, que supone unas 200 páginas aproximadamente. Recomendamos encarecidamente consultar el texto completo con ilustraciones y anexos en el PDF incluido en el [repositorio original](https://github.com/dcuartielles/platform-design/blob/master/201809_Cuartielles_Thesis_Platform-Design_web.pdf)

## Proceso de traducción

La traducción de esta obra partió de los esfuerzos previos de otros traductores, que comenzaron con la introducción y el primer capítulo. Una vez se observó el ritmo de progreso y el tiempo disponible para la misma, se optó por utilizar un servicio de traducción online (Deepl) para generar una versión inicial completa.

Dicha traducción ha sido revisada manualmente para revisar todos los términos técnicos, mantener la coherencia entre los distintos capítulos, preservar el formato de la obra y garantizar que el resultado final es legible en castellano. La obra original emplea un lenguaje académico bastante denso, cuyo estilo se ha intentado preservar tras la traducción, aunque determinadas oraciones resultantes tengan una longitud y complejidad elevada.

En el caso de las traducciones previas, se han revisado también, eliminándose referencias que no existían en la obra original y armonizando los términos con los empleados en el resto de la obra.

El texto original en inglés en formato markdown estaba ajustado a un ancho de columna fijo, de cara a la maquetación final. Esto hizo que el servicio de traducción creara en ocasiones fragmentos duplicados, al encontrarse con frases separadas de forma arbitraria. Se ha intentado eliminar dichos duplicados durante el proceso de revisión, pero es posible que perduren algunos elementos. Dada la naturaleza abierta del proyecto, se anima al lector a remitir sus correciones a través de Github, enviando los propios cambios a los textos o avisando a través del sistema de Issues.

## Adenda técnica

La versión en PDF de la obra en español se ha generado utilizando los siguientes comandos:

```
pandoc Notas_a_la_traducción.md -s -o notas.pdf --pdf-engine=xelatex
pandoc v0002-ch00.md -s -o v0002-ch00.pdf --pdf-engine=xelatex
pandoc v0002-ch01.md -s -o v0002-ch01.pdf --pdf-engine=xelatex
pandoc v0002-ch02.md -s -o v0002-ch02.pdf --pdf-engine=xelatex
pandoc v0002-ch03.md -s -o v0002-ch03.pdf --pdf-engine=xelatex
pandoc v0002-ch04.md -s -o v0002-ch04.pdf --pdf-engine=xelatex
pandoc v0002-ch05.md -s -o v0002-ch05.pdf --pdf-engine=xelatex
pandoc v0002-ch06.md -s -o v0002-ch06.pdf --pdf-engine=xelatex
convert diy_cover.png diy_cover.pdf
pdfunite diy_cover.pdf notas.pdf v0002-ch00.pdf v0002-ch01.pdf  \ 
v0002-ch02.pdf v0002-ch03.pdf v0002-ch04.pdf v0002-ch05.pdf \
v0002-ch06.pdf 202310_Cuartielles_Tesis_Diseño_de_Plataformas_web.pdf
```

Para replicar estos comandos es necesario disponer de las pandoc, ImageMagick y poppler (que ofrece pdfunite).


## Colofón
Esta traducción original se ha completado a día 18 de Octubre de 2023 a las 13:30, en el quinto aniversario de la defensa de la tésis en la Universidad de Malmö

Traductor: César García Sáez
