# Dreame X50 – Automatic Garage Door Control

Home Assistant Blueprint zur Steuerung eines Garagentors für einen Dreame-Saugroboter.

## Funktionen

- Öffnet bei der ersten Abfahrt, sobald der LDS-Turm hochfährt und der Roboter noch angedockt ist.
- Öffnet nach einer Zwischenwäsche, sobald `washing` von `true` auf `false` wechselt und der Roboter noch an der Station steht.
- Schließt nach der Abfahrt, sobald der Entfernungssensor den eingestellten Abstand überschreitet.
- Öffnet bei der Rückkehr, sobald der Entfernungssensor den eingestellten Abstand unterschreitet.
- Schließt nach dem Andocken.
- Verhindert das Schließen durch den Abfahrt-Entfernungstrigger, solange der Roboter als rückkehrend gemeldet wird.

## Voraussetzungen

- Home Assistant mit Blueprint-Unterstützung
- Dreame-Integration, die die verwendeten Attribute bereitstellt:
  - `lds_state`
  - `docked`
  - `washing`
  - `started`
  - `returning`
- Ein numerischer Entfernungssensor zur Ladestation, dessen Einheit Meter ist
- Ein Garagentor als `cover`-Entität

## Installation

1. In Home Assistant **Einstellungen → Automationen & Szenen → Blueprints** öffnen.
2. Den Blueprint importieren oder die YAML-Datei in den Blueprint-Ordner kopieren.
3. Eine neue Automation aus diesem Blueprint erstellen.
4. Roboter, Garagentor und Entfernungssensor auswählen.
5. Die gewünschten Abstände einstellen.

## Standardwerte

- Schließen nach Abfahrt: 0,5 m
- Öffnen bei Rückkehr: 3,0 m

## Hinweise

Die verwendeten Attributnamen und Zustandswerte können je nach Dreame-Integration und Modell abweichen.
Vor dem unbeaufsichtigten Betrieb muss die Automation mit dem jeweiligen Roboter und Garagentor geprüft werden.
Insbesondere bei sehr geringem Abstand zwischen Roboter und Tor muss sichergestellt sein, dass das Tor vor der Roboterbewegung vollständig geöffnet ist.

Dieses Projekt basiert auf einer individuellen Dreame-X50-Garageninstallation. Es wird ohne Gewähr bereitgestellt.
