# SecureWindow

Es un API de Integración a páginas web, para realizar pagos de forma segurá.Para transaccionar con Blumon Pay se requiere de solicitar una alta de usuario al correo: helloworld@blumonpay.com

##Integración HTML

Para una Integración completa es importante incluir en la cabecera de la página lo siguiente:
```html
<script type="text/javascript" src="http://ajax.googleapis.com/ajax/libs/jquery/1.7.2/jquery.min.js"></script>
<script src="http://blumonpay.com/SecureWindow/demo.js" type="text/javascript"></script>
```

```html
<script  
  data-user = "123" 
  data-password = "123"
  data-serial = "888-888-888"
  data-ptid = "888888888"
  src = " http://blumonpay.com/SecureWindow/transaction.js">
</script>

```
###Descripción de parámetros

Parámetro | Descripción
---|---
data-user| Nombre de Usuario
data-password | Contraseña
data-serial | Serial de Usuario
data-ptid | Ptid de usuario

Nota: Los datos antes mencionados se le proporcionan a usuario en el momento que desea utilizar el Botón de Pago Blumon Pay.

###Respuestas y notificaciones

El sistema emitirá una serie de notificaciones en diferentes eventos del proceso que se detallarán a continuación:

Variable | Valor | Descripción
---|---|---
ds_response | denied | Estatus de la transacción
id_fingerprint | Alfanumérico | Identificador
amount | Decimal | Total pagado



