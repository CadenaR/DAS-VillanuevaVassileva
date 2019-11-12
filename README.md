## TABLA DE TIEMPOS

|Week|Iteration|Time in ADD<br>(ASS) |Reflection<br>Time<br>(ASS-ASC)|Time in refined<br> ADD<br>(ASS)|Design ADD<br> Time<br>(ASJ) |
| ------------- | ------------- |------------- |------------- |------------- |------------- |
|1|1|17min|15min|2min|11min|
|1|2|22min|12min|8min|27min|
|2|3|5min|9min|5min|5min|
|2|4|19min|8min|7min|-|
|3|5|28min|11min|12min|-|

## ANÁLISIS DE REQUISITOS
|Identificador|Nombre|Descripción|
| ------------- | ------------- |------------- |
|RF000|Eventos<br>inesperados | Capturar las distintas sucesiones de eventos inesperados |
|RF001|Gestionar<br> llamadas |Controlar las llamadas realizadas por los diferentes tipos de emergencias  |
|RF001.1|Identificar<br> llamadas<br> entrantes | Su función consiste en la identificar las llamadas entrantes tanto si son externas como si son internas |
|RF001.1.1|Gestionar<br> Incidencias<br> internas | Trata de resolver la incidencia interna en el sistema previamente identificada, en caso contrario lo comunicará conllevando a una solución inmediata si es posible |
|RF001.2|Llamadas<br> simultáneas |Recibe una cola de llamadas en un rango variable entre 15 y 20 llamadas simultáneas al centro de emergencias  |
|RF001.3|Distribución de<br> llamadas |Se pasarán las llamadas a los operadores disponibles en ese momento  |
|RF001.4|Reproducción de<br> llamadas | Muestra en un monitor el número identificado previamente por el identificador y la voz de la llamada |
|RF002|Gestión recursos<br> activos |Controla ambulancias bomberos, policías y unidades militares incluyendo los recursos necesarios para la emergencia.  |
|RF002.1|Mejorar ruta | Calcula las rutas más rápidas para que las unidades lleguen al punto de emergencias lo más rápido posible desde las instalaciones como punto de partida.  |
|RF002.2|Preasignación |Existe una unidad de preasignación de recursos activos para cada una de las unidades activas de cada emergencia  |
|RF003|Monitorización<br> emergencias |Monitoriza los activos en curso (emergencia videovigilancia y comunicaciones)  |
|RF004|Videovigilancia<br> urbana |Video vigilancia urbInteractuar usando una BD afín a poder acceder, enviar, recibir y consultar los datos internos del SCE para diferentes interacciones necesarias involucrando la diferenciación de los diferentes lugares ana mediante cámaras remotas que transmiten video mediante antenas de móvil/cableado urbano al sistema de emergencias en curInteractuar usando una BD afín a poder acceder, enviar, recibir y consultar los datos internos del SCE para diferentes interacciones necesarias involucrando la diferenciación de los diferentes lugares o y en el amplio abanico de instalaciones del complejo de emergencia  |
|RF005|Acceder a las<br> unidades activas |Interactuar usando una BD afín a poder acceder, enviar, recibir y consultar los datos internos del SCE para diferentes interacciones necesarias involucrando la diferenciación de los diferentes lugares  |
|RF006|Login | Facilita entrar con su perfil específico (Administrador del sistema, operarios de emergencias, operarios de unidades activas (ambulancias, helicópteros)) cuyos datos de información están actualizados en tiempo real |
|RF007|Sensores | Para detectar los eventos inesperados incendios) y que transmiten información vía radio a un centro de control remoto el cual envía un SMS y una alerta al sistema de emergencias como por ejemplo como sería el caso del detector de incendios |
|RF008|Priorización|Sirve para filtrar las emergencias y así jerarquizar cuales son más importantes que otras para que, en caso de que no haya operadores o nodos funcionales suficientes, se identifiquen las emergencias más prioritarias |
|RF009|Insuficientes<br> nodos funcionales | En caso de que no haya operadores suficientes poder atender las diferentes peticiones de los usuarios, por ejemplo, estructuración en temáticas de las posibles peticiones por parte de los usuarios de forma automática para así satisfacer sus peticiones, en caso de que el nodo funcional no pueda solucionarlo se le conectara con un operador lo antes posible. |
|RF010|Comunicación <br>cifrada | Garantiza la seguridad de comunicación entre organismos de defensa y del ejército a nivel tanto nacional como internacional. Existen comunicaciones cifradas para posibilitar la comunicación con unidades de policía y la unidad militar de emergencias (UME) por medio de radio y canales concretos |
|RF011|Traducción | Permite la traducción textual simultánea en tiempo real para emergencias que afectan a países cercanos |
|RF012|Subscripción | Facilitar la subscripción de los usuarios a noticias generadas por sucesos en tiempo real |
|RF012.1|Actualización de<br> información | Esta información tiene que estar siempre actualizada para los diferentes tipos de usuario |


## ITERACIÓN 1

#### ADD-00:

| Short title of decision  |Captura de eventos inesperados |
| ------------- | ------------- |
| ID | ADD-00 |
| Date | 15/10/2019 |
| Creator of the decision | Borja Castro, Deborah Villanueva |
| Status | Accepted |
| Requirements (decision drivers)  | - RF000-Eventos inesperados<br> - RF007-Sensores  |
| Decision outcome (options selected)  | Estilo por eventos |
| Pros Opciones | - Detectan eventos inesperados<br> - Alerta al sistema de emergencias  |
| Cons Opciones | - Alto y continuo mantenimiento<br> - Posibilidad de fallos y ruptura  |
| Link to other decisions | ADD-00, ADD-01, ADD-02, ADD-03, ADD-04, ADD-05, ADD-06,<br> ADD-07, ADD-08, ADD-09, ADD-10 |
| Link to architecture artifacts | UML iteración 1  |



#### ADD-01:

| Short title of decision  | Gestor de llamadas |
| ------------- | ------------- |
| ID | ADD-01 |
| Date | 15/10/2019 |
| Creator of the decision | Borja Castro, Deborah Villanueva |
| Status | Accepted |
| Requirements (decision drivers)  | RF001.Gestiónar llamadas<br>RF001.2 Llamadas simultaneas<br>RF001.3 Distribución de llamadas  |
| Decision outcome (options selected)  | Gestor de llamadas |
| Pros Opciones | - Engloba el amplio abanico de subsistemas<br> anidados  en lo referente a la gestión de llamadas<br> - Gestión ordenada<br> - Fácil escalado<br> - La generalización proporciona optimización<br> - Fácil administración y acceso  entre los subsistemas adheridos |
| Cons Opciones | - Menos particularización<BR> - más lento por acceso  |
| Link to other decisions | ADD-00, ADD-02, ADD-03, ADD-09, ADD-07,  |
| Link to architecture artifacts | UML iteración 2 (Sistema de procesamiento) |
  
#### UML

<img src="UML/iteracion1.png"> 

#### ADmentor

<img src="UML/ADMentor1.png">

<img src="UML/ADMentor2.png">

<img src="UML/ADMentor3.png">


## ITERACIÓN 2

#### ADD-02:

| Short title of decision  | Identificación de llamadas entrantes |
| ------------- | ------------- |
| ID | ADD-02 |
| Date | 16/10/2019 |
| Creator of the decision | Borja Castro, Deborah Villanueva |
| Status | Accepted |
| Requirements (decision drivers)  | - R001.1  Identificar de llamadas entrantes<br> - RF001.1.1 Gestionar incidencias internas<br> - RF001.4 Reproducción de llamadas   |
| Pros Opciones  | - Identificación inmediata de las llamadas<br> - Posible solución de una incidencia rápidamente<br> - Resolución de conflictos internos no conocidos<br> - Visualización identificada con voz de la llamada correspondiente  |
| Cons Opciones | - Amplia variedad de identificadores con resultante confusión |
| Link to other decisions | ADD-00, ADD-01 |
| Link to architecture artifacts | UML iteración 2 (Sistema de procesamiento) |

#### ADD-03:

| Short title of decision  | Gestión recursos activos |
| ------------- | ------------- |
| ID | ADD-03 |
| Date | 16/10/2019 |
| Creator of the decision | Borja Castro, Deborah Villanueva |
| Status | Accepted |
| Requirements (decision drivers)  | - RF002: Gestión de recursos activos<br>- RF002.2 Preasignación<br> - F003 Monitorización emergencias|
| Pros Opciones | - Control del personal  necesario en cada momento de<br> cierta emergencia.<br> - Rapidez a la hora de facilitar los recursos puesto que<br> son pre asignados con antelación |
| Cons Opciones | - Posibilidad de recursos inactivos puesto que al estar<br> asignados una cantidad mínima de personal,<br> algunos no ejercen |
| Link to other decisions | ADD-00, ADD-01, ADD-04, ADD-07  |
| Link to architecture artifacts | UML iteración 2 (Sistema de procesamiento) |

#### ADD-04:

| Short title of decision  | Optimización de ruta |
| ------------- | ------------- |
| ID | ADD-04 |
| Date | 16/10/2019 |
| Creator of the decision | Borja Castro, Deborah Villanueva |
| Status | Accepted |
| Requirements (decision drivers)  | - RF002.1 Mejorar ruta |
| Alternative decisions (options) | Programas de terceros (como Google Maps o Waze) |
| Decision outcome (options selected)  | Optimización de ruta |
| Pros Opciones | Opcion1:<br> - Mayor rapidez para llegar al lugar<br> - Tráfico en tiempo real<br><br>Opcion2:<br>- Económico |
| Cons Opciones | Opcion1:<br>- Algoritmo complejo<br>- Requiere de personal especializado para<br> desarrollarlo, optimizarlo y mantenerlo con continuidad<br>- Precio elevado<br><br>Opción2:<br>- Menos personalizable |
| Link to other decisions | DD-00, ADD-03  |
| Link to architecture artifacts | UML iteración 2 (Sistema de procesamiento) |

#### UML

<img src="UML/iteracion2.png"> 

## ITERACIÓN 3

#### ADD-05:

| Short title of decision  | Sistema de videovigilancia |
| ------------- | ------------- |
| ID |  ADD-05 |
| Date | 22/10/2019 |
| Creator of the decision | Borja Castro, Deborah Villanueva |
| Status | Accepted |
| Requirements (decision drivers)  | - RF004 Video-vigilancia |
| Pros Opciones | - Control visual de los activos<br>- Incremento de seguridad en las instalaciones |
| Cons Opciones | - Pueden ser hackeadas<br>- Posible robo de privacidad<br>- Mantenimiento económicamente elevado |
| Link to other decisions | DD-00, ADD-03 |
| Link to architecture artifacts | UML iteración 3 (Sistema de Recepción) |

#### UML

<img src="UML/iteracion3.png">

## ITERACIÓN 4

#### ADD-06:

| Short title of decision  | Acceso a perfil |
| ------------- | ------------- |
| ID |  ADD-06 |
| Date | 23/10/19 |
| Creator of the decision | Borja Castro, Deborah Villanueva |
| Status | Accepted |
| Requirements (decision drivers)  | - RF006 Login |
| Pros Opciones | - Acceso a datos específicos para el usuario<br>- Adaptación al entorno digital<br>- Mejora de la experiencia de usuario |
| Cons Opciones | - Necesidad de una base de datos para<br> almacenar los usuarios almacenados |
| Link to other decisions | ADD-00, ADD-03 |
| Link to architecture artifacts | UML iteración 4 (Sistema de Gestión y Sistema de Procesamiento) |

#### ADD-07:

| Short title of decision  | Creación de nodos funcionales |
| ------------- | ------------- |
| ID |  ADD-07 |
| Date | 23/10/19 |
| Creator of the decision | Borja Castro, Deborah Villanueva |
| Status | Accepted |
| Requirements (decision drivers)  | - RF009- Insuficientes nodos funcionales |
| Decision outcome (options selected)  | Creación de nodos funcionales |
| Pros Opciones | Nodos funcionales<br>- Proporciona una estrategia de resolución de conflicto<br> en el acceso  de operadores aun no estando los<br> operadores disponibles, permitiendo la respuesta de las<br> peticiones de los usuarios<br>- Aumentando la entrada de llamadas.<br><br>Contratación de  más operadores<br> - Más atención personalizada<br> - Mayor disponibilidad prestada a los usuarios<br> - Cercanía al ususario<br><br>Inclusión de la Inteligencia Artificial(IA) con Machine <br>Learning<br>- Constante aprendizaje a cerca de las peticiones, <br>consecuentemente una mejor aplicación a futuras llamadas<br>- Disminución de personal |
| Cons Opciones | Nodos funcionales<br>- No hay atención personalizada<br>- Hay un límite de respuestas, correspondiente a la<br> capacidad del servidor<br><br>Contratación de  más operadores<br>- Elevar el coste<br>- Proporcionar mayor espacio físico(instalaciones)<br>- Mayor cantidad de nodos<br><br>Inclusión de la Inteligencia Artificial(IA) con Machine <br>Learning<br>- Elevado coste<br>- Mantenimiento<br>- Personal especializado para desarrollarlo o personalizarlo |
| Link to other decisions | ADD-00, ADD-01, ADD-02, ADD-03, ADD-09 |
| Link to architecture artifacts | UML iteración 4 (Sistema de Procesamiento, específicamente en “Gestor de Llamadas” el método “Operadoresocupados(Llamada)”) |

#### UML

<img src="UML/iteracion4.png">

## ITERACIÓN 5

#### ADD-08:

| Short title of decision  | Cifrado propio de comunicación  |
| ------------- | ------------- |
| ID |  ADD-08 |
| Date | 23/10/19 |
| Creator of the decision | Borja Castro, Deborah Villanueva |
| Status | Accepted |
| Requirements (decision drivers)  | - RF010 Comunicación cifrada |
| Alternative decisions (options) | Encriptación de terceros |
| Decision outcome (options selected)  | Cifrado propio de comunicación |
| Pros Opciones | Cifrado propio de comunicación<br>- Comunicación adaptada a organismos de defensa<br>- Privacidad gubernamental<br>- Seguridad de mensajes privados<br><br>Encriptación de terceros<br>- Uso de claves ya proporcionadas<br>- Más económico |
| Cons Opciones | Cifrado propio de comunicación<br>- Actualización constante en el código de <br>encriptación<br>- Crear el propio algoritmo de cifrado y la clave<br> correspondiente para descifrarlo<br>- Personal especializado<br><br>Encriptación de terceros<br>- Poca seguridad debido a la clave compartida |
| Link to other decisions | ADD-00, ADD-06, ADD-03  |
| Link to architecture artifacts | UML iteración 5 (Sistema de Gestión)  |

#### ADD-09:

| Short title of decision  | Traductor de terceros |
| ------------- | ------------- |
| ID |  ADD-09 |
| Date | 29/10/19 |
| Creator of the decision | Borja Castro, Deborah Villanueva |
| Status | Accepted |
| Requirements (decision drivers)  | - RF011. Traducción |
| Alternative decisions (options) | Traductor propio |
| Decision outcome (options selected)  | Traductor de terceros |
| Pros Opciones | Traductor propio:<br>- Comunicación internacional<br>- Traducción precisa a profesionales en<br> lengua materna<br>- Aprendizaje de termionología <br>especialista(tecnicismos)<br><br>Traductor de terceros:<br>- Mas barato |
| Cons Opciones | Traductor propio:<br>- Posible pérdida de información<br>- Posible malinterpretación<br><br>Traductor de terceros:<br>- Difícil modificación |
| Link to other decisions | ADD-00, ADD-03, ADD-10 |
| Link to architecture artifacts | UML iteración 5 (Sistema de Gestión)|

#### ADD-10:

| Short title of decision  | Subscripción de usuario |
| ------------- | ------------- |
| ID |  ADD-10 |
| Date | 29/10/19 |
| Creator of the decision | Borja Castro, Deborah Villanueva |
| Status | Accepted |
| Requirements (decision drivers)  | - RF012 Subscripción<br>- RF012.1Actualización de información |
| Pros Opciones | - Distribución de información a los usuarios<br>- Información actualizada en tiempo real<br>- Fácil, simple ordenado<br>- Accesible  |
| Cons Opciones | - Dependencia de la conexión a internet<br>- Personal técnico encargado de la elaboración de las noticias |
| Link to other decisions | ADD-00, ADD-03, ADD ADD-05, ADD-06,ADD-09 |
| Link to architecture artifacts | UML iteración 5 (Sistema de Gestión) |


#### UML

<img src="UML/iteracion5.png">
