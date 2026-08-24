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

    class `Vinst/Förlust` {
    }

    class Oavgjort {
    }

    %% Relationer
    Spel -- Resultat : får
    Spel -- Spelare : deltagare
    Spel -- Bräde : består av
    Spel -- Tur : består av
    Bräde -- Ruta : består av
    Ruta -- Sten : kan innehålla
    Tur -- Spelare : utförs av
    Tur -- Ruta : sker på
    Spelare -- Sten : spelar med
    Resultat -- `Vinst/Förlust` : kan vara
    Resultat -- Oavgjort : kan vara
```

#### Spel
Spel är en enskild spelomgång av Gomoku

#### Spelare
Aktor som agerar i spelet

#### Bräde
Spelplan där spelet genomförs

#### Ruta
Unik punkt på brädet som man kan placera sten på

#### Sten
Spelmärke som spelare placerar i rutor

#### Tur
En Handling i spelomgång

#### Resultat
Slutliga tillstånd

#### Vinst/Förlust
Match som slutade med en spelare som placerade 5 stenar horizontalt, vertikalt och diagonal

#### Oavgjort
Matchen där ingen av spelare kunde placera 5 stenar horizontalt, vertikalt och diagonal