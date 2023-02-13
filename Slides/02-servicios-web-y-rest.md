---
title       : Servicios web y REST
author      : 
  - Alberto Díaz Álvarez <alberto.diaz@upm.es>
  - Francisco Serradilla García <francisco.serradilla@upm.es>
description : Qué son los servicios web y qué es el conjunto de principios REST para la descripción de API
keywords    : Servicios, Web, REST, Agentes, Recolección, Información, Internet.
marp        : true
paginate    : true
theme       : etsisi
--- 
<!-- _class: titlepage -->

# Servicios web y REST

## Agentes de extracción de información en Internet

### Alberto Díaz Álvarez y Francisco Serradilla García

#### 10 de febrero de 2023

##### Departamento de Sistemas Informáticos - ETSISI - UPM

[![height:30](https://img.shields.io/badge/License-CC%20BY--NC--SA%204.0-informational.svg)](https://creativecommons.org/licenses/by-nc-sa/4.0/)

---

# Servicios web

Un servicio web es un conjunto de protocolos y estándares que permiten la comunicación entre aplicaciones

- Se basan en estándares abiertos que funcionan sobre el protocolo HTTP
- Su origen proviene de estándares de ejecución remota de código de los 90
- Un conjunto de servicios web con propósito común se denomina API (*Application Programming Interface*)
- Pueden estar documentados también para máquinas usando WSDL (_Web Services Description Language_)

En la actualidad, estos estándares están en desuso por el auge de la web

- La transmisión de datos es a través del puerto 80 o 443 (adios *firewalls*)
- Protocolos que funcionan sobre un estándar ya probado (SOAP)
- O simplemente conjuntos de pautas para hacer la comunicación más ligera (REST)

---

# Acerca de REST

*Representational State Transfer* (REST) es un estilo de arquitectura de software

- No es un protocolo, es un conjunto de principios para la creación de servicios web

Sus principios arquitectónicos son:

- **Interfaz uniforme**: La información se envía en un formato estándar (XML, JSON, etc.)
- **Sin estado**: El servidor completa solicitudes independientes (es inherente a HTTP)
- **Distribuido**: Permite que varios servidores trabajen juntos
- **Almacenamiento en caché**: Ayuda a mejorar el rendimiento
- **Código bajo demanda**: El servidor puede enviar código al cliente para que lo ejecute

Las API que siguen la arquitectura de REST se llaman **API RESTful**

---

# API RESTful

Son aquellos **servicios web que implementan una arquitectura REST**

Requieren que las peticiones contengan los siguientes **elementos principales**:

- **URL**: La ruta hacia el recurso o servicio
- **Método**: La acción que se quiere realizar sobre el servicio, que suelen ser:
  - `GET`: Para obtener listas (e.g. `GET /games`) o elementos (e.g. `GET /game/1`)
  - `POST`: Para enviar información o crear elementos (e.g. `POST /game`)
  - `PUT` o `PATCH`: Para actualizar elementos (e.g. `PUT /game/1`)
  - `DELETE`: Para eliminar elementos (e.g. `DELETE /game/1`)
- **Cuerpo**: La información enviada al servidor (para peticiones `POST`, `PUT` o `PATCH`)
- **Cabeceras**: Información adicional de la petición, (e.g. datos de autenticación)

Es un estándar muy usado en la actualidad, pero no es obligatorio

---

Gracias<!-- _class: endpage -->
