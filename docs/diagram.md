# Diagram – Aplikacja do planowania nauki

```mermaid
flowchart TD
    START([START])
    LOGIN[Logowanie / Profil użytkownika]
    EDIT[Dodaj / Edytuj zadanie]
    LISTA[Lista zadań]
    SYNC[Synchronizacja / przypomnienia]
    KALENDARZ[Kalendarz tygodniowy]
    STATY[Proste statystyki (postęp)]
    POW[Powiadomienia]
    END([KONIEC])

    START --> LOGIN
    LOGIN --> EDIT
    EDIT --> LISTA
    LISTA --> KALENDARZ
    KALENDARZ --> STATY
    STATY --> POW
    POW --> END

    LISTA <---> SYNC
