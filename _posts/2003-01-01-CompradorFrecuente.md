---
layout: single
title: Programa de Comprador Frecuente
excerpt: "Solución que permite identificar las compras por cliente y asignar puntos de acuerdo a artículos comprados, grupo de artículos o por monto de compras."
date: 2003-01-01
classes: 
header: 
  teaser: 
  teaser_home_page: true
  icon: 
categories:
  - Programación
  - Integración
tags:  
  - SQL
  - SQL Server
  - C#
  - .Net Framework
  - C++
---

## Roles en el proyecto

- Programación

## Situación

Se requiere identificar centralizadamente las compras de los clientes para establecer un programa de comprador frecuente. Cómo parte de los incentivos se pretende otorgar puntaje de acuerdo a los artículo comprados, grupo de artículos o monto de ventas. Además en su momento con el motivo del 50 aniversario de la empresa se otorgarán acciones que luego serán utilizadas para rifar casas de habitación.

## Solución

El controlador de cajas genera el TLOG como un archivo binario para el cual se crea un extractor y luego se envía dicha información a las oficinas centrales, allí se crean los ETL necesarios para procesar la información y almacenarla en la base de datos. Por medio de procedimientos almacenados se hacen todos los cálculos para optimizar el manejo de la información y se acompaña par una solución de comprador frecuente que administra las reglas de asignación de puntos asi como diferente reporte y gráficas que permiten medir la fidelidad de los clientes.
