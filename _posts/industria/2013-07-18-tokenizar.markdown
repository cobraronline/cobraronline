---
layout: post
title:  "Tokenizar tarjetas"
date:   2013-08-14 16:32:36
categories: industria
excerpt: ¡Conoce la operación básica para realizar pagos recurrentes en tu negocio!
---

Básicamente, _tokenizar_ un conjunto de datos trata de substituirlos por otro conjunto , que podamos utilizar en su lugar, utilizando un algoritmo difícil de adivinar y que además se pueda revertir si fuera necesario. Normalmente se utiliza para almacenar de forma segura información sensible, como por ejemplo contraseñas, datos personales y por supuesto datos bancarios.

En la industria de las tarjetas de crédito se utiliza desde 2005 para, entre otras cosas, almacenar tarjetas de crédito validadas de manera que las podamos utilizar posteriormente. Nuestra pasarela de pago almacenará los datos de la tarjeta, cumpliendo los más altos estándares de seguridad marcados por la industria y nos dará un _token_ con el que hacer referencia a la misma a la hora de hacer cargos posteriormente. De esta forma los datos de nuestros clientes están mucho más protegidos.

Esta es la forma en la que funcionan los servicios que permiten [pagos recurrentes](/pagos-recurrentes/):

1. El negocio solicita los datos de la tarjeta de crédito del cliente
2. Los envía a la pasarela de pago para su tokenización
3. La pasarela devuelve el token al negocio, que lo almacena relacionado con la transacción o el cliente
4. A partir de aquí el negocio puede realizar todas las operaciones que quiera sobre esa tarjeta sin que el cliente intervenga utilizando el token.


#### ¿He leído bien?, ¿lo que quiera?

Si, lo que quiera, mientras el token y la tarjeta sean válidos. No hay que olvidar que las tarjetas pueden ser canceladas, anuladas o caducar.

Pero igual de importante es realizar las operaciones adecuadas, en el momento adecuado. De no ser así puede aumentar el número de disputas de cargos y con ello aumentar nuestro _fee_ o que nos bloqueen la pasarela, así que no lo entiendas como una barra libre.


#### ¿Me estoy casando con mi plataforma?

Aunque no es algo que se ofrezca siempre públicamente, la mayoría de las pasarelas que ofrecen tokenización permiten mover una vez los tokens de una pasarela a otra. Consúltales si es tu caso o si te da miedo.

En este sentido también es muy interesante el servicio de [Spreedly](/spreedly/), enfocado precisamente a _tokenizar_ tarjetas de forma independiente a la pasarela. De esta forma puedes utilizar una misma tarjeta _tokenizada_ con distintas pasarelas según te interese en cada momento.

