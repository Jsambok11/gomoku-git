```mermaid
classDiagram
    direction TB

    class Spel {
    }

    class Resultat {
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

    class ´Vinst/Förlust´ {
    }

    class Oavgjort {
    }

    %% Relationer
    Spel -- Resultat : får
    Spel -- Spelare : deltagare
    Spel -- Bräde : spelplan
    Spel -- Tur : består av
    Bräde -- Ruta : består av
    Ruta -- Sten : kan innehålla
    Tur -- Spelare : utförs av
    Tur -- Ruta : sker på
    Spelare -- Sten : spelar med
    Resultat -- ´Vinst/Förlust´ : kan vara
    Resultat -- Oavgjort : kan vara
```