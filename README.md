# Actividades-Casos-De-Uso

Diagramas de Casos De Uso en Mermaid

Ejercicio 1.

```mermaid
graph LR
    %% Definición del Actor con estilo de nodo circular
    Usuario((Usuario))

    %% Límite del Sistema
    subgraph App_Iluminacion [Aplicación Móvil]
        UC1(Encender luces)
        UC2(Apagar luces)
    end

    %% Relaciones de interacción
    Usuario --> UC1
    Usuario --> UC2

```
 
 Ejercicio 2.

```mermaid
graph LR
%% Definición de Actores
Cliente((Cliente))
Admin((Administrador))
subgraph "Sistema de E-commerce"
%% Casos de Uso
CU1([Comprar Producto])
CU2([Aplicar Cupón Descuento])
CU3([Gestionar Stock])
%% Relación de Extensión (Opcional)
%% La flecha apunta del extensor al base
CU2 -.->|&lt;&lt;extend&gt;&gt;| CU1
end
%% Relaciones de los Actores
Cliente --- CU1
Admin --- CU3
```
Ejercicio 3.

```mermaid

     graph LR
    %% Actores
    Espectador((Espectador))
    Editor((Editor de Contenido))
    Pasarela[Pasarela de Pagos]

    subgraph Sistema_Streaming [Plataforma de Streaming]
        UC1(Reproducir Película)
        UC2(Subir Nuevo Video)
        UC3(Renovar Suscripción)
        UC4(Validar Suscripción)
        UC5(Activar Subtítulos)

        %% Relaciones internas (UML)
        UC1 -.->|include| UC4
        UC5 -.->|extend| UC1
    end

    %% Interacciones de los Actores
    Espectador --- UC1
    Espectador --- UC3
    Editor --- UC2
    UC3 --- Pasarela

  ```
    
