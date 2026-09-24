# BaseHider 1.3.0

Paper plugin für quadratische, persönliche Base-Zonen.

## Zonen der eigenen Base

- 0–20 Blöcke: unsichtbar
- mehr als 20 bis unter 25 Blöcke: blau, noch unsichtbar
- 25–30 Blöcke: gelb, sichtbar
- mehr als 30 Blöcke: sichtbar

Die Distanz wird quadratisch über X/Z berechnet. Jede Zone wird ausschließlich anhand der eigenen Base des Spielers geprüft. Die Base eines anderen Spielers löst keine Nachrichten bei dir aus.

## Nachrichten

- Außen → Gelb: `Du bist gleich unsichtbar.`
- Gelb → Blau: `Du bist gleich sichtbar.`
- Blau → Gelb/Außen: `Du bist jetzt sichtbar.`
- Beim Betreten des inneren Bereichs: `Du bist jetzt unsichtbar.`

## Befehle

- `/setbase` setzt die eigene Base auf den aktuellen Block.
- `/removebase` entfernt die eigene Base.

## Bauen

Voraussetzungen: Java 21 und Maven.

```bash
mvn clean package
```

Die fertige JAR liegt danach unter:

```text
target/BaseHider-1.3.0.jar
```
