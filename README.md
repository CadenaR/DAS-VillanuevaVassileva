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
| Link to other decisions | ADD-00, ADD-01, ADD-02, ADD-03, ADD-04, ADD-05, ADD-06,<br> ADD-07, ADD-08, ADD-09, ADD-10, ADD-11 |
| Link to architecture artifacts | Arquitectura por eventos (observer)  |


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
| Link to other decisions | ADD-02,ADD-03,ADD06 |
| Link to architecture artifacts | Arquitectura por eventos (observer) |
  
#### UML

<img src="UML/iteracion1.png"> 


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
| Link to other decisions | ADD-01, ADD-06 |

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
| Link to other decisions | ADD-01,ADD02, ADD06 |

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
| Link to other decisions | ADD-03 |

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
| Link to architecture artifacts | PAQUETE: (Arquitectura por eventos (observer)) |

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
| Link to other decisions |  |
| Link to architecture artifacts | Arquitectura por eventos (observer) |

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
| Link to other decisions | ADD00, ADD06, ADD03 |
| Link to architecture artifacts | UML iteración 5 (Sistema de Gestión)  |

#### ADD-09:

| Short title of decision  | Traductor de terceros |
| ------------- | ------------- |
| ID |  ADD-09 |
| Date | 29/10/19 |
| Creator of the decision | Borja Castro, Deborah Villanueva |
| Status | Accepted |
| Requirements (decision drivers)  | - RF011. Traducción |
| Alternative decisions (options) | Traductor de terceros terceros |
| Decision outcome (options selected)  | Traductor de terceros terceros |
| Pros Opciones | Traductor propio:<br>- Comunicación internacional<br>- Traducción precisa a profesionales en<br> lengua materna<br>- Aprendizaje de termionología <br>especialista(tecnicismos)<br><br>Traductor de terceros:<br>- Mas barato |
| Cons Opciones | Traductor propio:<br>- Posible pérdida de información<br>- Posible malinterpretación<br><br>Traductor de terceros:<br>- Difícil modificación |
| Link to other decisions | ADD00, ADD03, ADD10 |
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
| Link to other decisions | ADD00, ADD ADD05, ADD06,ADD09 |
| Link to architecture artifacts | UML iteración 5 (Sistema de Gestión) |


#### UML

<img src="UML/iteracion5.png">
