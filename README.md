# LeadHunter — publicaciones

Aquí se publican los instaladores de **LeadHunter**, la aplicación de
escritorio para prospección B2B local: encuentra negocios sin sitio web, lo
verifica, y te pone a llamarlos con el guion delante.

Este repositorio contiene **solo los instaladores**. El código fuente no es
público.

## Descargar

La última versión está siempre en **[Releases](../../releases/latest)**.

Descarga el fichero `LeadHunter_X.Y.Z_x64-setup.exe` y ejecútalo.

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
Get-FileHash .\LeadHunter_X.Y.Z_x64-setup.exe -Algorithm SHA256
```

El resultado tiene que coincidir letra por letra con la huella publicada. Si no
coincide, no lo instales.

## Actualizaciones

Una vez instalada, la aplicación comprueba sola si hay versión nueva al
abrirse y se ofrece a actualizarse. No hace falta volver aquí.

## Tus datos

LeadHunter funciona entero en tu ordenador. Su base de datos y sus copias de
seguridad se guardan en local, y no se envía nada a ningún servidor.
