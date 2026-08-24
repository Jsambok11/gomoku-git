```mermaid
classDiagram
    direction TB

    class Spel {
    }

    class Spelare {
    }

    class Tur {
    }

    class Brädet {
    }

    class Sten {
    }

    class `Vann/Förlust` {
    }

    class Oavgjort {
    }

    %% Relationer
    Spel "1" *-- "2" Spelare : a
    Spel "1" *-- "1" Brädet : a
    Spel "1" *-- "0..*" Tur : a
    
    Tur "1" --> "1" Spelare : a
    Tur "1" --> "1" Sten : a

    Spelare "1" o-- "1..*" Sten : a
    Brädet "1" o-- "0..*" Sten : a

    Spel "1" --> "0..1" seger/förlust : a
    Spel "1" --> "0..1" Oavgjort : a
```
