```mermaid
classDiagram
    direction TB

    class Spel {
    }

    class Spelare {
    }

    class Bräde {
    }

    class Ruta {
    }

    class Sten {
    }

    class Tur {
    }

    class Resultat {
    }

    %% Relationer
    Spel *--  Spelare
    Spel *--  Bräde
    Spel *--  Tur
    Spel -->  Resultat

    Bräde *-- Ruta
    Ruta o-- Sten

    Tur --> Spelare
    Tur --> Ruta

    Spelare -- Sten
```