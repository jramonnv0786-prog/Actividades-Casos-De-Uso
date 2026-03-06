## Ejercicio 1 Justificación.

## Usuario (Actor Principal) Actor humano externo al sistema. En este caso inicia las interaccciones
## con el fin de modificar el estado físico de la iluminación en su hogar.

## El Limite Del Sistema: El uso de subgraph delimita qué funcionalidades pertenecen estrictamente a la app móvil. Así separa la interfaz de usuario.

## Caso de Uso (UC1,UC2) :  Representan funciones específicas.

## Ejercicio 2.

## El Cliente: Actor Primario, interactuando con la parte FRONTEND del sistema. Como objetivo principal es el valor del negocio (Comprar Producto).

## El Administrador (Actor de Soporte/Gestión): Interactúa con el Backend o la lógica operativa. Su función "Gestionar Stock" es un proceso de mantenimiento necesario para que el sistema sea funcional.

## Relación Extensión: (<Extends>): Uno de los puntos más interesantes del diagrama. La relación entre "Aplicar Cupón Descuento" UC3 y "Comprar Producto" UC1 está correctamente modelada: 
## - Opcionalidad: El uso de extensión es opcional. Se puede aplicar compra sin necesidad de cupón.
## - Sentido De La Flecha: En UML, las flechas de extensión nacen del comportamiento adcional (cupón) y apunta al caso base, en este caso (La compra). Esto indica que el primero se "incorpora" en el segundo bajo ciertas condiciones. 


## Ejercicio 3.
