# React.js Library

Este repositorio proporciona una introducción a React.js, una biblioteca de JavaScript desarrollada por Facebook para construir interfaces de usuario.

## ¿Qué es React?

React es una biblioteca declarativa, eficiente y flexible para construir interfaces de usuario. Permite crear componentes reutilizables que manejan su propio estado y se pueden combinar para construir interfaces complejas.

## Principales Características

- **Componentes Declarativos:** React se basa en componentes, que son unidades de código encapsuladas que representan partes de la interfaz de usuario.
- **Virtual DOM:** Utiliza un árbol de objetos en memoria (Virtual DOM) para minimizar el acceso al DOM real y mejorar el rendimiento.
- **Unidirectional Data Flow:** El flujo de datos es unidireccional, lo que facilita la gestión del estado y la depuración de aplicaciones.
- **JSX:** Utiliza JSX, una extensión de la sintaxis de JavaScript que permite escribir estructuras de HTML dentro del código JavaScript.

## Instalación

Para comenzar a usar React en tu proyecto, primero necesitas instalarlo. A continuación se muestra cómo hacerlo utilizando npm:

```sh
npx create-react-app my-app
cd my-app
npm start

## Estructura Básica de un Componente

import React from 'react';

function MiComponente() {
  return (
    <div>
      <h1>¡Hola, mundo!</h1>
      <p>Este es mi primer componente en React.</p>
    </div>
  );
}

export default MiComponente;

## Ciclo de Vida de un Componente

React ofrece métodos de ciclo de vida que permiten ejecutar código en diferentes etapas del ciclo de vida de un componente:

componentDidMount()

componentDidUpdate()

componentWillUnmount()

Estos métodos se utilizan para manejar tareas como la obtención de datos, la actualización del DOM y la limpieza de recursos.

## Hooks

Hooks son una adición reciente a React que permiten usar el estado y otras características sin escribir una clase. Los dos hooks más comunes son:

useState(): Permite agregar estado local a los componentes funcionales.

useEffect(): Permite realizar efectos secundarios en los componentes funcionales.

Ejemplo de uso de hooks:

javascript

import React, { useState, useEffect } from 'react';

function Contador() {
  const [count, setCount] = useState(0);

  useEffect(() => {
    document.title = `Has clickeado ${count} veces`;
  }, [count]);

  return (
    <div>
      <p>Has clickeado {count} veces</p>
      <button onClick={() => setCount(count + 1)}>Click me</button>
    </div>
  );
}

export default Contador;


## Para más detalles, consulta la documentación oficial de React.
