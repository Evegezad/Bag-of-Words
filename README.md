# Bag of Words

## Introducción

**Bag of words (BoW)** es una técnica importante en el [procesamiento del lenguaje natural] (https://surface.syr.edu/cgi/viewcontent.cgi?referer=https://scholar.google.com.mx/&httpsredir=1&article=1019&context=cnlp) y en la [recuperación de información] (https://nlp.stanford.edu/IR-book/pdf/01bool.pdf). BoW utiliza vectores de frecuencia de términos para representar el contenido de documentos de texto, lo que hace posible el uso de programas matemáticos y de computadora para analizar y comparar documentos de texto.

BoW contiene la siguiente información:

1. Un diccionario de todos los términos (palabras) en los documentos de texto. Los términos se normalizan en términos de mayúsculas y minúsculas (por ejemplo, `México` => `méxico`), tiempo (por ejemplo, `had` => `have`), forma singular (por ejemplo, `students` => `student`), etc.
2. El número de ocurrencias de cada término normalizado en cada documento.

Por ejemplo, supongamos que tenemos tres documentos de texto:

DOC 1: CDMX es la capital de México.

DOC 2: Me encanta México.

DOC 3: Soy estudiante en UPIITA.

El BoW de los documentos anteriores se ve a continuación:

| TÉRMINO | DOC 1 | DOC 2 | DOC 3 |
|---|---|---|---|
| CDMX | 1 | 0 | 0 |
| es | 1 | 0 | 0 |
| la | 1 | 0 | 0 |
| capital | 1 | 0 | 0 |
| de | 1 | 0 | 0 |
| México | 1 | 1 | 0 |
| Me | 0 | 1 | 0 |
| encanta | 0 | 1 | 0 |
| Soy | 0 | 0 | 1 |
| estudiante | 0 | 0 | 1 |
| en | 0 | 0 | 1 |
| UPIITA | 0 | 0 | 1 |
