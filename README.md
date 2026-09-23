# Arcia — publicaciones

Aquí se publican los instaladores de **Arcia**, la aplicación de escritorio para
prospección B2B local: encuentra negocios sin sitio web, lo verifica, y te pone
a llamarlos con el guion delante.

Este repositorio contiene **solo los instaladores**. El código fuente no es
público.

## Descargar

La última versión está siempre en **[Releases](../../releases/latest)**.

Descarga el fichero `Arcia_X.Y.Z_x64-setup.exe` y ejecútalo.

## Al instalar, Windows te va a avisar

Verás una pantalla que dice **«Windows protegió su PC»** y menciona un *editor
desconocido*.

No es un virus. Es lo que Windows muestra con cualquier programa que no lleva
un certificado de firma, que es un trámite de pago anual contratado aparte.

Para continuar: **«Más información» → «Ejecutar de todas formas»**. Solo pasa
al instalar, no cada vez que abras la aplicación.

## Verificar que el fichero es el auténtico

Cada versión se publica con la huella SHA-256 de sus instaladores en las notas
de la publicación. Para comprobar el fichero que te has descargado:

```powershell
Get-FileHash .\Arcia_X.Y.Z_x64-setup.exe -Algorithm SHA256
```

El resultado tiene que coincidir letra por letra con la huella publicada. Si no
coincide, no lo instales.

## Actualizaciones

Una vez instalada, la aplicación comprueba sola si hay versión nueva al
abrirse y se ofrece a actualizarse. No hace falta volver aquí.

## Tus datos

Arcia funciona entera en tu ordenador. Su base de datos y sus copias de
seguridad se guardan en local: tus leads, tus notas y tus claves no se envían a
ningún servidor.

Desde la 1.6.87 hay una excepción, contada en la cláusula 4 de los términos: si
Google Maps deja de devolver negocios de una forma que apunta a un fallo de
Google, la app manda a soporte un aviso **anónimo** —la versión, el modo de
búsqueda y el nicho, la ciudad y el número de resultados de tus últimos
escaneos— como mucho una vez al día. Se apaga en **Ajustes → Datos**.

## Historial de versiones

De la más reciente a la más antigua. Cada versión tiene sus notas completas en
**[Releases](../../releases)**.

### Arcia 1.6

| Versión | Fecha | Qué cambia |
|---|---|---|
| **1.6.93** | 23-09-2026 | Términos y condiciones 1.3: los correos comerciales que mandes son responsabilidad tuya. El guion ya no se inventa un cliente de referencia, y Ajustes está más limpio. |
| **1.6.92** | 23-09-2026 | Si falla el cobro, la pantalla de activación te deja arreglarlo en Stripe. Los números grandes llevan su punto (1.000), y los correos se presentan para el seguimiento. |
| **1.6.91** | 23-09-2026 | Términos y condiciones 1.2: el cambio de ordenador con suscripción lo haces tú desde la app. Tu licencia explica qué consulta, y las notas de versión llevan tildes y eñes. |
| **1.6.90** | 23-09-2026 | Corregido el aviso sobre el correo comercial no solicitado: la LSSI lo prohíbe también entre empresas. «Enviar a soporte» lleva tu correo para poder contestarte. |
| **1.6.89** | 23-09-2026 | La suscripción se gestiona o se cancela desde la app, y se pasa a otro ordenador con un código por correo. Todas las métricas, en Resultados. |
| **1.6.88** | 23-09-2026 | Los errores se explican en castellano claro y dicen qué hacer, Ajustes → Búsqueda sin tecnicismos, y la activación enseña el precio y los 7 días de prueba gratis. |
| **1.6.87** | 22-09-2026 | Si Google Maps deja de devolver negocios en una búsqueda que antes sí los daba, Arcia lo dice claramente y avisa a soporte con un aviso anónimo que se puede apagar. Términos y condiciones 1.1. |
| **1.6.86** | 22-09-2026 | Mantenimiento: la app, mejor ordenada por dentro. No cambia nada de lo que ves. |
| **1.6.85** | 21-09-2026 | Los términos y condiciones se aceptan antes de activar o pagar, y se pueden releer en Ajustes → Tu licencia. |
| **1.6.84** | 20-09-2026 | Buscar un gremio ya no devuelve de todo: «Hamburguesería» en Elche pasa de 179 negocios mezclados a 23 que lo son. |
| **1.6.83** | 20-09-2026 | Un desplegable que se abre hacia arriba aparece pegado a su campo. |
| **1.6.82** | 20-09-2026 | El aviso de versión nueva ya no parte las frases por la mitad. |
| **1.6.81** | 20-09-2026 | El desplegable de modelos de IA solo enseña los que escriben texto. |
| **1.6.80** | 20-09-2026 | Un escaneo ya no se come la cuota diaria de IA: queda crédito para generar webs. |
| **1.6.79** | 20-09-2026 | Verificar negocios va 2,25 veces más rápido (60 negocios, de 209 s a 93 s) con los mismos resultados. |
| **1.6.78** | 19-09-2026 | Una búsqueda pasa del tope de 120 negocios de Maps preguntando de varias formas. |
| **1.6.77** | 19-09-2026 | Las webs generadas dejan de llevar la marquesina de frases. |
| **1.6.76** | 19-09-2026 | Guardar Ajustes ya no borra el modelo de IA que la app había puesto al día. |
| **1.6.75** | 19-09-2026 | Cuando tu proveedor retira el modelo de IA por defecto, la app se pasa sola al que lo sustituye y te lo dice. |
| **1.6.74** | 19-09-2026 | «Tu zona» es un desplegable de municipios, para que el guion no diga una ciudad mal escrita. |
| **1.6.73** | 19-09-2026 | Un fichero dañado ya no cierra la app a mitad de una tanda. |
| **1.6.72** | 19-09-2026 | Versión de seguridad: componentes al día, y un PDF preparado ya no puede tumbar la app. |
| **1.6.71** | 19-09-2026 | En «Qué guion cierra» cada guion se nombra por sus fechas, y una cita que se cae no le quita el mérito al guion que la consiguió. |
| **1.6.70** | 19-09-2026 | Cuatro cifras de Resultados corregidas: «Qué nicho funciona» agrupa por nicho, un porcentaje pide un mínimo de casos y el embudo ya no pasa del 100 %. |
| **1.6.69** | 19-09-2026 | «Embudo» pasa a llamarse «Resultados». |
| **1.6.68** | 18-09-2026 | La cabecera de la tabla se queda dentro de su tarjeta al desplazar la lista. |
| **1.6.67** | 18-09-2026 | La búsqueda de correos hace una búsqueda menos por lead, y «Regenerar todos los guiones» respeta los escritos a mano. |
| **1.6.66** | 18-09-2026 | Las webs generadas funcionan bien en el móvil. |
| **1.6.65** | 18-09-2026 | Todos los leads por llamar tienen su guion, y un error de la IA ya no dice que Google está caído cuando no lo está. |
| **1.6.64** | 18-09-2026 | «Solo la categoría buscada» aprende cómo llama Google a cada gremio: un sushi es un «Restaurante japonés». |
| **1.6.63** | 17-09-2026 | Si la web de un negocio está enlazada desde su página en un portal (idealista, booksy…), se encuentra. |
| **1.6.62** | 17-09-2026 | Arreglos de la 1.6.61: Correos deja sitio a los leads y el menú cabe en ventanas bajas. |
| **1.6.61** | 17-09-2026 | Del primer correo a la reunión: Arcia lee las respuestas y las aplica, secuencias de seguimiento, recontacto, comprobación de entregabilidad, varios buzones y empresas recién creadas del BORME. |
| **1.6.60** | 17-09-2026 | Un nombre que comparten varios municipios («San Juan») ya no vacía la búsqueda, y «Solo la categoría buscada» viene encendido. |
| **1.6.59** | 16-09-2026 | Arreglos del Embudo: ya se puede desplazar, lleva su cabecera y redondea bien. |
| **1.6.58** | 16-09-2026 | Nueva sección Embudo: de negocios escaneados a euros cobrados, y qué nicho y qué pueblo rinden más. |
| **1.6.57** | 16-09-2026 | Webs generadas más trabajadas —carrusel, carta con pestañas, galería con visor— y sin bloques en blanco. |
| **1.6.56** | 15-09-2026 | El contador de reseñas se lee también en instalaciones nuevas. |
| **1.6.55** | 15-09-2026 | Vuelven las fotos en instalaciones nuevas, y reescanear una zona trae solo lo que no tenías. |
| **1.6.54** | 14-09-2026 | Suscripción mensual: la app se activa sola al pagar y se renueva cada mes sin pegar ninguna clave. |
| **1.6.53** | 14-09-2026 | Una licencia que caduca no se alarga atrasando el reloj del ordenador. |
| **1.6.52** | 13-09-2026 | Pantalla de activación más clara, y entera en ventanas pequeñas. |
| **1.6.51** | 13-09-2026 | Una web que devuelve el buscador solo cuenta si de verdad es del negocio: su teléfono, o su nombre y su ciudad. |
| **1.6.50** | 13-09-2026 | La verificación encuentra muchas más webs de verdad y no confunde fichas de directorios con webs. |
| **1.6.49** | 13-09-2026 | Nueva casilla «Solo negocios de la categoría buscada», y fuera los correos de otras empresas. |
| **1.6.48** | 13-09-2026 | La verificación ya no da la web de otro negocio con nombre parecido ni la ficha de un directorio, que descartaban leads buenos. |
| **1.6.47** | 13-09-2026 | Termina el rediseño: Agenda, tutorial, activación y primera búsqueda. |
| **1.6.46** | 13-09-2026 | Leads, Correos y la ficha de cada negocio, rediseñados. |
| **1.6.45** | 13-09-2026 | Ajustes rediseñado, y cada error trae su botón «Enviar a soporte». |
| **1.6.44** | 13-09-2026 | Prospección rediseñada: la búsqueda en una barra y el resultado justo debajo. |
| **1.6.43** | 13-09-2026 | La pantalla de Llamar, mucho más despejada. |
| **1.6.42** | 13-09-2026 | Los botones de la ventana en su franja, y los leads nuevos ya no se ven amontonados. |
| **1.6.41** | 13-09-2026 | Arreglado un parpadeo del menú al cambiar de sección. |
| **1.6.40** | 13-09-2026 | Diseño nuevo con paneles flotantes, y el informe de soporte se envía sin usar tu correo. |
| **1.6.39** | 13-09-2026 | El horario ya no se da por inexistente cuando lo tapaba el aviso de cookies de Google, y el informe de diagnóstico recoge los errores. |
| **1.6.38** | 10-09-2026 | Buscando en un pueblo ya no se cuelan negocios del de al lado con la ciudad equivocada en el guion. |
| **1.6.37** | 09-09-2026 | La medición de la verificación explica qué quiere decir su «cero». |
| **1.6.36** | 09-09-2026 | La medición de la verificación cuenta también cuándo se toma por web la ficha de un portal. |
| **1.6.35** | 09-09-2026 | La medición de la verificación contaba como fallos tres aciertos. |
| **1.6.34** | 08-09-2026 | La medición de la verificación enseña por dónde va. |
| **1.6.33** | 08-09-2026 | Un proxy bloqueado ya no tumba el escaneo, y nuevo botón para medir cuánto acierta la verificación. |
| **1.6.32** | 08-09-2026 | El tutorial nombra las secciones, y se explica cómo sacar la contraseña de aplicación del correo. |
| **1.6.31** | 07-09-2026 | Tutorial para quien abre Arcia por primera vez. |
| **1.6.30** | 07-09-2026 | El aviso de negocios sin correo se quita al entrar en Correos. |
| **1.6.29** | 07-09-2026 | Escaneos más rápidos: ya no se abren las fichas de los negocios descartados. |
| **1.6.28** | 07-09-2026 | Arreglado Ajustes, que en la 1.6.27 se abría en negro, y el informe de diagnóstico se envía con un botón. |
| **1.6.27** | 07-09-2026 | *Retirada*: dejaba Ajustes en negro. La sustituyó la 1.6.28. |
| **1.6.26** | 07-09-2026 | La búsqueda de correos sigue funcionando cuando DuckDuckGo deja de contestar. |
| **1.6.25** | 07-09-2026 | La búsqueda de respaldo en Bing por fin funciona: los correos encontrados pasan del 5 % al 44 %. |
| **1.6.24** | 07-09-2026 | El aviso de negocios sin correo se queda hasta que lo atiendes. |
| **1.6.23** | 07-09-2026 | Al terminar un escaneo, aviso de los negocios sin correo con un botón para buscárselo. |
| **1.6.22** | 07-09-2026 | El botón de buscar correos, a la vista, y vaciar la base ya no le hace olvidar a la app lo que ha aprendido. |
| **1.6.19** | 07-09-2026 | «Vaciar la base» vacía de verdad, sin tocar tus ajustes ni tu lista de bajas. |
| **1.6.18** | 06-09-2026 | Se retira la extensión del navegador. |
| **1.6.17** | 06-09-2026 | Las webs generadas se ven mejor en el móvil y sin bloques en blanco. |
| **1.6.16** | 06-09-2026 | Webs sin secciones vacías, con horario aunque el negocio tenga varios, y cada una con su propio diseño. |
| **1.6.15** | 06-09-2026 | El icono de WhatsApp ya sale en las webs. |
| **1.6.14** | 06-09-2026 | Los logotipos de marca de las webs salen exactos, de una librería. |
| **1.6.13** | 06-09-2026 | El horario se lee aunque Maps lo tenga plegado, el menú de las webs se lee y se avisa mientras se genera. |
| **1.6.12** | 06-09-2026 | Cuando un modelo de IA gratis falla, Arcia dice qué hacer. |
| **1.6.11** | 06-09-2026 | La web no se inventa el horario, y arreglos de secciones y desplazamiento. |
| **1.6.10** | 06-09-2026 | El horario de la semana se trae solo de Google Maps. |
| **1.6.9** | 06-09-2026 | Horario de la semana en la ficha, y la web usa la carta de las fotos y el mapa. |
| **1.6.8** | 06-09-2026 | Webs con iconos de verdad, portada con el local y SEO. |
| **1.6.7** | 06-09-2026 | Probar la conexión de IA ya no pide aceptar nada antes. |
| **1.6.6** | 06-09-2026 | El tope de webs con IA gratis pasa a ser un contador, y el aviso de datos se ajusta a cada proveedor. |
| **1.6.5** | 06-09-2026 | Proveedores de IA gratis y sin tarjeta: OpenRouter y NVIDIA. |
| **1.6.4** | 06-09-2026 | Permiso explícito para usar los modelos que entrenan con lo que se les manda. |
| **1.6.3** | 06-09-2026 | Nuevos proveedores de IA, OpenCode Zen y Groq, y relevo automático cuando el tuyo no contesta. |
| **1.6.2** | 06-09-2026 | Termina la cara nueva: la letra pasa a ser la del logotipo. |
| **1.6.1** | 06-09-2026 | Arregla un fallo al actualizar desde la 1.5 y quita el azul de la interfaz. |
| **1.6.0** | 05-09-2026 | **Imagen nueva**: nombre, logotipo e iconos nuevos. Mismas funciones. |

Las versiones 1.6.20 y 1.6.21 no llegaron a publicarse.

### Arcia 1.5

| Versión | Fecha | Qué cambia |
|---|---|---|
| **1.5.10** | 03-09-2026 | Las webs generadas ya se recorren con la rueda del ratón. |
| **1.5.9** | 02-09-2026 | «Hacerle la web» ya funciona: en la 1.5.7 y la 1.5.8 se cortaba siempre. |
| **1.5.8** | 02-09-2026 | Si el proveedor de IA retira el modelo por defecto, la app se arregla sola, y sus errores se leen enteros. |
| **1.5.7** | 02-09-2026 | **Hacerle la web a un lead** con IA, con los colores de su local. Proveedores Kimi y DeepSeek, y el modelo en un desplegable. |
| **1.5.6** | 02-09-2026 | Las variantes de un oficio salen debajo de su oficio y no como un nicho aparte. |
| **1.5.5** | 02-09-2026 | Pronóstico de leads al escribir oficio y ciudad, otras formas de pedir el mismo oficio, y un municipio con dos nombres cuenta una vez. |
| **1.5.4** | 01-09-2026 | Antes de buscar, la app te dice cuántos leads espera darte, y la tanda de llamadas ya no trae leads sin teléfono. |
| **1.5.3** | 30-08-2026 | La búsqueda de correos no repite negocios ya buscados y va más rápida. |
| **1.5.2** | 30-08-2026 | La extensión del navegador se empareja sola y añade negocios desde cualquier página. |
| **1.5.1** | 28-08-2026 | La extensión se instala en dos pasos, y las fotos de los negocios ya no dependen de la suerte. |
| **1.5.0** | 28-08-2026 | Búsqueda de correos cuatro veces más rápida, fuera los negocios fantasma y la ficha del lead más despejada. |

### Arcia 1.4

| Versión | Fecha | Qué cambia |
|---|---|---|
| **1.4.4** | 26-08-2026 | La etiqueta NUEVO de la primera fila se ve entera. |
| **1.4.3** | 26-08-2026 | Las fotos del local en la ficha, escaneo más rápido y **conexión opcional con IA** para el guion, el correo y buscar webs. |
| **1.4.2** | 26-08-2026 | Lo que trae cada escaneo sale marcado como NUEVO, y dos nichos más: Cafetería de especialidad y Brunch. |
| **1.4.1** | 26-08-2026 | Dos arreglos de la lista al abrir la ficha de un negocio. |
| **1.4.0** | 25-08-2026 | El horario debajo del teléfono, en amarillo si está cerrado; búsqueda de correos más rápida; buscador de Google y extensión del navegador. |

### Arcia 1.0 – 1.3

| Versión | Fecha | Qué cambia |
|---|---|---|
| **1.3.0** | 17-08-2026 | Revisión del diseño: la tabla se maneja con el teclado, se ordena por columnas, filas compactas y mejor contraste. |
| **1.2.0** | 17-08-2026 | Sin barra de título: la interfaz gana una fila entera. La tanda de envío deja rastro en el registro. |
| **1.1.1** | 16-08-2026 | Tres arreglos: comprobar rebotes, correos de negocios con tildes y el registro de directorios. |
| **1.1.0** | 16-08-2026 | Muchos más correos encontrados (directorio del pueblo, guías en PDF, teléfono); un perfil de Facebook o Instagram ya no cuenta como web; ventana propia. |
| **1.0.2** | 12-08-2026 | Correos en el ayuntamiento y la asociación de comerciantes, 197 nichos con sinónimos y borrar todos los leads de una búsqueda. |
| **1.0.1** | 10-08-2026 | Licencias atadas a tu ordenador y actualizaciones automáticas. |
| **1.0.0** | 08-08-2026 | Primera versión a la venta: escaneo de Google Maps, verificación de si cada negocio tiene web, guion de llamada, correos, y registro e informe de diagnóstico. Ya no está en esta página, y no se actualiza sola: desde ella hay que instalar una versión nueva a mano. |
