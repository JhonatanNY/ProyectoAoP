# 📅 Spring Boot - AOP (Aspect-Oriented Programming)

Este es un proyecto desarrollado con **Spring Boot**, donde implemento **AOP (Programación Orientada a Aspectos)** para aplicar funcionalidades transversales como podria ser logging, etc y control de ejecución de métodos sin modificar la lógica principal.

---

## 🚀 Tecnologías usadas

* Java
* Spring Boot
* Spring AOP
* Spring MVC
* Maven

---

## 📌 ¿Qué estoy aprendiendo?

En este proyecto refuerzo conceptos clave como:

* Uso de **AOP en Spring Boot**
* Creación de **Aspectos (`@Aspect`)**
* Tipos de Advice:

  * `@Before` → antes del método
  * `@After` → después del método
  * `@AfterReturning` → cuando termina correctamente
  * `@AfterThrowing` → cuando ocurre un error
  * `@Around` → controla toda la ejecución
* Definición y reutilización de **Pointcuts**
* Uso de **JoinPoint y ProceedingJoinPoint**
* Control del orden de ejecución con `@Order`

---

## ⚙️ ¿Cómo funciona?

La aplicación expone endpoints REST que llaman a un servicio (`GreetingService`).
A través de AOP, se interceptan sus métodos para ejecutar lógica adicional automáticamente.

### Endpoints:

* `/greeting` → retorna un mensaje exitoso
* `/greeting-error` → lanza una excepción para probar manejo de errores

---

## 🔍 ¿Qué hace AOP en este proyecto?

Se implementan múltiples aspectos que:

* Registran una simulacion de logs antes y después de ejecutar métodos
* Capturan el resultado cuando el método finaliza correctamente
* Detectan y registran errores cuando ocurre una excepción
* Interceptan métodos usando `@Around` para controlar la ejecución completa
* Permiten definir el orden de ejecución entre aspectos con `@Order`

---

## 🧠 Conceptos clave (resumen rápido)

* **Aspect** → clase que contiene la lógica AOP
* **Advice** → acción que se ejecuta (before, after, etc.)
* **Pointcut** → expresión que define dónde aplicar AOP
* **JoinPoint** → método interceptado en ejecución

---

## 🎯 Objetivo

Desacoplar lógica transversal (como logging y manejo de errores) de la lógica de negocio, logrando un código más limpio, reutilizable y mantenible.

---

## 📌 Autor

**Jhonatan Nuñez**

