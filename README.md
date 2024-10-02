graph TD;
    A[Inicio] --> B{¿Identificar productos?};
    B -- Sí --> C[Investigar regulaciones];
    B -- No --> D[Finalizar proceso];
    
    C --> E{¿Documentación lista?};
    E -- Sí --> F[Solicitar cotizaciones];
    E -- No --> G[Reunir documentación];

    G --> E;

    F --> H{¿Seleccionar proveedor?};
    H -- Sí --> I[Realizar pedido];
    H -- No --> J[Evaluar cotizaciones];

    J --> F;

    I --> K[Organizar envío];
    K --> L{¿Recibir productos?};
    L -- Sí --> M[Verificar calidad];
    L -- No --> N[Esperar envío];

    M --> O{¿Todo en orden?};
    O -- Sí --> P[Registrar importación];
    O -- No --> Q[Reclamar al proveedor];

    P --> R[Fin];
    Q --> H;

    
