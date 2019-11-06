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
  
### UML

<img src="UML/iteracion1.png"> 
