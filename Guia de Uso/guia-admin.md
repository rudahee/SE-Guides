# Guia para moderacion ¡Hay comandos que cambiar, Por causa del lag!
---

### Funciones y Comandos para Helper

#### **Funciones**
El helper es un rango que tiene permisos basicos, este rango permite realizar ciertos asuntos, como asignar rangos de patreons, crear hologramas, o ayudar a otros miembros que tengan problemas.
Tienen permisos para kickear y mutear, y aunque a veces tengan que personarse en un sitio (y para ello tienen tps/godmode/fly) deben estar atentos al chat para ayudar en las dudas que puedan surgir con respecto a los mods/plugins y el funcionamiento del servidor.

Tambien son las personas que deben ayudar a los nuevos miembros si tienen dudas.

La gran mayoria de sus comandos, son para calidad de vida, y poder ayudar a otros jugadores.

Pueden sobrepasar las protecciones de parcelas. 

#### **Comandos**

* Holographic Display (Para poner holograma aka texto flotante):

```js
/hd create <nombre> <texto>                     -> CREA UN TEXTO FLOTANTE
/hd moveHere <nombre>                           -> LO MUEVE A TUS PIES
/hd addLine <nombre> <texto>                    -> AGREGA UNA LINEA
/hd setLine <nombre> <numero de linea> <texto>  -> SETEA UNA LINEA ESPECIFICA
/hd remove <nombre>                             -> BORRA UN HOLOGRAMA
/hd list                                        -> LISTA TODOS LOS HOLOGRAMAS
/hd teleport <nombre>                           -> TP A UN HOLOGRAMA
```

* Worldguard
```js
/rg bypass                                      -> TE PERMITE SOBREPASAR LAS PROTECCIONES
/wg reload                                      -> TE PERMITE RECARGA LA CONFIGURACION (Por si un rango no se aplico correctamente, o no le dio los permisos en una parcela, etc...)
```

* Metallics Arts
```js
/ma-items get <item> <usuario>                      -> DA UN ITEM CARGADO DE LA ALOMANCIA 
/ma-powers [add|get|remove] <poder/es> <usuario>    -> MODIFICA PODERES DE ALGUIEN
```

* Minecraft
```js
/tp                                                 -> TE TELETRANSPORTAS A OTRO JUGADOR
/gamemode                                           -> CAMBIA TU MODO DE JUEGO O EL DE OTROS
/give                                               -> TE DA UN ITEM
/kill                                               -> MATAS A ALGUIEN
/minecraft:tp                                       -> TE PEGAS UN TP
/minecraft:give                                     -> DA UN ITEM
/god                                                -> NO PUEDES MORIR
/heal                                               -> TE CURAS LA VIDA Y EL HAMBRE
/fly                                                -> TE DA VOLAR
/kick <jugador> <razon>                             -> ECHAS A ALGUIEN (PON UN MOTIVO)
/mute <jugador> <tiempo> <motivo>                   -> MUTEAS A ALGUIEN UN TIEMPO (PON UN MOTIVO)
/weather                                            -> CAMBIA EL TIEMPO
/summon                                             -> INVOCA UNA ENTIDAD
```
---

### Funciones y Comandos para Mod

#### **Funciones**
Son los miembros con mayores permisos de moderacion antes de los admins. Su funcion principal, es mantener el orden en el servidor y ayudar a que todo funcione correctamente, Ademas de todas las funciones de los helpers, son los encargados de asignar parcelas, bases y teams. Este rango es el que debe controlar que los jugadores construyan sus bases donde tocan, que no partan nada, que no usen hacks, que no abusen de bugs, etc... **Este es el rango que esta obligado a moderar antes que jugar**, Si se incumple una de las reglas, en este caso pueden banear. Opcionalmente, pueden tener acceso al SocialSpy

Pueden banear, y ver a los baneados, entrar en modo incognito, y hacer tps masivos.

#### **Comandos**

Minecraft
```js
/team                                               -> CREA UN TEAM PARA QUE PUEDAN MANDAR MENSAJES (SOLO SI LO PIDEN)
/ban                                                -> QUITAS EL ACCESO A UNA PERSONA PARA SIEMPRE O DE FORMA TEMPORAL
/banlist                                            -> LISTA DE BANEADOS
/vanish                                             -> INVISIBLE
/tpaall                                             -> PREGUNTA A TODOS PARA TEPEAR A TU POS
/tpall                                              -> TPA A TODOS, SIN PREGUNTAR, A TU POSICION
```


LuckPerms
```js
/lp user <usuario> meta clear                       -> QUITAR LOS PREFIJOS
/lp user <usuario> meta addprefix 100 "<prefijo>"   -> PONER UN PREFIJO = GUIA PARA COPYPASTE -> "&4&lNOMBRE&r&l| "
```
 
WorldGuard//WorldEdit
```
//expand vert                                       -> EXPANDE DESDE BEDROCK A LA ALTURA MAX UNA SELECCION
```
```js
/rg define <nombre>                                 -> CREA UNA REGION (PARCELA = parcela-RuDaHee, BASE = base-URSS. asi se pueden localizar facil)
/rg remove <nombre>                                 -> ELIMINA UNA REGION
/rg list                                            -> MUESTRA LA LISTA INTERACTIVA DE PARCELAS
/rg info <nombre>                                   -> MUESTRA LA INFORMACION DE UNA PARCELA
/rg setpriority -w "Scadrial" <nombre-parcela> 20   -> DA UNA PRIORIDAD SUPERIOR A ELENDEL EN UNA PARCELA
```
---

### Funciones y Comandos para Admin

#### **Funciones**
Ademas de todas las funciones de mod y helper (Y despidete de jugar), es el unico rango con acceso a la consola. los admins a diferencia de los mods, pueden hacer backups, apagar el servidor, ponerlo en modo mantenimiento, ver los logs, cambiar plugins, y todo lo que conlleva la propia administracion del servidor fuera del juego. (Esto no es necesariamente comprender como funciona todo al detalle, pero si estar pendiente que no haya errores en consola, y que el servidor funcione lo mas estable posible).

Tiene todos los permisos de worldguard, y pueden acceder a la web de luckperms desde la consola, asi como resetar la contraseña de otros miembros si se les olvida.

Tambien, son los unicos que pueden banear por ip y pueden desbanear, y controlar las tiendas de otros jugadores. Ademas, tienen acceso completo al SocialSpy en el propio juego. Asi como a las herramientas para comprobar el funcionamiento (lag, tps, etc..) del propio servidor.

En momentos puntuales pueden poner/quitar bloques de comando, realizando el op/deop desde la consola.

#### **Comandos desde el juego**

```js
/ban-ip
/unban
/unban-ip
/maintenance
/rg (Todos)
/save-all
/socialspy
/timings (Todos)
/spark (Todos)
/ishop (Todos)
```

### **Comandos desde la consola**
```js
/unregister <nombre>
/lp editor
```

---

### GUIAS

**CREAR PARCELA**

1. Selecciona el area con el hacha de madera (si es una parcela, desde dentro de las slabs)
2. expandes del cielo a la bedrock con `//expand vert`
3. creas la region con `/rg define <nombre>`
4. le asignas un dueño: `/rg addowner -w "Scadrial" <nombre-parcela> <usuario>`
5. Si es necesario, le agregas miembros con: `/rg addmember -w "Scadrial" <nombre-parcela> <usuario>`
6. Para finalizar le asignas una prioridad por defecto `/rg setpriority -w "Scadrial" <nombre-parcela> 20`

**CREAR BASE**

1. Selecciona el area con el hacha de madera (si es una parcela, desde dentro de las slabs)
2. expandes del cielo a la bedrock con `//expand vert`
3. creas la region con `/rg define <nombre>`
4. le asignas un dueño: `/rg addowner -w "Scadrial" <nombre-parcela> <usuario>`
5. Si es necesario, le agregas miembros con: `/rg addmember -w "Scadrial" <nombre-parcela> <usuario>`
6. Se le asigna una prioridad por defecto `/rg setpriority -w "Scadrial" <nombre-parcela> 20`
7. Se establecen las siguientes flags:
-`/rg flag -w "Scadrial" base-<nombre> sleep allow`
-`/rg flag -w "Scadrial" base-<nombre> pvp allow`
-`/rg flag -w "Scadrial" base-<nombre> tnt deny`
-`/rg flag -w "Scadrial" base-<nombre> greeting &5mensaje &lde entrada` <- Admite codigos de color
-`/rg flag -w "Scadrial" base-<nombre> farewell &5mensaje &lde salida` <- Admite codigos de color


**CREAR UN TEAM**
1. A cada miembo le pones un prefijo con: `/lp user <usuario> meta addprefix 100 "<prefijo>"`
2. Si te piden tener chat de equipo, creas un team con `/team add <nombre-team>`
3. Para finalizar agregas a los usuarios con `/team join <nombre-team> <nombre-usuario>`
