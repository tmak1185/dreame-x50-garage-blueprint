My DIY Dreame X50 Ultra Garage

Smart automatic garage door with Home Assistant

A custom-built garage for the Dreame X50 Ultra Complete, featuring an automatically controlled roller door integrated into Home Assistant.

The garage door opens and closes automatically depending on the robot’s operating status and distance from its docking station.

This project combines a custom-built cabinet, a motorized roller blind and a Home Assistant automation blueprint.

Features

* Automatic opening when the robot starts and raises its LDS sensor
* Automatic closing after the robot leaves the garage
* Automatic opening when the robot returns to its docking station
* Supports intermediate mop-washing trips
* Automatic closing once the robot is docked
* Adjustable distance thresholds
* Home Assistant blueprint for easy configuration

Hardware

* Dreame X50 Ultra Complete
* Home Assistant Green
* HACS Dreame Vacuum integration
* Motion Blinds motor
* Motion Blinds CMD-01 Bridge
* Roller blind from Bauhaus (approx. 50 cm wide, 25 mm tube)
* Custom-built black cabinet
* Two drawer slides used as vertical guides for the garage door

Home Assistant requirements

* Home Assistant
* HACS
* Dreame Vacuum integration
* A compatible cover entity controlling the garage door
* A distance sensor measuring the robot’s distance from its docking station

The blueprint uses the robot’s status information to control the garage door.

Installation

1. Open Home Assistant.
2. Navigate to Settings → Automations & Scenes → Blueprints.
3. Import the blueprint using this URL:
    https://github.com/tmak1185/dreame-x50-garage-blueprint/blob/main/dreame_x50_garage.yaml
4. Create a new automation using the imported blueprint.
5. Select your vacuum, garage cover and distance sensor.

Adjustable settings

Default distance thresholds:

* Close garage after departure: 0.5 m
* Open garage when returning: 3.0 m

These values can be adjusted in the blueprint.

Important

This project has been tested with the Dreame X50 Ultra Complete.

Other Dreame models may work if the required status attributes are available through the Dreame Vacuum integration. Compatibility with other models has not been tested.

Please supervise the first test runs and make sure the garage door cannot obstruct the robot.

⸻

Deutsche Version

Meine selbstgebaute Dreame-X50-Garage

Automatisches Garagentor mit Home Assistant

Eine selbstgebaute Garage für den Dreame X50 Ultra Complete mit motorisiertem Garagentor und vollständiger Home-Assistant-Integration.

Das Garagentor wird abhängig vom Betriebszustand und der Entfernung des Saugroboters zur Ladestation automatisch geöffnet und geschlossen.

Das Projekt kombiniert einen selbstgebauten Schrankkorpus, einen elektrischen Rollmechanismus und eine Home-Assistant-Blueprint-Automation.

Funktionen

* Automatisches Öffnen beim Start und Hochfahren des LDS-Turms
* Automatisches Schließen nach dem Verlassen der Garage
* Automatisches Öffnen bei der Rückkehr zur Ladestation
* Berücksichtigung von Zwischenfahrten zur Moppreinigung
* Automatisches Schließen nach dem Andocken
* Einstellbare Entfernungswerte
* Einfache Einrichtung über einen Home-Assistant-Blueprint

Verwendete Komponenten

* Dreame X50 Ultra Complete
* Home Assistant Green
* HACS Dreame Vacuum Integration
* Motion Blinds Motor
* Motion Blinds CMD-01 Bridge
* Bauhaus-Rollo (ca. 50 cm breit, 25-mm-Rollrohr)
* Selbstgebauter schwarzer Schrankkorpus
* Zwei Schubladenauszüge als seitliche Führung des Garagentors

Einrichtung

1. Home Assistant öffnen.
2. Zu Einstellungen → Automatisierungen und Szenen → Blueprints wechseln.
3. Blueprint über folgende URL importieren:
    https://github.com/tmak1185/dreame-x50-garage-blueprint/blob/main/dreame_x50_garage.yaml
4. Neue Automation mit dem importierten Blueprint erstellen.
5. Saugroboter, Garagentor und Entfernungssensor auswählen.

Standardwerte

* Garagentor schließen nach Abfahrt: 0,5 m
* Garagentor öffnen bei Rückkehr: 3,0 m

Die Werte können im Blueprint angepasst werden.

Hinweise

Das Projekt wurde mit dem Dreame X50 Ultra Complete getestet.

Andere Dreame-Modelle können möglicherweise ebenfalls funktionieren, sofern die benötigten Statusinformationen über die Dreame-Vacuum-Integration verfügbar sind. Eine Kompatibilität mit anderen Modellen wurde bisher nicht getestet.

Die ersten Testfahrten sollten beaufsichtigt werden. Das Garagentor darf den Roboter nicht behindern.
