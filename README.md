﻿# Punto de Venta
##### SuperMarket: Los Monitos de la Nona.


###### Librerias a descargar
- Framework Flask --- pip install Flask
- MySQL connector --- pip install mysql-connector

#### Estados de Avances:
- Autentificacion (login): OK.
- Pagina principal (presentacion) : falta mejorar estetica, funcional ok.
- catalogo principal (visible para el publico en general): OK.
- CRUD Administrador de Trabajadores: OK.
- CRUD Gestionador de Inventario: crd OK. update falta corregir bug de formulario.


#### Funciones A Desarrollar:
##### Interfaz de Ventas del Vendedor
- Poder agregar productos a ser adquiridos por un potencial cliente, detallándose: 
		 Cantidad. 
		Nombre del producto. 
		Código del producto. 
		Valor unitario. 
		Total por producto (cantidad * costo unitario). 
		Valor del IVA al 19%
 **IMPORTANTE**:
######Requeriemientos funcionales:
- Se deberá poder agregar más de un tipo de producto a una venta, y se deberá calcular el total a ser cancelado por el cliente. 
-  Se debe almacenar cada venta realizada en la base de datos, que contenga lo anterios detallado y una clave primaria para identificarla mas tarde.
- Se debe tener la opcion de buscar productos mediante su NOMBRE o CODIGO.
- Debe tener la posibilidad de emitir boleta o factura.

######Requeriemientos  NO funcionales:

 - Solo el trabajador con rol de VENDEDOR puede generar ventas.
 - Solo se puede generar ventas si el estado de jornada esta ABIERTA. Este estado solo lo puede modificar el Administrador o Jefe.




##### Administrar Jornada
######Funcion Unica del Administrado/Jefe

Se debe implementar la opcion para abrir/cerrar la jornada. lo cual permitira generar ventas al vendedor.
Al cerrar la jornada se debe generar el informe de venta automaticamente.


##### Informe de Ventas
######Funcion Unica del Administrado/Jefe

El informe de ventas del día (visible sólo para el jefe de ventas), deberá indicar: 
		1. Cantidad de ventas con boleta. 
		2. Cantidad de dinero por ventas con boleta, separando valor neto, IVA y total (neto + IVA). 
		3. Número de facturas generadas: 
			1. Por cada factura se deberá detallar: 
				1. Número de factura. 
				2. Valor en dinero, separando neto, IVA y total (neto + IVA). 
		4. El informe de ventas es de un día en particular, y deberá ser posible buscar informes de cualquier día que tenga ventas. 
En el informe de ventas, se deberá identificar al vendedor que estuvo trabajando en el día. 

 Se deberá proveer una opción para filtrar los informes de ventas por vendedor, listando sólo los días que dicho vendedor trabajó o generó ventas efectivamente. 
-- No deberán aparecer en el listado días donde el vendedor no trabajó o no realizó ventas.  
# pdv
