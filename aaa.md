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
    Spel -- Spelare : har deltagare
    Spel -- Bräde : har spelplan
    Spel -- Tur : har händelseförlopp
    Spel -- Resultat : får
    Bräde -- Ruta : består av
    Ruta -- Sten : kan innehålla
    Tur -- Spelare : utförs av
    Tur -- Ruta : sker vid
    Spelare -- Sten : spelar med
```