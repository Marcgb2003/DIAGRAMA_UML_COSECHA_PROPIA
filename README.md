Tenemos un juego tipo rpg por turnos, en el que tenemos las clases Combate, Protagonista, Compañeros, Enemigos, Personaje, Equipamiento, Objetos e Invocaciones.

La clase Combate, que va relacionada con protagonista, compañeros y enemigos, tiene un atributo Timer que indica el retraso hasta la siguiente acción, un atributo localización de tipo string, que sería la dirección del archivo de imagen usado como fondo, un booleano llamado final y un atributo time de tipo int, que se usará para calcular la luz. Sus métodos serán un constructor con 1 protagonista, 1 array de compañeros y un array de enemigos, que será donde se genere la batalla, el método turno, que  es donde se invocan los ataques, el uso de objetos y el método vic_or_der, que muestra la pantalla de victoria y derrota dependiendo de cómo haya acabado la batalla, y si es victoria, da los objetos a los ganadores.

La clase Personaje tiene el String nombre, un int llamado nivel, un booleano llamado KO(es decir, si el personaje está KO en el combate o no), un int ataque, un int velocidad, un int defensa, un int vida, un int magia, un int llamado exp, un array de Equipamiento llamado equipo, un array de Objetos llamado inventario y un array de Invocaciones. Además tiene los Setters y Getters correspondientes y el método calcNivel, que recibe exp y nivel.

La clase Protagonista, que hereda de personaje, tiene el booleano gender, ya que este puede cambiar a lo largo del juego, y el booleano revivido, que viene de la historia y modifica su aspecto.

La clase Compañeros, que hereda de Personaje tiene el booleano gender, el booleano liz, que determina si su especie es Lizarca o no, el booleano caido, que indica si es un caído, es decir, un no muerto, y el int relación, que indica la relación con el protagonista del 1 al 10. 

La clase Enemigos, que hereda de Personaje, tiene el booleano animal, el Objeto drop y el int exp_given. 

La clase Equipamiento tiene el string nombre, el int plus_vel, el int plus_def, el int plus_atq, el int plus_vid, el int plus_mag, el int nivel y el int precio. 

La clase Objetos tiene el string nombre, el int efecto y el enum tipo, que tiene los tipos curacion, dano, recuperacion y  revivir. Además tiene el método cura, el método dano, el método recu y el método revivir.

La clase Invocaciones tiene los atributos coste, de tipo int, un int llamado efecto y un enum llamado tipo que tiene los valores dano, recuperacion, protección, curacion y revivir. A su vez tiene los métodos cura, dano, recu, prot y revi.
