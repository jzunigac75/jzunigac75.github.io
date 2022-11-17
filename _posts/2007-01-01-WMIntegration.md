---
layout: single
title: Integración sistemas Walmart
excerpt: "Con motivo de la adquisisión de la Walmart de la Corporación Supermercados Unidos se dará una sustitución gradual de los sistemas globales por los locales, inialmente en un plazo de tres años."
date: 2007-01-01
dateto: 2009-06-01
classes: 
header: 
  teaser: 
  teaser_home_page: true
  icon: 
categories:
  - Integración
tags:  
  - .Net Framework
  - C#
  - SQL
  - SSIS
  - SSRS
  - SQL Server
---

## Roles en el proyecto

- Programación
- Arquitectura de Soluciones
- Coordinación

## Situación

Se requiere diseñar una interace entre los sistemas de WM y los sistemas locales de tal forma que pueden convivir al mismo tiempo y se apaguen las funcionalidades del sistema local miestrs se van sustituyendo por el sistema global. La información viajará en dos dos sentidos. 

## Solución

Se diseñeron las interfaces de lo que se denominó en su momento la Capa Media que era la encargada de enviar y recibir la información entre los dos sistemas, dicha implementación llegó a ser la primera de Walmart que se hizo en tiempo y de forma efectiva, aún con la complejidad de que integraba cinco paises con políticas, impuestos, monedas diferentes. Razón por la cual al final todo el equipo fue premiado por el trabajo realizado.

Todas las interfaces se hicieron con SSIS apoyados por los reportes en SSRS asi como sitios de monitoreo con Visual Studio c#. Éste fue un proyecto que se duraron mas de seis meses deserrándolo por la cantidad de interfaces que se tenían que crear y al cual se dio soporte por tres años y que derivó luego en un equipo dedicado a la Datawarehowse que siguieron utilizando SSIS y luego Alterix.



