---
layout: gateway
title:  "Addon Payments"
date:   2017-04-19 10:02:36
categories: pasarelas insite offsite recurring oneshot prestashop magento woocommerce shopify


gw_logo: "/images/gateways/addonpayments.jpg"
gw_url: "https://www.addonpayments.com/es-es/"
gw_slogan: "Nosotros nos ocupamos de los pagos mientras tú te ocupas de tu negocio"
gw_country: España
gw_fee: "€19/mes fijos + 0,09 + Tasa de descuento de tu banco"
gw_twitter: 'AddonPayments'
gw_docs: 'https://desarrolladores.addonpayments.com/'
---

Addon Payments es una solución de [Comercia Global Payments](https://www.comerciaglobalpayments.com) la empresa en la que [CaixaBank](https://www.caixabank.es) concentra sus servicios de pago. A falta de confirmación oficial, mi apuesta es que es una capa sobre [Redsys](/redsys/) o procesador similar, porque si no no tiene sentido el pricing (X + la tasa de descuento del banco de la empresa).

Está bien que los bnaco tradicionales vayan dando valor al procesamiento de los pagos, si bien no me inspira especial confianza casos como el del BBVA con [Nimble Payments](/nimble/), que fue discontinuado un par de años después de sacarlo al mercado. Pero si por margen u otro tipo de restricciones te ves obligado a usar Redsys, yo al menos lo probaría.

Que puedas a través de una única integración ofrecer métodos de pago alternativos como Paypal o Sofort tampoco está mal.


-------------

#### Funciones

- Pagos únicos
- Tokenización de tarjeta y cargos posteriores, pero sin gestión de recurrencia por su parte
- Integración con Paypal y Sofort, próximamente Apple Pay.
- Pagos fracciones: próximamente.
- TPV para venta telefónica. Algo poco habitual.


-------------

#### Tecnología

La parte de API se basa en ficheros XML, algo que personalmente no me gusta demasiado, pero podría ser peor :). Si vas a hacer un uso amplio de su API deberías tener en cuenta que a) debes cumplir con PCI, y b) que su API no es del todo completa, sobre todo en lo que a gestión de recurrencia respecta (a día de hoy, gestión inexistente). Interesante que tienen incluso la gestión del 3D Secure por API, no es muy normal.

Tiene librerías de Android, iOS, Javascript, Java y PHP.

Si no quieres complicarte, tienen páginas alojadas para hacer toda la gestión de las transacciónes, almacenamiento, en su sitio. Sale el logo de La Caixa, que puede ser bueno de cara a dar seguridad al comprador.



-------------

#### Módulos ecommerce

- [Prestashop](https://desarrolladores.addonpayments.com/#!/other-integration/shopping-carts/prestashop)
- [Magento](https://desarrolladores.addonpayments.com/#!/other-integration/shopping-carts/magento)
- [WooCommerce](https://desarrolladores.addonpayments.com/#!/other-integration/shopping-carts/woocommerce)
- [Shopify](https://desarrolladores.addonpayments.com/#!/other-integration/shopping-carts/shopify)
- [Opencart](https://desarrolladores.addonpayments.com/#!/other-integration/shopping-carts/opencart)
