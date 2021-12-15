# criptograf-a-https


## ¿Qué es http?

Las siglas HTTP, acrónimo de Hypertext Transfer Protocol, es un protocolo de transferencia de hipertexto. En otras palabras, HTTP es un protocolo de comunicación que permite la transferencia de información en Internet.

## Diferencia entre http y https

La principal diferencia entre HTTP y HTTPS es la seguridad. El protocolo HTTPS impide que otros usuarios puedan interceptar la información confidencial que se transfiere entre el cliente y el servidor web a través de Internet.


## El certificado SSL en una página web


El certificado permite pasar de http a https, es decir, permite encriptar los datos dentro de una página web para que una persona que intente interceptar esos datos a través de un ataque man in de middle sea "imposible" gracias a este cifrado.


## Tipos de certificados.

Comercialmente existen varios tipos de cifrados que te ofrecen distintas protecciones a nivel de dominio, pero todos con la misma base.

https://raw.githubusercontent.com/antonioherediia/criptograf-a-https/main/captura%20tabla%20certificados.JPG


## El certificado  Let’s Encrypt

 Let’s Encrypt es una Autoridad de Certificación gratuita, automatizada, y abierta. Puedes instalarlo de forma gratuita en tu página web. Existen dos formas de instalación.
 
###Con Acceso Shell
Recomendamos que la mayoría de las personas con acceso shell usen el cliente ACME llamado Certbot. Éste puede automatizar la emisión e instalación de certificados con cero tiempo de inactividad. También tiene modos de expertos para personas que no quieren autoconfiguración. Es fácil de usar, funciona en muchos sistemas operativos, y tiene documentación genial. Visita la página web de Certbot para conseguir instrucciones para tu sistema operativo y servidor de web.

Si Certbot no cumple con tus necesidades, o quisieras tratar otra cosa, hay muchos otros clientes ACME para escoger. Una vez hayas escogido un cliente ACME, ve la documentación para ese cliente para proceder.

Si estás experimentando con diferentes clientes ACME, usa nuestro ambiente de staging para evitar que llegues a nuestros limites de tarifa.

###Sin Acceso Shell
La mejor forma de utilizar Let’s Encrypt sin acceso shell es usando el soporte incorporado de tu proveedor de hospedaje. Si tu proveedor de hospedaje ofrece soporte para Let’s Encrypt, pueden solicitar un certificado gratis en su nombre, instalarlo, y mantenerlo actualizado automáticamente. Para algunos proveedores de hospedaje, esto es un ajuste de configuración que tienes que prender. Otros proveedores automaticamente solicitan e instalan certificados para todos sus clientes.

Revisa nuestra lista de proveedores de hospedaje para ver si el tuyo está en ella. Si lo está, sigue su documentación para configurar tu certificado de Let’s Encrypt.

Si tu proveedor de hospedaje no tiene soporte para Let’s Encrypt, puedes contactarlos para que lo soporten. Hacemos lo mejor que podemos para hacer fácil añadir soporte para Let’s Encrypt, !y proveedores suelen estar felices de escuchar sugerencias de clientes!

Si tu proveedor de hospedaje no quiere integrar Let’s Encrypt, pero sí tiene soporte para subir certificados custom, puedes instalar Certbot en tu propia computadora y usarlo en modo manual. En modo manual, tu subes un archivo específico a tu sitio web para probar tu control. Certbot recuperará un certificado que tu puedes subir a tu proveedor de hospedaje. No recomendamos esta opción porque es un contratiempo y necesitaras repetirlo varias veces durante el año cuando tu certificado expira. Para la mayoría de las personas es mejor solicitar soporte para Let’s Encrypt de su proveedor de hospedaje, o cambiar de proveedor si no tienen planes de implementarlo.

