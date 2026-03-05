# Actividades-Casos-De-Uso
Diagramas de Casos De Uso en Mermaid

Ejercicio 1.

<pre>
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

    %% Estética opcional: Colores para diferenciar
    style Usuario fill:#f9f,stroke:#333,stroke-width:2px
    style App_Iluminacion fill:#f5f5f5,stroke:#666,stroke-dasharray: 5 5

    </pre>
 
 Ejercicio 2.

<pre>
graph LR
    %% Actores
    Cliente((Cliente))
    Admin((Administrador))

    subgraph Tienda_Online [Sistema de Tienda]
        UC1(Comprar Producto)
        UC2(Gestionar Stock)
        UC3(Aplicar Cupón Descuento)
    end

    %% Interacciones principales
    Cliente --&gt; UC1
    Admin --&gt; UC2

    %% Relación de Extensión (Opcional)
    %% La flecha va de la extensión hacia el caso base
    UC3 -.-&gt;|&amp;lt;&amp;lt;extend&amp;gt;&amp;gt;| UC1

    %% Estilos para mayor claridad
    style Cliente fill:#e1f5fe,stroke:#01579b
    style Admin fill:#fff3e0,stroke:#e65100
    style UC3 fill:#f1f8e9,stroke:#33691e
    
      </pre>