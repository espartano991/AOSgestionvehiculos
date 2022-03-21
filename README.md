# AOSgestionvehiculos

> Atributos finales:
- vin (string)
- matricula (string)
- marca (string)
- modelo (string)
- motor (cilindrada, CV, tipo de motor) (Text)
- año (int)
- reparación (fecha ultima reparación) (Text) 
> Atributos obligatorios para post:
- Matrícula
- Marca
- Modelo
- Motor
- Año

## Mockup:

coche  
  GET  
  POST  
    body: {  
	  Matrícula  
	  Marca  
	  Modelo: (string)  
	  Motor: (Text)  
	    {  
		  cilindrada, (int)  
		  CV, (int)  
		  tipo de motor (enum)  
		    [  
			  diesel,  
			  gasolina,  
			  híbrido,  
			  eléctrico  
			]  
	    }  
      Año: (Date ? Date : int)  
	  Reparación: (Text)  
	    {  
		  fecha_reparacion (Date ? Date : int)  
		  ¿Más cosas? ¿Nos salimos del scope?  
		}  
	}  
  PUT  

coche/{vin} (string)  
  GET  
  PUT  
  DELETE  
  
coche/{matricula} (string)  
  GET  
  PUT  
  DELETE  
  
coche/{marca} (string)  
  GET  
  
coche/{año} (int)  
  GET  
