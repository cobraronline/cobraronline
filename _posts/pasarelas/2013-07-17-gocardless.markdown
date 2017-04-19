---
layout: gateway
title:  "GoCardless"
date:   2016-06-10 20:02:36
categories: pasarelas sepa recurring insite prestashop 

gw_logo: "/images/gateways/gocardless.png"
gw_url: "https://gocardless.es"
gw_slogan: "Simpler Direct Debit."
gw_country: Reino Unido
gw_fee: "1%, máximo de €2 + Fijo mensual para que tu nombre aparezca en los extractos"
gw_twitter: 'GoCardless'
gw_docs: "https://developer.gocardless.com/pro"
---

GoCardless no utiliza la red de tarjetas, sino que utiliza la red SEPA para hacer los cargos directamente a la cuenta bancaria, es decir, vía domiciliación bancaria.
Eso hace que sus comisiones par a importes altos no admitan comparación con cualquier sistema de cobro basado en tarjetas de crédito/débito. 

Llevan cuatro años funcionando en Reino Unido y finalmente en 2015 han comenzado la expansión por todo Europa, incluyendo España.

Es una empresa creada por y para internet que gestiona el proceso de domiciliación bancaria totalmente, sin intervención del banco de empresa, nada más que para recibir el dinero de las remesas procesadas.

Al igual que [Besepa](/besepa/), GoCardless ofrece dos modos de funcionamiento, en función de que el que realice el cargo sea GoCardless o la empresa. Por defecto funcionan de la primera manera, aunque por un fijo de aproximadamente €200/mes puedes utilizar el segundo modo. 
 
El primer modo tiene un punto bueno (la simplificación del proceso de alta) pero un punto malo a tener en cuenta: al actuar como central de pagos, son ellos los que cobran al cliente y por tanto el cliente final tiene que firmar con ellos el mandato, no con el negocio, y por tanto pasan a ser clientes de GoCardless y si la empresa decide dejar GoCardless deberá firmar una un nuevo mandato o gestionar el cambio de acreedor en el siguiente cargo a cada cliente. 


-------------

#### Funciones

- Cobro con cargo directo a la cuenta bancaria
- Pagos recurrentes
- Autorizaciones y mandatos online
- Devoluciones a clientes
- Reintentos en caso de cobro incorrecto
- Emails a clientes y a comercios automatizados


-------------

#### Tecnología


Pueden integrarse directamente en tu web o formulario. Ofrecen también un API para integrarte con librerías oficiales en Ruby, PHP y Java. También soporta Webhooks para extender su funcionalidad y notificar de cualquier cambio que ocurra en tus cobros.

Es una empresa moderna por y para internet. Un gran API para integrarte con librerías oficales en Ruby, PHP, Java, Python y .NET.

También soporta Webhooks para extender su funcionalidad.

-------------

#### Panel de control

Aplicación moderna y de aspecto correcto con todo lo necesario para operar pero sin estridencias.

-------------

#### Módulos ecommerce


- [Prestashop](http://addons.prestashop.com/es/pagos-prestashop-modulos/5412-gocardless-payment.html)
- [Wordpress](https://wordpress.org/plugins/gocardless-wordpress-plugin/)
