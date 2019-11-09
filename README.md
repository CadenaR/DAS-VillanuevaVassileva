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
