# AOSgestionvehiculos

> Atributos finales:
- vin (string)
- matricula (string)
- marca (string)
- modelo (string)
- motor (cilindrada, CV, tipo de motor) (Text)
- año (int)
- reparación (fecha ultima reparación) (Text) 
- clienteID (string)
- propósito (reparar o revisar) (enum)
> Atributos obligatorios para post:
- VIN
- Matrícula
- Marca
- Modelo
- Motor
- clienteID
- propósito
> Respuestas_HTTP:
- 200 OK
- 201 Created
- 400 Bad Request
- 403 Forbidden
- 401 unauthorized
- 404 Not Found
- 408 Request Timeout
- 500 Internal Server Error
## Mockup:

coche/  
  GET  
  POST  
  &nbsp;&nbsp;  body: {  
  &nbsp;&nbsp;&nbsp;&nbsp;	  Matrícula  
  &nbsp;&nbsp;&nbsp;&nbsp;	  Marca  
  &nbsp;&nbsp;&nbsp;&nbsp;	  Modelo: (string)  
  &nbsp;&nbsp;&nbsp;&nbsp;	  Motor: (Text)  
  &nbsp;&nbsp;	    {  
  &nbsp;&nbsp;	    cilindrada, (int)  
  &nbsp;&nbsp;	    CV, (int)  
  &nbsp;&nbsp;      tipo de motor (enum)  
&nbsp;&nbsp;&nbsp;&nbsp;  [  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;  diesel,  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;  gasolina,  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;  híbrido,  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;  eléctrico  
&nbsp;&nbsp;&nbsp;&nbsp;  ]  
  &nbsp;&nbsp;      }  
&nbsp;&nbsp;  Año: (Date ? Date : int)  
&nbsp;&nbsp;  Reparación: (Text)  
&nbsp;&nbsp;&nbsp;&nbsp;  {  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;  fecha_reparacion (Date ? Date : int)  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;  ¿Más cosas? ¿Nos salimos del scope?  
&nbsp;&nbsp;&nbsp;&nbsp;  }  
&nbsp;&nbsp;  }  
  PUT  

coche/{vin}/ (string)  
  GET  
  PUT  
  DELETE  
  
coche/{matricula}/ (string)  
  GET  
  PUT  
  DELETE  
  
coche/{marca}/ (string)  
  GET  
  
coche/{año}/ (int)  
  GET  
