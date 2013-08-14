---
layout: post
title:  "Pagos recurrentes"
date:   2013-08-14 16:02:36
categories: escenario
excerpt: "Existen muchas razones para cobrar a tus clientes regularmente: pago por uso, simplificar el proceso, etc. ¿Pero puedo hacerlo de forma sencilla?. La respuesta es si, claro, que puedes."
---

Además de los negocios de subscripción pura más habituales, como los [SAAS](/SAAS/) de subscripción, cada vez son más negocios los que requieren ciertos pagos recurrentes o los que quieren simplificar las compras sucesivas de sus clientes. 

Algunos casos ilustrativos podrían ser:

- Negocios que quieren simplificar las compras sucesivas (y las compras por impulso, claro :) ) de sus clientes reduciendo la fricción del proceso de compra al no requerir meter todos los datos de la tarjeta de crédito. ¿No es genial lo sencillo que es dejarse el dinero en Amazon o en el App Store de Apple?

- Negocios que quieren simplificar la compra desde dispositivos móviles (autorizar una operación de tarjeta de crédito con un móvil puede ser un dolor). Navegar con un móvil es fácil, pulsar botones aceptable, ¿pero validar una tarjeta de crédito?. No tanto, pruébalo y lo comprobarás. ¿Y si tu tienda/aplicación puede eliminar eso? 

- Negocios de pago por uso, en función de la utilización que hagan del servicio, ya sea mes a mes o de recarga automática de crédito. Todo es mucho más sencillo, y rentable, si puedes almacenar los datos de cobro de tu cliente y cobrarles cuando y cuanto corresponda. O en caso de usar _créditos_ ofrecerles la opción de recarga automática pasado un umbral. ¿No suena bien lo de _paga solo por lo que uses_ pero cobrarles automáticamente en lugar de perseguirles? 

- Negocios con un tipo de subscripción sencillo, sin varios planes, sin cambios, con ciclos largos, etc. Negocios como un registrador de dominios, acceso a contenidos premium, en los que no necesitas una gestión de subscripciones completas y compleja como las que ofrecen las plataformas pensadas para negocios [SAAS](/SAAS/).

Simplificar la forma en la que pagan los clientes no es más que bueno para el negocio, de modo que intentar ponérselo fácil debería ser una prioridad. 

##### ¿Cómo lo hago?

Esta forma de gestionar los cobros se basa en almacenar la tarjeta de crédito del cliente una vez autorizada, lo que comunmente se llama _[tokenizar la tarjeta](/tokenizar/)_

Cuando cobramos con tarjeta de crédito lo único que necesito es almacenar la tarjeta del cliente y poder realizarles el cargo posteriormente. Al proceso de almacenar la tarjeta se le llama [tokenizar la tarjeta](/tokenizar/) mientras que el cargo será una operación de autorización+captura habitual, siempre que el cliente tenga saldo en su tarjeta, por supuesto. Esto normalmente lo hace tu pasarela, y tú únicamente almacenas una referencia a dicha tarjeta, no su información.

Con plataformas como Paypal la terminología empleada es _crear un acuerdo de pagos_. En este caso, en lugar de realizar el pago, el cliente acudirá a la web de Paypal para autorizar a tu negocio a realizar cargos a su cuenta. Si bien en el caso de Paypal es posible que tengamos limitaciones para realizar determinadas operaciones desde España, como el pago por uso, por lo que sería inteligente hablar con ellos para explicar la operativa de vuestro negocio para confirmar que es viable utilizarlo.

Servicios como [GoCardless](/gocardless/) que trabajan con transferencias bancarias también serán una opción tan pronto estén disponibles en nuestro país.


##### Confianza.

Darle a un _semidesconido_ los datos de nuestra tarjeta de crédito es algo que no le gusta a nadie. Incluso cuando _técnicamente no sea así_. Los datos los almacena nuestra pasarela, pero eso es algo que ni sabe ni interesa al comprador.

Por tanto, no seas demasiado impetuoso pidiéndoles que almacenen sus datos aún a riesgo de perder alguna venta. Es importante que la confianza vaya creciendo. Si lo que ofreces es útil tu cliente optará por el medio más sencillo. Si no lo es, ofrecerles pagar en un click no va a hacer que lo sea.

Aunque es habitual en sistemas de créditos, no seas excesivamente ambicioso con los importes de las cargas/recargas esperando que el tener saldo sea razón suficiente para que el cliente vuelva, porque no lo es. Es posible que frustre la primera venta, y si no lo hace, forzarle a gastar mucho más de lo necesario no hará que aumente su satisfacción.



##### ¿Por dónde empezarías tú?

Ahora mismo hay ya muchas plataformas que soportar tokenizar la tarjeta, de modo que no debería ser problema conseguir una. Aún a riesgo de ser repetitivo:

- [Stripe](/stripe/) (en cuanto esté disponible en España) y [Paymill](/paymill/) me parecen los más avanzados tecnológicamente. Soy fan.
- La combinación de [Spreedly](/spreedly/) + [Redsýs](/redsys/) puede ser la más económica, sacrificando, de momento, el panel de control.


##### Bonus point.

Aunque no es estrictamente ilegal, las principales redes de tarjetas de crédito consideran que es una mala práctica cobrar por un producto antes de enviarlo si no se le notifica claramente al comprador. Con un producto digital no tenemos problema, puesto que el envío es inmediato. Pero, ¿qué podemos hacer con un producto físico que tenemos que pedir a nuestro proveedor antes de enviárselo a nuestro cliente?. 

Lo normal es que una autorización no se pueda mantener durante más de 7 días, de modo que si el plazo de envío es superior no podemos usar esta opción. ¿Qué hacer entonces?. Sencillo: [tokenizar la tarjeta](/tokenizar/) una vez autorizada, realizar el cargo al enviar el producto, eliminar la tarjeta almacenada (si no queremos ofrecerle guardarla para compras posteriores, claro). 
