# Simulador "Radio Alura" 🎧🎙️

## Descripción 
Radio Alura es una aplicación simple que simula una estación de radio virtual. 
Permite gestionar canciones y podcasts, 
así como llevar un registro de reproducciones y “Me gusta”.

## Características
Clases:
- **Audio**:
La clase Audio es la base para las canciones y los podcasts. 
Contiene los siguientes atributos:

*titulo*: El título del audio.
*totalDeReproducciones*: El número total de reproducciones.
*totalDeMeGusta*: La cantidad de veces que se marcó como “Me gusta”.
*clasificacion*: La clasificación del audio (calculada según ciertos criterios).
- **Cancion**:
La clase Cancion hereda de Audio y agrega los siguientes atributos:

*album*: El álbum al que pertenece la canción.
*cantante*: El cantante o banda que interpreta la canción.
*genero*: El género musical.
Además, sobrescribe el método getClasificacion() para asignar una clasificación basada en la cantidad de “Me gusta”.

- **Podcast**:
La clase Podcast también hereda de Audio y tiene los siguientes atributos adicionales:

*presentador*: El presentador o anfitrión del podcast.
*descripcion*: Una breve descripción del contenido del podcast.
Al igual que con las canciones, la clasificación se calcula según el número de reproducciones.

## Uso
En la clase Principal, se crean instancias de una canción y un podcast, 
se simulan reproducciones y “Me gusta”, y se muestran los totales. 
Además, se agrega el audio a la lista de favoritos.
