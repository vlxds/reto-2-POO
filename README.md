# reto-2-POO

## Diagrama UML
 ´´´mermaid
 classDiagram
direction TB
    class AireAcondicionado {
	    modelo
	    capacidad
	    tipo de instalación
	    tamaño
	    eficiencia
	    garantia
	    tipo de refrigerante
	    encender()
	    apagar()
	    ajustar Temperatura()
	    establecer tienpo de encendido()
	    mostrar Información()
    }

    class Compresor {
	    potencia
	    caudal
	    Tamaño del tanque
	    Tipo
	    Ruido
	    eficiencia
	    iniciar()
	    detener()
    }

    class Condensador {
	    dimensiones
	    eficiencia
	    potencia
	    tipo de ventilador
	    encender ventilador()
	    apagar ventilador()
	    disipar Calor()
    }

    class Evaporador {
	    capacidad
	    temperatura
	    Caudal
	    dimensiones
	    encender ventilador()
	    apagar ventilador()
	    absorver calor()
    }

    class ValvulaExpansion {
      tipo de valvula
      capacidad
      dimensiones
      caida de presión maxima
	    regular presion del refrigerante()
    }

    class SensorTemperatura {
	    rango de temperatura
	    velocidad de respuesta
	    precion y exactitud
	    tipo de sensor
	    medir()
	    enviar Datos()
    }

    AireAcondicionado <-- Compresor
    AireAcondicionado <-- Condensador
    AireAcondicionado <-- Evaporador
    AireAcondicionado <-- ValvulaExpansion
    AireAcondicionado <-- SensorTemperatura


 ´´´
