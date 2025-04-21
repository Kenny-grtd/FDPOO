🧩 Explicación del código
Clase Juego:
Es la clase base de donde heredan tanto el Jugador como el Enemigo.

Tiene los atributos:

nombre: el nombre del personaje.

posición: una tupla (x, y) que indica dónde está en el escenario.

Tiene un método mover() para cambiar la posición del objeto.

Clase Poder:
Representa los poderes especiales del juego.

Tiene:

nombre: como “Estrella” o “Flor de fuego”.

descripción: explica qué hace ese poder.

Se usa para asignar habilidades especiales al jugador.

Se puede mostrar como texto gracias al método _str_().

Clase Jugador:
Hereda de la clase Juego.

Tiene:

vida: cantidad de vidas del jugador.

poderes: una lista de poderes que puede ir ganando.

Métodos:

agregar_poder(): agrega un nuevo poder al jugador.

_str_(): muestra la información completa del jugador (nombre, posición, vida y poderes).

Clase Enemigo:
También hereda de Juego.

Tiene un atributo adicional:

tipo: indica el tipo de enemigo (por ejemplo: “Goomba”, “Koopa Troopa”, “Planta Piraña”).

Usa _str_() para mostrar fácilmente su información.

🎮 Programa principal:
Crea un jugador Mario con 3 vidas y posición inicial (0, 0).

Se le asignan 2 poderes:

“Estrella”: da inmunidad temporal.

“Flor de fuego”: permite lanzar fuego.

Se crean 3 enemigos:

Goomba

Koopa Troopa

Planta Piraña

Mario se mueve a la posición (3, 1).

Finalmente, se muestra en pantalla:

La información del jugador.

La lista de enemigos con sus posiciones y tipos.
