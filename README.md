# Presentación en Línea de las Clases de Autómatas

>[!NOTE]
> Esta presentación utiliza la librería [reveal.js](https://revealjs.com/) para una experiencia interactiva.

>[!WARNING]
> **Advertencia:** La teoría de autómatas puede parecer abstracta al principio, ¡pero la práctica constante es clave para dominarla!

>[!TIP]
> **Tip:** Dibuja diagramas de estados a mano.  ¡La visualización es tu mejor amiga!

>[!IMPORTANT]
> **Importante:** Comprende la diferencia entre un Autómata Finito Determinista (AFD) y un Autómata Finito No Determinista (AFN).  Es un concepto fundamental.

>[!CAUTION]
> **Precaución:** ¡No confundas el alfabeto con el lenguaje! El alfabeto son los símbolos permitidos, el lenguaje son las cadenas válidas formadas por esos símbolos.

## Diagrama Visual de Conceptos Clave

```mermaid
graph LR
    A[Alfabeto (Σ)] -- Contiene --> B(Símbolos);
    C[Cadena (String)] -- Compuesta por --> B;
    D[Lenguaje (L)] -- Conjunto de --> C;
    E[Autómata] -- Procesa --> C;
    E -- Acepta/Rechaza --> D;
    F[Estados] -- Componente de --> E;
    G[Transiciones] -- Componente de --> E;
    H[Estado Inicial] -- Componente de --> E;
    I[Estado de Aceptación] -- Componente de --> E;

    style A fill:#f9f,stroke:#333,stroke-width:2px
    style E fill:#ccf,stroke:#333,stroke-width:2px
```