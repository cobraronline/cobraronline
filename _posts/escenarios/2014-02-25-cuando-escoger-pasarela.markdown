---
layout: post
title:  "Cuándo escoger una pasarela"
date:   2014-02-25 22:32:36
categories: escenario
excerpt: "¿En que momento del desarrollo de mi aplicación ebusiness debo escoger una pasarela de pago? ¿Valen todas para todo?"
---

A menudo recibo preguntas sobre cómo resolver un problema generado por la pasarela. A veces es por los límites impuestos por el banco que realiza la adquirencia (ver [Trabajar con bancos](/bancos/)), otras por el índice de rechazo, algunas otras porque lo que prometían no lo han cumplido. Y es que **no todas las pasarelas son iguales** y una vez escogida una, cambiarla puede ser costoso, o simplemente demasiado tarde.

**Una pasarela de pago debe servir al negocio**. La pasarela es la manera (o una de las maneras) que tendremos de cobrar a nuestros clientes y por tanto deberíamos prestar atención a su elección y hacerlo lo suficientemente temprano para estar seguros de que se ajusta a nuestras necesidades. Tanto funcionales como en lo referente a tiempos de implementación y, por supuesto, a costes.

Imaginemos que necesitamos una pasarela que nos permita gestionar pagos recurrentes. Como un amigo utiliza la pasarela A en su proyecto y para él tiene un coste del 1%, hacemos nuestros cálculos con esa pasarela y ese número en la cabeza. ¿Correcto?, no. No sería de extrañar que nos encontrásemos con alguna desagradable situación bien avanzado el desarrollo. Por citar algunas que he vivido cerca:

- que tardemos dos meses en tener disponible nuestra pasarela. Tiempo que tardaremos en poder operar.
- que pasadas varias semanas desde la solicitud nos informen que no nos la pueden ofrecer porque nuestro negocio es demasiado nuevo y tengamos que volver a empezar.
- que como nuestras circunstancias no son las de nuestro amigo el coste es del doble y nos rompe el plan de negocio.
- que aunque nos dijeron que la pasarela soportaba pagos recurrentes al final _no son exactamente pagos recurrentes_ y tengamos que cambiar nuestro modelo negocio porque de cambiar no nos salen los números.
- que como queremos ofrecer planes anuales debemos suscribir un aval bancario o dejar un % bloqueado durante X meses como fondo de garantía y no lo teníamos presupuestado.

Idealmente deberíamos contratar nuestra pasarela antes de empezar nuestro proyecto pero eso es una tarea casi imposible. Pero lo que si podemos hacer es prestar atención a su elección: hablar con amigos, pedir referencias, documentarnos con ellos, ver que usa la competencia, etc. Cualquier cosa menos ir a ciegas con algo tan importante. 

Si me lo preguntáseis a mí, ¿qué querría saber yo antes de recomendaros alguna pasarela?. Dependería del negocio, pero algunas de ellas saldrían de la siguiente lista

- ¿Vendes productos físicos?
- ¿Tienes 1 operación al día o 100?, ¿1000?
- ¿De importes pequeños o grandes?
- ¿Necesitas empezar a operar rápido?, ¿realmente rápido?
- ¿Es para el negocio Secure3D obligatorio o en absoluto deseado?
- ¿Es un negocio de subscripción?, ¿con cantidades variables?
- ¿Necesitas cobrar en divisas?, ¿y únicamente en divisas? 
- ¿Son tus clientes principalmente empresas o particulares?
- ¿Españoles o de cualquier parte del mundo?
- ¿Vienen tus clientes a comprarte repetidamente o lo normal es que lo hagan una única vez?

Y es que no es lo mismo [Stripe](/stripe/) que [Paymill](/paymill/), [Redsys/Sermepa](/redsys) que [Braintree](/braintree/), [Tefpay](/tefpay/) que [Paypal](/paypal/), [Adyen](/adyen/) que [Ceca](/ceca/) o [Wirecard](/wirecard/) que [Pagantis](/pagantis/).

**Intentar que el uso de una pasarela nos cueste lo menos posible es un objetivo, pero ni mucho menos debe ser el único**. Porque si la pasarela escogida no se ajusta a nuestras necesidades el coste para el negocio puede ser demoledor. A fin de cuentas una diferencia del 1% en la tasa de descuento significa únicamente €10 por cada €1000 vendidos, un precio mucho menor de lo que nos puede costar equivocarnos en términos de esfuerzo de desarrollo, en transacciones perdidas o en *time-to-market*.


