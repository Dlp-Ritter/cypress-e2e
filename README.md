# cypress-e2e-suite

Suite de tests E2E automatizados con Cypress sobre [Sauce Demo](https://www.saucedemo.com) — una tienda de e-commerce de práctica. Cubre flujos de autenticación, catálogo de productos y proceso de checkout.

> Mi primer acercamiento serio a testing automatizado. Vengo de un perfil
> más de sistemas/infraestructura, así que aquí documento también lo que
> voy aprendiendo sobre Cypress y buenas prácticas de QA.

---

## Demo

![Demo](cypress/assets/demo.gif)

---

## Tests incluidos

### Auth (`cypress/e2e/auth/login.cy.js`)
- Login exitoso con credenciales válidas
- Error con usuario bloqueado
- Error con credenciales inválidas
- Logout exitoso

### Products (`cypress/e2e/products/catalog.cy.js`)
- Muestra 6 productos después del login
- Ordenar productos de menor a mayor precio
- Agregar producto al carrito
- Ver detalle de un producto

### Checkout (`cypress/e2e/checkout/checkout.cy.js`)
- Completar proceso de compra end-to-end
- Checkout con carrito vacío
- Error si faltan datos en el formulario

---

## Stack

![Cypress](https://img.shields.io/badge/Cypress-17202C?style=flat-square&logo=cypress&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=nodedotjs&logoColor=white)

---

## Estructura

```
cypress-e2e/
├── cypress/
│   ├── e2e/
│   │   ├── auth/
│   │   │   └── login.cy.js
│   │   ├── products/
│   │   │   └── catalog.cy.js
│   │   └── checkout/
│   │       └── checkout.cy.js
│   ├── fixtures/
│   │   └── users.json
│   └── support/
│       ├── commands.js
│       └── e2e.js
├── cypress.config.js
├── package.json
├── .gitignore
└── LICENSE
```

---
## Instalación

```bash
git clone https://github.com/Dlp-Ritter/cypress-e2e
cd cypress-e2e
npm install
```

## Correr los tests

Modo interactivo (abre Cypress):

```bash
npx cypress open
```

Modo headless (terminal):

```bash
npx cypress run
```

---

## Cómo se integra en mi portafolio

Este repo es parte de un flujo más grande:

- [`docker-infra`](https://github.com/Dlp-Ritter/docker_infra) — la app Node.js/Nginx contra la que en el futuro pienso adaptar estos tests (actualmente corren contra Sauce Demo como entorno de práctica).

---

## Contacto

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=flat-square&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/duglas-pop-guitz-490ab72b0)
[![Email](https://img.shields.io/badge/Email-8B89CC?style=flat-square&logo=protonmail&logoColor=white)](mailto:duglas_leonel_1704@protonmail.com)

