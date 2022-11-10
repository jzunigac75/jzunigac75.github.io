---
layout: single
title: Interfaces Digitales para equipos analógicos
excerpt: "Existen centrales telefónicas con marcadores analógicos que se convierten en señales digitales para capturar el consumo de los abonados"
date: 1995-09-30
classes: 
header: 
  teaser: 
  teaser_home_page: true
  icon: 
categories:
  - Programación
tags:  
  - C++
  - Clipper
---

## Roles en el proyecto

- Programación

## Situación

El Instituto Costarricense de Electricidad cuenta con centrales analógicas que mediante relojes análogos marcan el consumo de los abonados. A dichos marcadores se les toma fotos todos los meses y los datos de las fotos son digitados y comparados con el mes anterior para poder calcular el consumo.

## Solución

Para automatizar el cálculo del consumo se unen dos equipos de ingeniería, uno eléctrico que crea las tarjetas de interface con la central y otro informático que crea la interface programática que lee el puerto RS232 y va almacenando los resultados en un motor de base de datos que luego será utilizada para el cálculo del consumo evitando la toma de fotografías y reingreso de datos.