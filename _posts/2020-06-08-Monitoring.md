---
layout: single
title: Logging and Monitoring Platform
excerpt: "Proveer de una plataforma única de monitoreo al equipo de desarrollo para ser utilizada en los nuevos proyecto asi como adaptable a los proyectos ya implementados."
date: 2020-06-08
dateto: 2020-12-31
classes: 
header: 
  teaser: 
  teaser_home_page: true
  icon: 
categories:
  - Investigación
  - Integración
  - Coordinación
tags:  
  - Elastic Search
---

## Roles en el proyecto

- Coordinación
- Investigación

## Situación

Cada proyecto crea su propia implementación de registro de eventos en diferentes repositorios, ya sea base de datos, archivos planos, json, xml, registro de enventos en windows, etc. Se pretende crear una sola plataforma que sea utilizada por todas las aplicaciones que además posea la capacidad de alertar creando los incidentes en la herramienta de incidentes de la empresa controlando cuando se abre y cierran automáticamente sin saturar la creación por un mismo incidente que permaneza abierto.

## Solución

Se hace la investigación necesaria y se encuentran dos herramientas que cumplen con lo esperado. 

- [Elastic Search](https://www.elastic.co/es/elastic-stack/)
- [Splunk](https://www.splunk.com/en_us/products.html)

Dado que ElasticSearch cuenta con una licencia OpenSouce se hace el piloto utilizando las herramientas del stack de elastic con:

- [Kibana](https://www.elastic.co/es/kibana/): Confección de tablero
- [LogStash](https://www.elastic.co/es/logstash/): Recolección de logs
- [ElasticSearch](https://www.elastic.co/es/elasticsearch/): Repositorio y motor de búsqueda
  
Para poder hacer un switch a futuro se creo un adaptador que es el que consumen las aplicaciones y que luego permitirá cambiar el motor de búsqueda.

Para contar con un tablero universal se confeccionó un solo formato de log para todas las nuevas aplicaciones y mediante logstash recolectar y transformar viejos logs en el nuevo formato de tal forma que se logró contar con un solo tablero de Monitor.

Se hizo el piloto con el procesamiento de facturas electrónicas y se catalogó como un éxito el poder localizar los problemas que se presentaban sin necesidad del ingreso a ambientes de producción para determinar la solución. A ello se sumó que los mismos logs dieron información necesaria para generar métricas de rendimiento (KPIs).

