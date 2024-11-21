<p align="left">
<a href="https://github.com/ndeadly/MissionControl/blob/master/LICENSE"><img alt="GitHub" src="https://img.shields.io/github/license/ndeadly/MissionControl"></a>
<a href="https://github.com/ndeadly/MissionControl/releases/latest"><img alt="GitHub release (latest by date)" src="https://img.shields.io/github/v/release/ndeadly/MissionControl"></a>
<a href="https://github.com/ndeadly/MissionControl/releases"><img alt="GitHub All Releases" src="https://img.shields.io/github/downloads/ndeadly/MissionControl/total"></a>
<a href="https://github.com/ndeadly/MissionControl/releases/latest"><img alt="GitHub Releases" src="https://img.shields.io/github/downloads/ndeadly/MissionControl/latest/total"></a>
<a href="https://discord.gg/gegfNZ5Ucz"><img alt="Discord Server" src="https://discordapp.com/api/guilds/905069757361971303/widget.png?style=shield"/></a>
<br>
<a href="https://www.bitcoinqrcodemaker.com/api/?style=bitcoin&prefix=on&address=bc1q4rh4vmqaujmewrswes303nms5mj3p80j7lqat0"><img alt="Donate Bitcoin" src="https://img.shields.io/static/v1?label=donate&message=bc1q4rh4vmqaujmewrswes303nms5mj3p80j7lqat0&color=yellow&style=flat&logo=bitcoin"></a>
<a href="https://www.bitcoinqrcodemaker.com/api/?style=ethereum&prefix=on&address=0xFD28C8680416D5c706Ad8E404955e0a3A2aA7124"><img alt="Donate Ethereum" src="https://img.shields.io/static/v1?label=donate&message=0xFD28C8680416D5c706Ad8E404955e0a3A2aA7124&color=yellow&style=flat&logo=ethereum"></a>
</p>


# MissionControl

Verwenden Sie Controller von anderen Konsolen nativ auf Ihrer Nintendo Switch über Bluetooth. Keine Dongles oder andere externe Hardware erforderlich.

### Funktionen

* Unterstützt alle Switch-Firmware-Versionen.
* Verbinden Sie bis zu 8 Nicht-Switch-Bluetooth-Controller gleichzeitig ohne zusätzliche Hardware.
* Nutzen Sie native HOS-Menüs für Controller-Pairing, Tastenumzuordnung (ab Firmware 10.0.0) usw.
* Unterstützung für Rumble und Bewegungssteuerungen (nur kompatible Controller)
* Geringe Eingangsverzögerung.
* Dateibasiertes virtuelles Controller-Speichermodul, das die Speicherung und Wiederherstellung von Daten wie Kalibrierung des Analogsticks ermöglicht.
* Spoofing des Namens und der Adresse des Host-Bluetooth-Adapters.
* Das `mc.mitm`-Modul fügt Erweiterungs-IPC-Befehle hinzu, die verwendet werden können, um mit dem `bluetooth`-Prozess zu interagieren, ohne den Zustand des Systems zu beeinträchtigen.

### Unterstützte Controller

Aktuell werden die folgenden Controller unterstützt. Wenn Sie eine Controllervariante eines der unten aufgeführten Controller von Drittanbietern haben oder einen Bluetooth-Controller, der nicht aufgeführt ist, können Sie einen Controller-Anforderungs-[Issue](https://github.com/ndeadly/MissionControl/issues/new/choose) einreichen.

* __Nintendo Wii Remote + Erweiterungen (Nunchuck, Classic Controller, Classic Controller Pro, SNES Mini, TaTaCon (Taiko-Trommel), MotionPlus)__
* __Nintendo Wii Balance Board (experimentell)__
* __Nintendo WiiU Pro Controller__
* __Sony Dualshock3 (Playstation 3) Controller__
* __Sony DualShock4 (Playstation 4) Controller__
* __Sony Dualsense (Playstation 5) Controller__
* __Sony Dualsense Edge Controller__
* __Microsoft Xbox One S/X Controller (nicht zu verwechseln mit Series S/X Controllern - diese verwenden Bluetooth LE, das derzeit nicht unterstützt wird)__*
* __Microsoft Xbox Elite Wireless Controller Series 2__
* __NVidia Shield Controller (Modell 2017)__
* __Ouya Controller__
* __Gamestick Controller__
* __Gembox Controller__
* __iCade Controller__
* __Ipega-Controller (7197, 9017s, 9023, 9055, 9062S, 9076, 9078, 9087, 9096 funktionieren bestätigt. Andere können auch funktionieren)__
* __g910 Wireless Bluetooth Controller__
* __Xiaomi Mi Controller__
* __Steelseries Free__
* __Steelseries Nimbus__
* __Steelseries Stratus Duo__
* __Steelseries Stratus XL__
* __GameSir G3s__
* __GameSir G4s__
* __GameSir T1s__
* __GameSir T2a__
* __Hori Onyx__
* __8BitDo SN30 Pro Xbox Cloud Gaming Edition__
* __8BitDo Ultimate 2.4G Wireless Controller__
* __8BitDo ZERO (Die meisten anderen 8BitDo-Controller haben einen Switch-Modus verfügbar. Kann ein Firmware-Update erfordern)__
* __PowerA Moga Hero__
* __PowerA Moga Pro__
* __PowerA Moga Pro 2__
* __Mad-Catz C.T.R.L.R__
* __Mad-Catz L.Y.N.X 3__
* __Razer Raiju Tournament__
* __Razer Raiju Ultimate__
* __Razer Serval__
* __Mocute 050__
* __Mocute 053__
* __Gen Game S3__
* __AtGames Legends Pinball Controller + Arcade Control Panel__
* __Hyperkin Scout__
* __Betop 2585N2__
* __Atari Wireless Modern Controller__
* __SCUF Vantage 2__

**Nicht alle kabellosen Xbox One-Controller unterstützen Bluetooth. Ältere Varianten verwenden ein proprietäres 2,4-GHz-Protokoll und können nicht mit der Switch verwendet werden. Sehen Sie [hier](https://support.xbox.com/help/hardware-network/accessories/connect-and-troubleshoot-xbox-one-bluetooth-issues) für Informationen zur Identifizierung der Bluetooth-Variante.*

### Anforderungen

* Hackbare Nintendo Switch mit einer aktuellen Version der [Atmosphère](https://github.com/Atmosphere-NX/Atmosphere/releases) Custom Firmware. Andere benutzerdefinierte Firmware-Versionen werden ***nicht unterstützt***.
* Kompatibler Bluetooth-Controller

### Installation

Laden Sie das [neueste Release](https://github.com/ndeadly/MissionControl/releases) .zip herunter und entpacken Sie es im Stammverzeichnis Ihrer SD-Karte, wobei die Ordner fusionieren und vorhandene Dateien überschrieben werden. Starten Sie Ihre Konsole neu, um das Modul zu aktivieren, und Sie sind fertig!

***IMPORTANT: 
Atmosphère >= 1.8.0 is required to run the latest release of Mission Control on firmware 19.0.0. Using an older Atmosphère version will cause Mission Control to crash or freeze the system on boot.***

### Verwendung

Mission Control ist hauptsächlich ein Sysmodul (Hintergrundprozess), das von Atmosphère beim Booten geladen wird und dauerhaft neben dem Rest des Betriebssystems läuft. Es ermöglicht die Verwendung von nicht unterstützten Bluetooth-Controllern, als wären sie native Pro Controller. Das bedeutet, dass Sie neue Controller über die eigenen Systemmenüs von Nintendo pairen und konfigurieren können, ohne zusätzliche Homebrew-Anwendungen laden zu müssen. Es gibt (derzeit) keine Mission Control "App", die geöffnet werden muss.

Controller müssen zuerst mit der Konsole gepaart werden (siehe unten), bevor sie verwendet werden können. Einmal gepaart, suchen und verbinden sich die Controller automatisch mit der Konsole, wenn sie aufgeweckt werden. Es ist nicht erforderlich, sie jedes Mal erneut zu pairen. Beachten Sie, dass inoffizielle Controller nicht verwendet werden können, um die Konsole aufzuwecken.

Sobald verbunden, werden die Tasten Ihres Controllers so nah wie möglich an das physische Layout eines Switch Pro Controllers gemappt. Dies bedeutet, dass A/B- und X/Y-Tasten für Controller, die ein Xbox-ähnliches Tastenlayout verwenden, vertauscht werden, anstatt das zu verwenden, was auf der Taste gedruckt ist. Die Tastenkombinationen `MINUS + DPAD_UP` und `MINUS + DPAD_DOWN` werden für alle Controller bereitgestellt, um als Alternative für die `CAPTURE`- und `HOME`-Tasten zu fungieren, falls nicht genügend Face-Tasten vorhanden sind. Die Tastenzuordnungen können im offiziellen Systemmenü unter `Systemeinstellungen->Controller und Sensoren->Tastenzuordnung ändern` geändert werden.

Die meisten anderen nativen Funktionen *sollten* einfach funktionieren (mit Ausnahme von Dingen wie Firmware-Update). Wenn Sie etwas finden, das nicht funktioniert, öffnen Sie bitte ein Support-Problem auf dieser GitHub-Seite.

#### Controller-Pairing
Nintendo hat mit ihren Menüpunkten für Controller eine eher verwirrende Namenswahl getroffen. Controller werden im Systemmenü unter `Controller->Grip/Reihenfolge ändern` gepaart und ***nicht*** unter `Neue Controller pairen` oder `Controller suchen`, wie es der gesunde Menschenverstand erwarten lässt. Auf diesem Bildschirm setzen Sie Ihren Controller in den Pairing-Modus (siehe unten) und warten ein paar Sekunden. Wenn erfolgreich, sehen Sie eine `Gepaart`-Benachrichtigung oben links auf dem Bildschirm. Ihr Controller ist jetzt gepaart und kann jederzeit wieder verbunden werden, ohne diesen Bildschirm erneut aufrufen zu müssen. Eine erneute Paarung ist nur erforderlich, wenn der Controller mit einem anderen Gerät oder emummc verbunden wurde.

Die unterstützten Controller haben jeweils ihre eigenen Methoden, um in den Pairing-/Sync-Modus zu gelangen. Unten finden Sie Anweisungen zum Eintritt in diesen Modus für einige der gängigen Konsolencontroller.

***Nintendo Wii/WiiU Controller***
Drücken Sie die rote Sync-Taste auf der Rückseite des Controllers. Die Controller-LEDs blinken dann schnell.

Es wird empfohlen, für diese Controller-Typen, wo möglich, eine Analogstick-Kalibrierung durchzuführen, da jeder Controller einen unterschiedlichen Analogstick-Bereich und eine unterschiedliche Mittelposition hat, aber im Gegensatz zu Switch-Controllern gibt es keine gespeicherte Werkseinstellungskalibrierung.

***Sony Dualshock3 Controller***
Um diesen Controller zu paaren, müssen Sie ihn über ein USB-Kabel mit der Konsole verbinden. Sobald die Controller-LEDs zu blinken beginnen, trennen Sie das USB-Kabel und drücken Sie die `PS`-Taste.

*Hinweis: Um unerwünschtes Verhalten zu vermeiden, wenn der Controller im USB-Kabelmodus verwendet wird, funktioniert dies nur vom üblichen Bildschirm `Controller->Grip/Reihenfolge ändern` aus.*

***Sony Dualshock4/Dualsense Controller***
Drücken und halten Sie die `PS`- und `Share`-Tasten gleichzeitig, bis die Lichtleiste zu blinken beginnt. Wenn dies korrekt ausgeführt wird, ähnelt das Blinkmuster einem Herzschlag, andernfalls blinkt es gleichmäßig an und aus.

Wenn Sie Schwierigkeiten haben, den Controller mit der Konsole zu verbinden, drücken und halten Sie die Reset-Taste auf der Rückseite des Controllers einige Sekunden lang und versuchen Sie es erneut. Manchmal ist dies erforderlich, nachdem Sie sich mit einer Playstation-Konsole oder einem anderen Gerät verbunden haben.

***Microsoft Xbox One/Elite 2 Controller***
Drücken und halten Sie die `Guide`(`X`)-Taste, bis die LED zu blinken beginnt. Halten Sie dann die kleine Sync-Taste auf der Rückseite in der Nähe des Ladeanschlusses gedrückt, bis die LED schneller zu blinken beginnt.

*Hinweis: Controller-Firmware-Versionen 5.xx.xxxx.x und höher verwenden Bluetooth Low Energy und werden derzeit nicht unterstützt. Bitte lesen Sie die [FAQ](#häufig-gestellte-fragen), um Anweisungen zum Downgrade auf eine kompatible Firmware zu erhalten.*

***Andere Controller***
Bitte konsultieren Sie die Bedienungsanleitung Ihres Controllers, um Informationen darüber zu erhalten, wie Sie ihn in den Synchronisierungsmodus versetzen können. Beachten Sie, dass viele generische Bluetooth-Controller in einem von mehreren Modi gestartet werden können. Normalerweise möchten Sie einen Modus wie HID, PC oder Android auswählen, damit er korrekt funktioniert.

Controller, die erfolgreich gepaart wurden, aber noch nicht offiziell unterstützt werden, werden im `Controller`-Menü mit roten Tasten angezeigt, um anzuzeigen, dass ihre Steuerungen nicht gemappt werden. Bitte öffnen Sie ein Problem, um Unterstützung für solche Controller anzufordern.

### Modulkonfiguration

Eine Vorlage für die Konfigurationsdatei .ini wird unter `/config/MissionControl/missioncontrol.ini.template` installiert. Um die Standardmodul-Einstellungen zu ändern, kopieren Sie die Vorlage nach `/config/MissionControl/missioncontrol.ini` und kommentieren Sie (entfernen Sie das führende `;`) und ändern Sie alle Einstellungen, die Sie ändern möchten. Die Datei wird nur beim Start analysiert, daher erfordern alle von Ihnen vorgenommenen Änderungen einen Neustart, um wirksam zu werden. Einstellungen, die nicht korrekt analysiert/validiert werden können, werden ignoriert. Derzeit gibt es nur eine kleine Anzahl von Konfigurationseinstellungen, aber dies wird in zukünftigen Versionen erweitert.

- `[general]`
Dies sind allgemeine Einstellungen für Mission Control-Funktionen.
    - `enable_rumble` Aktivieren/Deaktivieren der Rumble-Unterstützung für inoffizielle Controller.
    - `enable_motion` Aktivieren/Deaktivieren der Bewegungssteuerungsunterstützung.

- `[bluetooth]`
Diese Einstellungen können verwendet werden, um Ihr Switch-Bluetooth so zu fälschen, dass es als ein anderes Gerät erscheint. Dies kann nützlich sein (in Verbindung mit einem Link-Schlüssel), wenn Sie Ihren Controller über mehrere Geräte hinweg verwenden möchten, ohne ihn jedes Mal neu pairen zu müssen. Beachten Sie, dass das Ändern dieser Einstellungen die auf früher gepaarten Controllern gespeicherten Informationen zu Ihrer Konsole ungültig macht und eine erneute Paarung erfordert.
    - `host_name` Überschreiben Sie den Bluetooth-Hostadapternamen.
    - `host_address` Überschreiben Sie die Bluetooth-Hostadapteradresse.

- `[misc]`
Dies sind verschiedene controller-spezifische Einstellungen usw.
    - `analog_trigger_activation_threshold` Legen Sie die Schwelle fest, ab der ZL/ZR für Controller mit analogen Triggern als gedrückt betrachtet werden. Gültiger Bereich [0-100] Prozent.
    - `dualshock3_led_mode` Legen Sie das Verhalten der Dualshock 3-Player-LEDs fest. Gültige Modi [0-1], wobei 0=Switch-Muster, 1=PS3-Muster, 2=Hybrid (Switch-Muster umgekehrt, um mit den numerischen Etiketten auf dem Controller übereinzustimmen)
    - `dualshock4_polling_rate` Legen Sie die Abfragefrequenz für Sony Dualshock 4-Controller fest. Gültiger Bereich [0-16], wobei 0=Max, 16=Min. Siehe [hier](https://github.com/ndeadly/MissionControl/blob/4a0326308d1ff39353b045f5efb1a99c4a504c28/mc_mitm/source/controllers/dualshock4_controller.hpp#L21) für entsprechende Frequenzwerte.
    - `dualshock4_lightbar_brightness` Legen Sie die LED-Lichtbalkenhelligkeit für Sony Dualshock 4-Controller fest. Gültiger Bereich [0-9], wobei 0=Aus, 1=Min, 2-9=12,5-100% in 12,5% Schritten.
    - `dualsense_lightbar_brightness` Legen Sie die LED-Lichtbalkenhelligkeit für Sony Dualsense-Controller fest. Gültiger Bereich [0-9], wobei 0=Aus, 1=Min, 2-9=12,5-100% in 12,5% Schritten.
    - `dualsense_enable_player_leds` Aktivieren/Deaktivieren der weißen Spielerindikator-LEDs unter dem Dualsense-Touchpad.
    - `dualsense_vibration_intensity` Legen Sie die Vibrationstärke des Dualsense fest, 12,5% pro Schritt. Gültiger Bereich [1-8], wobei 1=12,5%, 8=100%.

### Deinstallation

Um Mission Control und seine Komponenten funktional zu deinstallieren, müssen lediglich die folgenden Verzeichnisse von Ihrer SD-Karte gelöscht und Ihre Konsole neu gestartet werden.

* `/atmosphere/contents/010000000000bd00`
* `/atmosphere/exefs_patches/bluetooth_patches`
* `/atmosphere/exefs_patches/btm_patches`

Wenn Sie alle Spuren der Software vollständig entfernen möchten (Telemetrie ausgenommen), sollten Sie auch die folgenden zusätzlichen Schritte ausführen:

* Entfernen Sie das folgende Verzeichnis von Ihrer SD-Karte
    * `/config/MissionControl`

* Löschen Sie die Bluetooth-Paarungsdatenbank über `Systemeinstellungen->Controller und Sensoren->Controller trennen`

### Geplante/Laufende Funktionen
Im Folgenden finden Sie eine Liste von Funktionen, an denen ich derzeit arbeite oder die ich in Zukunft untersuchen möchte, grob in absteigender Reihenfolge der Priorität. Anfragen sind willkommen, wenn Sie eine Idee haben, von der Sie glauben, dass sie eine nützliche Funktion darstellen würde.

* ~~Rumble-Unterstützung~~
* ~~Bewegungssteuerungsunterstützung~~
* Bluetooth LE-Unterstützung
* USB-Kabelcontroller
* UART MITM, um Tastenkombinationen und andere zukünftige Funktionen auf Joy-Cons im Handheld-Modus anzuwenden
* Konfigurationen pro Controller
    * Rumble ein/aus
    * Bewegungssteuerung ein/aus
    * Identifizieren als Pro Controller oder Joy-Con
    * Controller-Gehäuse/Tastenfarben festlegen
    * Achsen der Analogsticks invertieren
    * Toleranzen der Analogsticks
* Begleitanwendung
    * Verwaltung der Paarungsdatenbank
        * Anzeigen von Informationen zu gepaarten Controllern
        * Datenbank löschen
        * Datenbank in Datei exportieren
        * Bestehende Datenbank aus Datei importieren
    * Controller-Management/Diagnose
        * Controllerkonfigurationen verwalten
        * Rohdatenberichte anzeigen
        * Tasten/Analogsticks testen
        * SPI-Flash speichern (nur offizielle Controller)
    * Controllerentdeckung/Neupaarung neu implementieren
* Tesla-Overlay
* Unterstützung für Tastatur und Maus
* Gamecube-Modus (Unterstützung für analoge Trigger)
* Titelspezifische Tastenzuordnungen

### Bekannte Probleme und Einschränkungen

* Nicht-Switch-Controller können das System nicht aus dem Schlafmodus wecken.
* Controller, die den Bluetooth-LE-Standard (BLE) verwenden, werden derzeit nicht unterstützt und können keine Verbindung zum System herstellen.
* Einige Controller können einige Zeit benötigen, um erkannt und anschließend mit der Konsole gekoppelt zu werden. Haben Sie Geduld und geben Sie den Synchronisierungsmodus des Controllers mehrmals ein, falls erforderlich. Sobald sie synchronisiert sind, sollten die Controller wie gewohnt funktionieren.
* Xbox One-Controller können nicht über die Software ausgeschaltet werden und versuchen, sich nach dem Trennen erneut mit der Konsole zu verbinden. Dies ist eine Einschränkung der Bluetooth-Firmware des Controllers. Um den Controller auszuschalten, muss die Führungstaste mehrere Sekunden lang gedrückt gehalten werden.
* Die gemeldeten Controller-Batteriestände sind möglicherweise nicht korrekt. Ich verlasse mich ausschließlich auf im Internet gefundene Reverse Engineering-Notizen. In vielen Fällen besitze ich den Controller nicht und es gibt einfach keine Informationen, sodass diese Controller immer volle Batterie anzeigen. Jede Hilfe zur Verbesserung ist sehr willkommen.
* Mehrere Benutzer haben über Nachahmer-WiiU- und Dualshock4-Controller berichtet, die während der Bluetooth-Erkennung nicht von der Konsole erkannt werden können. Leider glaube ich, dass sie einen inkompatiblen Bluetooth-Chipsatz verwenden.
* Mission Control speichert Konfigurationsdaten für jeden gekoppelten Controller im Verzeichnis `/config/MissionControl/controllers`. Wenn ein Teil dieses Verzeichnisbaums beschädigt wird, können Controller beim Versuch, Konfigurationsdaten zu lesen, getrennt werden.
* Bei Verwendung von Wii-Controllern mit MotionPlus muss der Controller eingeschaltet werden, während er mit der Knopfseite nach unten auf einer flachen Oberfläche liegt, um ordnungsgemäß kalibriert zu werden. Die Bewegungsachsen werden sonst durcheinandergebracht.
* Wii-Erweiterungscontroller werden manchmal falsch erkannt, wenn MotionPlus vorhanden ist. Dieses Problem scheint zeitabhängig zu sein und kann durch erneutes Anschließen der Erweiterung bei Bedarf behoben werden.

### Häufig gestellte Fragen

***Läuft das auf \<hier CFW einfügen\>?***
Nein. Mission Control läuft nur unter Atmosphère. Das ist kein Versuch, Nutzer anderer CFWs auszusperren, Atmosphere ist einfach die einzige, die die nötigen Erweiterungen bereitstellt, um die Bluetooth-Kommunikation zu überwachen, die dieses Sysmodul ermöglicht.

***Werde ich gebannt, wenn ich das online nutze?***
Aktuell gibt es keine bestätigten Fälle von Bans durch die Nutzung von Mission Control. Dennoch birgt die Nutzung inoffizieller Software unter CFW immer ein gewisses Risiko und Nintendo könnte die Bankriterien jederzeit ändern. Auch wenn Mission Control relativ sicher sein sollte, da es einfach einen angeschlossenen Pro Controller emuliert, wäre es sicher möglich zu erkennen, dass du inoffizielle Controller an die Konsole angeschlossen hast, wenn Nintendo daran interessiert wäre. Nutzung auf eigene Gefahr.

***Unterstützt das USB-Controller?***
Nein, Mission Control unterstützt aktuell nur Bluetooth. Vorerst kannst du catherys [sys-con](https://github.com/cathery/sys-con) für USB-Controller nutzen.

***Funktioniert das mit installiertem sys-con?***
Ja, die beiden können problemlos gleichzeitig laufen.

***Meine Konsole stürzt beim Booten wegen diesem Sysmodul ab. Was kann ich tun?***
Wenn du Abstürze beim Booten mit der Titel-ID von Mission Control (`010000000000bd00`) siehst, liegt es wahrscheinlich daran, dass du kürzlich auf eine neue Atmosphère-Version aktualisiert hast und ein Update für Mission Control nötig ist, oder dass du eine alte Version von Atmosphère nutzt, die nicht mit der neuesten Version von Mission Control kompatibel ist.
Abstürze in `sm` (Titel-ID `0100000000000004`) können auf Versionsinkompatibilitäten zwischen deiner aktuellen Atmosphère und einem oder mehreren deiner Homebrew-Sysmodule hinweisen. Das kann durch Mission Control verursacht werden, oder es könnte ein anderes benutzerdefiniertes Sysmodul sein, das libstratosphere nutzt, selbst wenn es so aussieht als wäre Mission Control schuld (`ldn_mitm` und `emuiibo` sind häufige Übeltäter). Wenn du gerade Atmosphère aktualisiert hast, solltest du immer prüfen ob es auch Updates für die von dir genutzten Sysmodule gab.
qlaunch-Fehler (Titel-ID `0100000000001000`) können ein Zeichen dafür sein, dass du zu viele benutzerdefinierte Sysmodule laufen hast und die begrenzten Systemressourcen aufbrauchst. Prüfe deinen `/atmosphere/contents` Ordner und stelle sicher, dass du wirklich alles darin brauchst. Wenn du nicht weißt was du tust, ist es vielleicht einfacher den Ordner komplett zu löschen, Atmosphère neu zu installieren und dann nur die Sysmodule explizit neu zu installieren, die du brauchst.

***Ich habe Mission Control installiert, aber es passiert nichts. Hilfe!***
Mission Control ist primär ein Hintergrundprozess. Es gibt keine sichtbaren Änderungen am System, die anzeigen, dass es installiert ist, außer dass dein Controller erfolgreich über Nintendos offizielle Menüs verbunden wird. Wenn du den Anweisungen zur Nutzung und Kopplung oben gefolgt bist und es nicht funktioniert, hier eine grundlegende Checkliste zur Fehlerbehebung.
- Stelle zunächst sicher, dass du die Konsole nach der Installation neu gestartet hast. Sonst wird das Modul nicht geladen.
- Stelle sicher, dass deine Konsole nicht im Flugmodus ist. Wenn doch, musst du ihn entweder deaktivieren oder Bluetooth explizit in den Flugmodus-Einstellungen aktivieren.
- Bestätige, dass Mission Control läuft. Dazu kannst du einen linken Joy-Con oder Pro Controller kabellos verbinden und die Tasten `DPAD_UP` + `MINUS` zusammen drücken. Das fungiert als Capture-Taste und macht einen Screenshot, wenn das Modul läuft. Wenn du keine Screenshot-Benachrichtigung siehst, wird Mission Control wahrscheinlich nicht geladen. Das liegt meist an einer fehlerhaften Installation und kann mehrere Gründe haben:
    - Archivbits wurden für eine oder mehrere Komponenten im Mission Control-Verzeichnisbaum gesetzt. Das kann passieren, wenn du einen Mac zum Übertragen der Dateien nutzt oder Mission Control aus inoffiziellen Quellen beziehst. Versuche, Hekates Tool zum Beheben von Archiv-Bits auszuführen.
    - Die von dir genutzte Software hat die Dateien nicht korrekt kopiert. Ich habe FTP-Clients gesehen, die leere Dateien gar nicht kopieren und Archivsoftware, die nicht direkt korrekt auf die SD entpackt. Versuche, das .zip-Archiv erst auf deinem PC zu entpacken, bevor du es überträgst und nutze eine seriöse Übertragungsmethode wie Hekate UMS/Haze (Atmosphères integriertes USB-Übertragungstool) oder einen vernünftigen FTP-Client (ich nutze WinSCP unter Windows).
    - Du bist den Installationsanweisungen nicht korrekt gefolgt und hast entweder Dateien ausgelassen oder am falschen Ort platziert.
    - SD-Karten-Korruption. Eventuell musst du deine SD-Karte formatieren oder ersetzen.
- Prüfe, ob der Controller, den du nutzen willst, in der Liste der unterstützten Controller ist. Insbesondere wenn du einen Xbox-Controller hast, stelle sicher, dass du ein kompatibles Modell nutzt und nicht auf die neuere Bluetooth-LE-Firmware aktualisiert hast. Controller, die Bluetooth LE nutzen, werden aktuell nicht unterstützt.
- Stelle sicher, dass dein Controller kein inoffizieller Klon ist. Das ist besonders häufig bei Dualshock 3 und 4 Controllern. Viele Klone funktionieren, aber es gibt welche, die sich einfach weigern.
- Stelle sicher, dass dein Controller-Akku ausreichend geladen ist. Manchmal haben Controller genug Ladung, um die Kopplung zu starten, schalten sich aber mittendrin immer wieder aus (bevor sie ihren Akkustand an die Konsole melden können).
- Wenn du alles oben Genannte versucht hast und nichts funktioniert, suche Hilfe auf meinem [Discord-Server](https://discord.gg/gegfNZ5Ucz).

***Wie kann ich dies mit mehreren sysNAND/emuMMC-Startkonfigurationen verwenden?***
Seit Version 1.5.1 enthält Atmosphäre nun Code, den ich beigetragen habe, um die Bluetooth-Kopplungsdatenbank zwischen sysNAND und emuMMC über eine Datei auf der SD-Karte zu synchronisieren. Dies kann aktiviert werden, indem `enable_external_bluetooth_db = u8!0x1` unter dem `[atmosphere]`-Abschnitt in `atmosphere/config/system_settings.ini` hinzugefügt wird. Hinweis: Diese Funktion erfordert, dass Atmosphäre ausgeführt wird, um zu funktionieren. Sie kann daher nicht verwendet werden, um sysCFW/emuMMC mit Stock/OFW zu synchronisieren.

***Kann ich Controller-Tasten mit Mission Control neu zuweisen?***
Ja. Da Mission Control offizielle Pro Controller emuliert, können Sie sie mit der offiziellen Methode von Nintendo in Firmware 10.0.0 neu zuweisen. Die Remapping-Optionen finden Sie im Systemmenü unter `Systemeinstellungen->Controller und Sensoren->Tastenbelegung ändern`.

***Meine Konsole zeigt eine "Gekoppelt"-Benachrichtigung an, aber mein Controller verbindet sich nicht. Was ist los?***
Ihr Controller hat sich erfolgreich mit der Konsole verbunden, wird aber kurz darauf getrennt, bevor er Eingaben senden kann. Dies kann aus verschiedenen Gründen geschehen, am häufigsten:
- Ihr Controller wird von Mission Control nicht offiziell unterstützt und ihm wurde kein Eingabehandler zugewiesen. Überprüfen Sie die Liste der [unterstützten Controller](#supported-controllers) für Ihren Controller. Bitte eröffnen Sie ein Controller-Anfrage [Problem](https://github.com/ndeadly/MissionControl/issues/new/choose), damit ich Unterstützung hinzufügen kann, wenn sie nicht vorhanden ist.
- Der Akku Ihres Controllers ist leer und muss ausgetauscht oder aufgeladen werden.
- Die virtuelle Speicherdatei Ihres Controllers oder der Verzeichnisbaum, der sie enthält, wurde beschädigt. Versuchen Sie, den Konfigurationseintrag des Controllers zu löschen (`/config/MissionControl/controllers/<xxxxxxxxxxxx>/`, wobei `<xxxxxxxxxxxx>` die 12-stellige hexadezimale Darstellung der Bluetooth-MAC-Adresse Ihres Controllers ist) und lassen Sie Mission Control eine neue erstellen. Es kann in einigen Fällen erforderlich sein, das gesamte Verzeichnis `controllers` zu löschen. Hinweis: Sie verlieren alle gespeicherten datenspezifischen Daten des Controllers, wie Benutzeranalogstick- oder Bewegungskalibrierungen, wenn Sie diese Dateien löschen. Da dies die zerstörerischste Maßnahme ist, sollten Sie sie zuletzt versuchen, nachdem Sie die oben genannten Vorschläge ausgeschöpft haben.

***Mein Xbox-Controller verbindet sich nicht, dabei sagtest du, sie seien unterstützt?***
Obwohl sie ähnlich aussehen mögen, sind nicht alle Xbox-Controller gleich. Tatsächlich gibt es mehrere Hardware-Revisionen/Modelle (7 zum Zeitpunkt der Abfassung) mit unterschiedlichen drahtlosen Fähigkeiten. Auf Xbox-Konsolen (oder PC mit dem drahtlosen USB-Adapter) verwenden alle Controller ein proprietäres drahtloses Microsoft-Protokoll namens GIP. Die Bluetooth-Konnektivität ist jedoch _nicht_ dasselbe und variiert je nach Controller-Modell. Einige unterstützen Bluetooth, andere nicht. Von denen, die es tun, verwenden einige den neueren (derzeit nicht unterstützten) Bluetooth Low Energy (LE) -Standard oder wechseln nach einem Firmware-Update dazu. **Die einzigen unterstützten Modelle sind die Revisionen 1708 (Xbox One S) und 1797 (Xbox Elite V2). Wenn diese auf eine Bluetooth LE-Firmware (5.xx.xxxx.x und höher) aktualisiert wurden, müssen Sie die Firmware auf die Legacy-Version downgraden (siehe unten)**. Controller-Modellnummern finden Sie im Inneren des Batteriefachs oder auf der Rückseite des Controllers bei Controllern mit internem Akku.

Weitere Details zu den verschiedenen Controller-Revisionen (mit Bildern) finden Sie [hier](https://en.wikipedia.org/wiki/Xbox_Wireless_Controller#Summary).

***Mein Xbox One/Elite V2-Controller hat früher verbunden und jetzt nicht mehr, woran liegt das?***
Seit Ende 2021 hat Microsoft eine neue Controller-Firmware eingeführt, die darauf abzielt, Xbox One/Elite 2-Controller mit den neueren Series X|S-Controllern in Einklang zu bringen. Durch das Update auf diese Firmware wird der Controller auf die Verwendung von Bluetooth Low Energy (LE) umgestellt, einem neueren Bluetooth-Standard, der auf geringen Stromverbrauch ausgelegt ist und derzeit nicht von Mission Control unterstützt wird. Wenn Ihre Controller-Firmware-Version 5.xx.xxxx.x oder höher ist, verfügen Sie über die neue LE-Firmware und müssen auf die Legacy-Version downgraden (siehe https://support.xbox.com/en-US/help/hardware-network/accessories/controller-firmware-reversion).

***Können Sie Unterstützung für Xbox 360-Controller hinzufügen?***
Nein, derzeit nicht. Diese verwenden kein Bluetooth. Probieren Sie sys-con mit einem drahtlosen USB-Adapter aus.

***Können Sie Unterstützung für das Aufwecken aus dem Schlafmodus hinzufügen?***
Wahrscheinlich nicht. Soweit ich weiß, beinhaltet das Aufwecken aus dem Schlafmodus das Senden eines speziellen Steuerbefehls an die Bluetooth-Hardware des Switch. Es gibt keine Möglichkeit, einen Nicht-Switch-Controller den vom Switch erkannten Befehl senden zu lassen, ohne die Hardware/Firmware zu modifizieren.

***Können Sie Bluetooth-Audio-Unterstützung hinzufügen?***
~~Nein. Das Bluetooth-Modul auf der Switch implementiert nur einen kleinen Satz von Diensten, die erforderlich sind, um HID-Controller funktionieren zu lassen. Von diesem kleinen Satz von Diensten sind nur eine Handvoll hochrangige Funktionen für den Rest des Systems verfügbar. Die Hinzufügung von Audio-Unterstützung würde erfordern, die Dienste zu implementieren, die für den Audio-Transport erforderlich sind, für die jede vernünftige Person eine Open-Source-Neuimplementierung des Bluetooth-Moduls benötigen würde, um Zugriff auf die erforderlichen Low-Level-Funktionen zu erhalten.~~ ~~Seit Firmware 12.0.0 unterstützt Nintendo nun offiziell Bluetooth-Audio. Während die Funktion in der offiziellen Software nicht aktiviert wurde, hat plutooo ein experimentelles Sysmodul namens [nx-btred](https://github.com/plutooo/nx-btred) erstellt, das Bluetooth-Audio in Spielen ermöglicht, die Aufnahmen unterstützen. Es gibt nicht viel Nutzen für mich, diese Funktionalität zu Mission Control hinzuzufügen.~~ Seit Firmware 13.0.0 unterstützt Nintendo nun offiziell Bluetooth-Audio.

***Mein Controller hat eine Audiobuchse, kannst du Headset-Unterstützung hinzufügen?***
Unwahrscheinlich. Soweit ich weiß, unterstützen Controller, die Audio-Headsets verwenden, dies über proprietäre oder nicht standardmäßige Mittel. Dies wäre viel Arbeit, nicht nur um zu verstehen, wie es für einen bestimmten Controller funktioniert, sondern auch um es irgendwie in HOS zu integrieren, wenn es kein Konzept eines Gamepads gibt, das Audio unterstützt. Im besten Fall verwendet ein Controller irgendeine Form von standardisiertem Bluetooth-Audio, Sie wären jedoch immer noch den üblichen Bandbreitenbeschränkungen der Konsole ausgesetzt (abgehacktes Audio, verzögerte Controller-Eingaben usw.). Verwenden Sie einfach normale Kopfhörer.

## Wie es funktioniert

Mission Control funktioniert, indem es sich als Man-In-The-Middle in das `bluetooth`-Systemmodul einklinkt und dessen Initialisierungs-IPC-Befehle und Systemereignisse abfängt. Dabei werden eingehende/ausgehende Daten übersetzt, um der Switch vorzugaukeln, dass sie mit einem offiziellen Pro Controller kommuniziert.

Um dies zu erreichen, erhält das `btdrv.mitm`-Modul die Handles für `bluetooth`-Systemereignisse und gemeinsamen Speicher, wenn das System versucht, diese über IPC mittels der `btm`- und `hid`-Module zu initialisieren. Es erstellt dann seine eigenen sekundären Versionen davon und übergibt deren Handles anstelle der Originale. Dies ermöglicht es, Änderungen an Datenpuffern vorzunehmen, bevor das System benachrichtigt wird (oder auch nicht). Zusätzlich wird der IPC-Befehl `WriteHidData` abgefangen, um ausgehende Anfragen an den Controller zu übersetzen oder zu verwerfen. Im letzteren Fall können gefälschte Antworten direkt in den Puffer im gemeinsamen Speicher geschrieben werden.

Das Abfangen von Initialisierungs-IPC-Befehlen ermöglicht es auch Homebrew, den `bluetooth`-Dienst korrekt zu nutzen. Normalerweise würde der Aufruf von IPC-Befehlen, die Systemereignisse initialisieren oder abschließen, entweder die Konsole zum Absturz bringen oder die von Systemprozessen gehaltenen Ereignis-Handles ungültig machen. Mit `btdrv.mitm` können wir alternative Ereignis-Handles bereitstellen, wenn Homebrew versucht, eine Schnittstelle zu initialisieren, und die echten Systemereignisse an diese umleiten, anstatt an die von Systemprozessen gehaltenen Ereignisse.

Exefs-Patches für das `bluetooth`-Modul werden bereitgestellt, um das Pairing von Wii/WiiU und anderen Controllern zu ermöglichen, die Legacy-Pincode-Pairing verwenden, sowie für Xbox Elite 2 Wireless Controller. Außerdem werden Geräteklassenüberprüfungen gelockert, die in neueren Firmwares hinzugefügt wurden, um auch Geräte zuzulassen, die sich als Tastatur oder Joystick identifizieren.

Exefs-Patches für das `btm`-Modul wurden hinzugefügt, um Aufrufe von `nn::bluetooth::hal::CloseHidConnection` zu überspringen, wenn ein Controller nicht korrekt auf den von `nn::bluetooth::hal::SetTsi` gesendeten Broadcom-Vendor-Befehl antwortet. Dies verhindert, dass alle betroffenen Controller sofort nach der Verbindung getrennt werden, und eliminiert die Notwendigkeit, bestimmte Controller manuell mit einer `settsi_disable.flag`-Datei zu kennzeichnen.

Der `btm`-Dienst wird jetzt ebenfalls als MITM verwendet, was es ermöglicht, Controller-Namen im laufenden Betrieb zu fälschen, während die Originalnamen in der Pairing-Datenbank beibehalten werden.

### Aus dem Quellcode bauen

Klone zuerst das Repository auf deinen lokalen Rechner und wechsle in das neu geklonte Verzeichnis
```
git clone --recurse-submodules https://github.com/ndeadly/MissionControl.git
cd MissionControl
```

~~Mission Control verwendet derzeit einen benutzerdefinierten Fork von `libnx`, der Bluetooth-Service-Wrapper und Typdefinitionen hinzufügt.~~ Offizielles libnx-Master wird jetzt verwendet, um Mission Control zu bauen. Zum Zeitpunkt des Schreibens kann das von devkitPro verteilte libnx verwendet werden, ohne dass du es selbst bauen musst. Dies kann sich ändern, wenn `Atmosphere-libs` aktualisiert wird, um bleeding-edge `libnx`-Commits zu verwenden, die im offiziellen Release nicht enthalten sind. In jedem Fall kannst du das enthaltene `libnx`-Submodul mit den folgenden Befehlen aus dem Quellcode bauen.

```
cd lib/libnx
make && make install
```

Baue als nächstes `libstratosphere`. Wenn du auf Buildfehler stößt, fehlen möglicherweise benötigte Abhängigkeiten (siehe https://github.com/Atmosphere-NX/Atmosphere/blob/master/docs/building.md)
```
cd ../Atmosphere-libs/libstratosphere
make
```

Baue und paketiere schließlich die Distributions-ZIP-Datei. Dabei wird das `mc.mitm`-Sysmodul gebaut und mit Bluetooth-Exefs-Patches verpackt.
```
cd ../..
make dist
```

Das resultierende Paket kann wie oben beschrieben installiert werden.


### Credits

* [__switchbrew__](https://switchbrew.org/wiki/Main_Page) für die umfangreiche Dokumentation des Switch-Betriebssystems.
* [__devkitPro__](https://devkitpro.org/) für die Homebrew-Compiler-Toolchain.
* __SciresM__ für seine engagierte Arbeit am [Atmosphère](https://github.com/Atmosphere-NX)-Projekt, libstratosphere und seine allgemeine Hilfsbereitschaft bei allen Themen rund um die Switch.
* __misson20000__ für seinen praktischen Debug-Monitor [Twili](https://github.com/misson20000/twili) und den IPC-Logger [Ilia](https://github.com/misson20000/ilia)
* __dekuNukem__, __CTCaer__, __shinyquagsire23__ und andere für ihre Arbeit beim Umkehren und Dokumentieren des Switch-Controller-Kommunikationsprotokolls.
* __Banz99__ für laufende Codebeiträge, Diskussion von Ideen, Tests und generelle Aufmerksamkeit.
* __friedkeenan__ für Hilfe beim Testen der Unterstützung für Wii-Erweiterungscontroller.
* __DatenThielt__ für die Hilfe beim Debuggen des Bluetooth-Dienstes remote mit seinem Xbox Elite Series 2-Controller, damit ich Patches entwickeln konnte, um ihn erfolgreich mit der Konsole zu koppeln.
* Alle anderen im __ReSwitched__ Discord-Server, die geholfen haben, technische Fragen zu beantworten.

### Unterstützung

Wenn dir dieses Projekt gefällt, dann unterstütze mich bitte, um die Entwicklung fortsetzen zu können :)

<a href="https://ko-fi.com/J3J01BZZ6"><img border="0" alt="ko-fi" src="https://www.ko-fi.com/img/githubbutton_sm.svg" align="left"></a>

</div>


---
---
---


<p align="left">
<a href="https://github.com/ndeadly/MissionControl/blob/master/LICENSE"><img alt="GitHub" src="https://img.shields.io/github/license/ndeadly/MissionControl"></a>
<a href="https://github.com/ndeadly/MissionControl/releases/latest"><img alt="GitHub release (latest by date)" src="https://img.shields.io/github/v/release/ndeadly/MissionControl"></a>
<a href="https://github.com/ndeadly/MissionControl/releases"><img alt="GitHub All Releases" src="https://img.shields.io/github/downloads/ndeadly/MissionControl/total"></a>
<a href="https://github.com/ndeadly/MissionControl/releases/latest"><img alt="GitHub Releases" src="https://img.shields.io/github/downloads/ndeadly/MissionControl/latest/total"></a>
<a href="https://discord.gg/gegfNZ5Ucz"><img alt="Discord Server" src="https://discordapp.com/api/guilds/905069757361971303/widget.png?style=shield"/></a>
<br>
<a href="https://www.bitcoinqrcodemaker.com/api/?style=bitcoin&prefix=on&address=bc1q4rh4vmqaujmewrswes303nms5mj3p80j7lqat0"><img alt="Donate Bitcoin" src="https://img.shields.io/static/v1?label=donate&message=bc1q4rh4vmqaujmewrswes303nms5mj3p80j7lqat0&color=yellow&style=flat&logo=bitcoin"></a>
<a href="https://www.bitcoinqrcodemaker.com/api/?style=ethereum&prefix=on&address=0xFD28C8680416D5c706Ad8E404955e0a3A2aA7124"><img alt="Donate Ethereum" src="https://img.shields.io/static/v1?label=donate&message=0xFD28C8680416D5c706Ad8E404955e0a3A2aA7124&color=yellow&style=flat&logo=ethereum"></a>
</p>

# Mission Control

Use controllers from other consoles natively on your Nintendo Switch via Bluetooth. No dongles or other external hardware neccessary.

### Features

* Supports all Switch firmware versions.
* Connect up to 8 non-switch Bluetooth controllers simultaneously without any additional hardware.
* Make use of native HOS menus for controller pairing, button remapping (firmware 10.0.0+) etc.
* Support for rumble and motion controls (compatible controllers only)
* Low input lag.
* File-based virtual controller memory allowing for data such as analog stick calibration to be stored and retrieved.
* Spoofing of host Bluetooth adapter name and address.
* `mc.mitm` module adds extension IPC commands that can be used to interact with the `bluetooth` process without interfering with the state of the system.

### Supported Controllers

 Currently, the following controllers are supported. If you have a third-party variant of one of the below, or a Bluetooth controller that isn't listed, consider submitting a controller request [issue](https://github.com/ndeadly/MissionControl/issues/new/choose).

* __Nintendo Wii Remote + extensions (Nunchuck, Classic Controller, Classic Controller Pro, SNES Mini, TaTaCon (Taiko drum), MotionPlus)__
* __Nintendo Wii Balance Board (experimental)__
* __Nintendo WiiU Pro Controller__
* __Sony Dualshock3 (Playstation 3) Controller__
* __Sony DualShock4 (Playstation 4) Controller__
* __Sony Dualsense (Playstation 5) Controller__
* __Sony Dualsense Edge Controller__
* __Microsoft Xbox One S/X Controller (not to be confused with Series S/X controllers - these use Bluetooth LE, which isn't currently supported)__*
* __Microsoft Xbox Elite Wireless Controller Series 2__
* __NVidia Shield Controller (2017 Model)__
* __Ouya Controller__
* __Gamestick Controller__
* __Gembox Controller__
* __iCade Controller__
* __Ipega Controllers (7197, 9017s, 9023, 9055, 9062S, 9076, 9078, 9087, 9096 confirmed working. Others may also work)__
* __g910 Wireless Bluetooth Controller__
* __Xiaomi Mi Controller__
* __Steelseries Free__
* __Steelseries Nimbus__
* __Steelseries Stratus Duo__
* __Steelseries Stratus XL__
* __GameSir G3s__
* __GameSir G4s__
* __GameSir T1s__
* __GameSir T2a__
* __Hori Onyx__
* __8BitDo SN30 Pro Xbox Cloud Gaming Edition__
* __8BitDo Ultimate 2.4G Wireless Controller__
* __8BitDo ZERO (Most other 8BitDo controllers have a Switch mode available. May require firmware update)__
* __PowerA Moga Hero__
* __PowerA Moga Pro__
* __PowerA Moga Pro 2__
* __Mad-Catz C.T.R.L.R__
* __Mad-Catz L.Y.N.X 3__
* __Razer Raiju Tournament__
* __Razer Raiju Ultimate__
* __Razer Serval__
* __Mocute 050__
* __Mocute 053__
* __Gen Game S3__
* __AtGames Legends Pinball Controller + Arcade Control Panel__
* __Hyperkin Scout__
* __Betop 2585N2__
* __Atari Wireless Modern Controller__
* __SCUF Vantage 2__

**Not all Xbox One wireless controllers support Bluetooth. Older variants use a proprietary 2.4Ghz protocol and cannot be used with the Switch. See [here](https://support.xbox.com/help/hardware-network/accessories/connect-and-troubleshoot-xbox-one-bluetooth-issues) for information on identifying the Bluetooth variant.*

### Requirements

* Hackable Nintendo Switch running an up-to-date version of [Atmosphère](https://github.com/Atmosphere-NX/Atmosphere/releases) custom firmware. Other custom firmwares are ***not supported***.
* Compatible Bluetooth controller

### Installation

Download the [latest release](https://github.com/ndeadly/MissionControl/releases) .zip and extract to the root of your SD card, allowing the folders to merge and overwriting any existing files. Reboot your console to activate the module and you're done!

***IMPORTANT: 
Atmosphère >= 1.8.0 is required to run the latest release of Mission Control on firmware 19.0.0. Using an older Atmosphère version will cause Mission Control to crash or freeze the system on boot.***

### Usage

Mission Control is primarily a sysmodule (background process) that gets loaded by Atmosphère at boot time and runs indefinitely alongside the rest of the operating system. It enables the use of unsupported Bluetooth controllers as if they were native Pro Controllers. This means that you can pair and configure new controllers via Nintendo's own system menus, without the need to load additional homebrew applications. There is (currently) no Mission Control "app" to be opened.

Controllers must first be paired with the console (see below) before they can be used. Once paired, controllers will seek out and reconnect to the console automatically when woken up. There is no need to re-pair them every time. Note that unofficial controllers cannot be used to wake the console.

Once connected, your controller's buttons are mapped as closely as possible to the physical layout of a Switch Pro Controller. This means that A/B and X/Y buttons will be swapped for controllers that use an Xbox style button layout rather than using what is printed on the button. The button combos `MINUS + DPAD_UP` and `MINUS + DPAD_DOWN` are provided for all controllers to function as an alternative for `CAPTURE` and `HOME` buttons in cases where there are not enough face buttons available. Button mappings can be changed from the official system menu at `System Settings->Controllers and Sensors->Change Button Mapping`.

Most other native features *should* just work (with the exception of things like firmware update). If you find something that's broken please open a support issue on this github page.

#### Pairing Controllers
Nintendo made some rather confusing naming choices with their controller menu items. Controllers are paired from the system menu under `Controllers->Change Grip/Order`, and ***not*** `Pairing New Controllers` or `Search for Controllers` as common sense may lead you to expect. On this screen, place your controller into pairing mode (see below) and wait a few seconds. If successful, you should see a `Paired` notification show in the top left of the screen. Your controller is now paired and can be reconnected at any time without having to re-enter this screen. Re-pairing is only required if you have connected the controller to another device or emummc.

The supported controllers each have their own methods for entering pairing/sync mode. Below are instructions on entering this mode for some of the common console controllers.

***Nintendo Wii/WiiU Controllers***
Press the red sync button on the back of the controller. The controller LEDs will blink rapidly.

It is recommended that you perform an analog stick calibration for these controller types where applicable, as every controller has different analog stick range and center position but unlike Switch controllers, there is no stored factory calibration.

***Sony Dualshock3 Controller***
To pair this controller, you will need to connect it to the console via USB cable. Once the controller LEDs start flashing, disconnect the USB cable and hit the `PS` button.

*Note: to avoid unwanted behaviour if using the controller in USB wired mode, this only works from the usual `Controllers->Change Grip/Order` screen.*

***Sony Dualshock4/Dualsense Controllers***
Press and hold the `PS` + `share` buttons simultaneously until the lightbar starts blinking. When done correctly the blink pattern will resemble a heartbeat, otherwise it will blink on and off at a constant rate.

If you have difficulty getting the controller to pair to the console, press and hold the reset button on the back of the controller for a few seconds and try again. Sometimes this is required after having connected to a Playstation console or other device.

***Microsoft Xbox One/Elite 2 Controllers***
Press and hold the `guide`(`X`) button until the LED starts blinking. Then press and hold the small sync button on the back near the charging port until the LED starts blinking more rapidly.

*Note: controller firmware versions 5.xx.xxxx.x and upward use Bluetooth Low Energy and are not currently supported. Please refer to the [FAQ](#frequently-asked-questions) for instructions on downgrading to a compatible firmware*

***Other Controllers***
Please refer to your controller's user manual for information on how to put it into sync mode. Note that many generic Bluetooth controllers can be started in one of several modes. Usually you want to choose something like HID, PC or Android mode for it to work correctly.

Controllers that successfully pair but haven't been officially supported yet will display with red buttons on the `Controllers` menu to indicate their controls are not being mapped. Please open an issue to request support for such controllers.

### Module configuration

A template for the config .ini file will be installed to `/config/MissionControl/missioncontrol.ini.template`. To modify the default module settings, copy the template to `/config/MissionControl/missioncontrol.ini` and uncomment (remove the leading `;`) and modify any settings you want to change. The file is only parsed on startup, so any changes you make will require a reboot to take effect. Settings entries that can't be parsed/validated correctly are ignored. Currently there is only a small set of configuration settings, but this will be expanded upon in future releases.

- `[general]`
These are general settings for mission control features. 
    - `enable_rumble` Enable/disable rumble support for unofficial controllers.
    - `enable_motion` Enable/disable motion controls support.

- `[bluetooth]`
These settings can be used to spoof your switch bluetooth to appear as another device. This may be useful (in conjunction with a link key) if you want to use your controller across multiple devices without having to re-pair every time you switch. Note that changing these settings will invalidate your console information stored in any previously paired controllers and will require re-pairing.
    - `host_name` Override the bluetooth host adapter name.
    - `host_address` Override the bluetooth host adapter address.

- `[misc]`
These are miscellaneous controller-specific settings etc.
    - `analog_trigger_activation_threshold` Set the threshold for which ZL/ZR are considered pressed for controllers with analog triggers. Valid range [0-100] percent.
    - `dualshock3_led_mode` Set Dualshock 3 player LED behaviour. Valid modes [0-1] where 0=Switch pattern, 1=PS3 pattern, 2=Hybrid (Switch pattern reversed to line up with numeric labels on the controller)
    - `dualshock4_polling_rate` Set polling rate for Sony Dualshock 4 controllers. Valid range [0-16] where 0=max, 16=min. Refer [here](https://github.com/ndeadly/MissionControl/blob/4a0326308d1ff39353b045f5efb1a99c4a504c28/mc_mitm/source/controllers/dualshock4_controller.hpp#L21) for corresponding frequency values.
    - `dualshock4_lightbar_brightness` Set LED lightbar brightness for Sony Dualshock 4 controllers. Valid range [0-9] where 0=off, 1=min, 2-9=12.5-100% in 12.5% increments.
    - `dualsense_lightbar_brightness` Set LED lightbar brightness for Sony Dualsense controllers. Valid range [0-9] where 0=off, 1=min, 2-9=12.5-100% in 12.5% increments.
    - `dualsense_enable_player_leds` Enable/disable the white player indicator LEDs below the Dualsense touchpad.
    - `dualsense_vibration_intensity` Set Dualsense vibration intensity, 12.5% per increment. Valid range [1-8] where 1=12.5%, 8=100%.

### Removal

To functionally uninstall Mission Control and its components, all that needs to be done is to delete the following directories from your SD card and reboot your console.

* `/atmosphere/contents/010000000000bd00`
* `/atmosphere/exefs_patches/bluetooth_patches`
* `/atmosphere/exefs_patches/btm_patches`

If you wish to completely remove all traces of the software ever having been installed (telemetry excepted), you may also want to follow these additional steps

* Remove the following directory from your SD card
    * `/config/MissionControl`

* Wipe the Bluetooth pairing database via `System Settings->Controllers and Sensors->Disconnect Controllers`

### Planned/In-progress Features
Below is a list of features I am currently working on or would like to look into in the future, roughly in descending order of priority. Requests are welcome if you have an idea you think would make a useful feature.

* ~~Rumble support~~
* ~~Motion controls support~~
* Bluetooth LE support
* USB wired controllers
* UART MITM to allow button combos and other future features to apply to joycons in handheld mode
* Per-controller configurations
    * Rumble on/off
    * Motion controls on/off
    * Identify as Pro Controller or Joycon
    * Set controller body/button colours
    * Invert analog stick axes
    * Analog stick deadzones
* Companion application
    * Pairing database management
        * View paired controller information
        * Clear database
        * Export database to file
        * Import existing database from file
    * Controller management/diagnostics
        * Manage controller configurations
        * View raw HID report data
        * Test buttons/analog sticks
        * Dump SPI flash (official controllers only)
    * Controller discovery/pairing reimplementation
* Tesla overlay
* Keyboard and mouse support
* Gamecube mode (analog trigger support)
* Title-specific button bindings

### Known Issues and Limitations

* Non-Switch controllers cannot be used to wake the system from sleep.
* Controllers using the Bluetooth LE (BLE) standard are currently not supported and will not connect to the system.
* Some controllers can take some time to be detected and subsequently pair with the console. Be patient and re-enter the sync mode of the controller several times if neccessary. Once synced, controllers should connect and work as usual.
* Xbox One controllers cannot be switched off via software and will attempt to reconnect to the console after being disconnected. This is a limitation of the controller's bluetooth firmware. To switch the controller off, the guide button must be held in for several seconds.
* Reported controller battery levels may not be correct. I'm relying entirely on reverse engineering notes found on the internet for these. In many cases I don't own the controller and there is simply no information available, so these controllers will always show full battery. Any help in improving this is most welcome.
* Several users have reported knockoff WiiU and Dualshock4 controllers that cannot be detected by the console during Bluetooth discovery. Unfortunately I think they're using an incompatible Bluetooth chipset.
* Mission Control stores configuration data for each paired controller in the `/config/MissionControl/controllers` directory. If any part of this directory tree becomes corrupted, controllers may be disconnected when attempting to read configuration data fails.
* When using Wii controllers with MotionPlus, the controller must be switched on while sitting button side down on a flat surface in order to be calibrated properly. Motion axes will be messed up otherwise.
* Wii extension controllers are sometimes detected incorrectly when MotionPlus is present. This issue appears to be timing related and can be resolved by reconnecting the extension as necessary.

### Frequently Asked Questions

***Does this run on \<insert CFW here\>?***
No. Mission Control will only run under Atmosphère. This is not some attempt to lock out users of other CFW, Atmosphere is simply the only one providing the extensions neccessary to MITM Bluetooth communications that make this sysmodule possible.

***Will using this get me banned from online?***
Currently there haven't been any confirmed cases of bans as a result of running Mission Control. That said, running any unofficial software under CFW will always carry a non-zero risk of ban, and Nintendo could change their ban criteria at any point. While Mission Control should be relatively safe, as it simply emulates a Pro Controller being connected, it would certainly be possible to detect that you had connected unofficial controllers to the console if Nintendo were interested in doing so. Use at your own discretion.

***Does this support USB controllers?***
No, Mission Control is currently Bluetooth-only. For now you can use cathery's [sys-con](https://github.com/cathery/sys-con) for USB controllers.

***Does this work with sys-con installed?***
Yes, the two can be run simultaneously without issue.

***My console is crashing on boot because of this sysmodule. What can I do?***
If you're seeing crashes on boot with Mission Control's title ID (`010000000000bd00`), it is likely either you have updated recently to a new Atmosphere release and an update to Mission Control is required, or you are running an old version of Atmosphere which is not compatible with the latest version of Mission Control.
Crashes in `sm` (title ID `0100000000000004`) can indicate version incompatibilities between your current Atmosphere and one or more of your homebrew sysmodules. This may be caused by Mission Control, or it could be another custom sysmodule that uses libstratosphere, even if it looks as though Mission Control is to blame (`ldn_mitm` and `emuiibo` are common offenders). If you've just updated Atmosphere you should always check if there have also been updates released for the sysmodules you use.
qlaunch errors (title ID `0100000000001000`) can be a sign that you have too many custom sysmodules running and are depleting the limited system resources available to them. Check your `/atmosphere/contents` folder and verify you actually need everything in there. If you don't know what you're doing, it may be easier to just delete this folder entirely, reinstall atmosphere, and then explicitly reinstall only the sysmodules you need.

***I installed Mission Control but it doesn't do anything. Help!***
Mission Control is primarily a background process. There are no visual changes to your system to indicate it's installed other than your controller successfully connecting through Nintendo's official menus. If you've followed the Usage and Pairing instructions above and you can't make it work, here's a basic troubleshooting checklist.
- Firstly, make sure you've rebooted the console after installing. The module won't be loaded otherwise.
- Make sure your console isn't in Flight Mode. If it is you will need to either disable it, or explicitly enable Bluetooth under Flight Mode settings.
- Confirm that Mission Control is running. To do this, you can connect a left Joycon or Pro Controller wirelessly and press the `DPAD_UP` + `MINUS` buttons together. This will act as the capture button and take a screenshot if the module is running. If you don't see a screenshot notification, it's likely that Mission Control isn't being loaded. This is usually due to a bad install and can happen for several reasons:
    - Archive bits have been set on one or more components in the Mission Control directory tree. This can happen if you use a Mac to transfer files or obtain Mission Control from unofficial sources. Try running Hekate's archive bit fix tool.
    - Software you are using hasn't copied the files over correctly. I have seen FTP clients that don't copy empty files at all, and archive software that doesn't unzip directly to SD correctly. Try extracting the .zip archive to your PC first before transferring, and use a reputable transfer method such as Hekate UMS/Haze (Atmosphere's included USB transfer tool) or a decent FTP client (I use WinSCP on Windows).
    - You haven't followed the install instructions correctly and have either excluded files or placed them in the wrong place.
    - SD card corruption. You may need to format or replace your SD card.
- Check that the controller you're trying to use is in the list of supported controllers. In particular, if you have an Xbox controller, make sure you're using a compatible model and that you're not updated to the newer Bluetooth LE firmware. Controllers using Bluetooth LE are not currently supported.
- Make sure your controller isn't an unofficial clone. This is particularly common with Dualshock 3 and 4 controllers. Many clones will work, but there are some that just refuse. 
- Make sure your controller battery is sufficiently charged. Sometimes controllers will have enough charge to start pairing, but will keep switching off halfway through (before they can report their battery level to the console).
- If you've tried all of the above and nothing works, seek help on my [Discord server](https://discord.gg/gegfNZ5Ucz).

***How can I use this with multiple sysNAND/emuMMC launch configs?***
~~Pairing controllers across multiple unique HOS installations requires multiple pairing databases and is essentially the same as pairing with two different consoles. The only exception being the case where you paired the controller(s) prior to making sysNAND copies. For now you will have to re-pair your controllers when switching back and forth. In the future I hope to include an option to load/store the database on the SD card to avoid this issue.~~ Since version 1.5.1, Atmosphere now contains code I contributed to synchronise the bluetooth pairing database between sysNAND and emuMMC via a file on the sd card. This can be activated by adding `enable_external_bluetooth_db = u8!0x1` under the `[atmosphere]` section in `atmosphere/config/system_settings.ini`. Note: this feature requires atmosphere to be running in order to function. As such, it cannot be used to synchronise sysCFW/emuMMC with stock/OFW.

***Can I remap controller buttons using Mission Control?***
Yes. Since Mission Control emulates official Pro Controllers, you can remap them using the official method introduced by Nintendo in firmware 10.0.0. You can find the remapping options in the system menu under `System Settings->Controllers and Sensors->Change Button Mapping`.

***My console shows a "Paired" notification but my controller doesn't connect, what's wrong?***
Your controller has successfully paired with the console but is being disconnected shortly after, before it can start sending inputs. This can happen for a variety of reasons, the most common being:
- Your controller is not officially supported by Mission Control and hasn't been assigned an input handler. Double-check the [Supported Controllers](#supported-controllers) list for your controller. Please open a controller request [issue](https://github.com/ndeadly/MissionControl/issues/new/choose) so that I can add support if it's not present.
- Your controller battery is low and needs to be replaced or recharged.
- Your controller's virtual memory file or the directory tree containing it has been corrupted. Try deleting the controller's config entry (`/config/MissionControl/controllers/<xxxxxxxxxxxx>/`, where `<xxxxxxxxxxxx>` is the 12-character hex representation of your controllers Bluetooth MAC address) and letting Mission Control create a new one. It may be necessary to delete the entire `controllers` directory in some cases. Note: you will lose any stored controller specific data such as user analog stick or motion calibrations when deleting these files. As this is the most destructive measure, you should attempt it last, after exhausting the suggestions above.

***My Xbox controller won't connect, I thought you said they were supported?***
Although they may look similar, not all Xbox controllers are created equal. There are actually several hardware revisions/models available (7 at the time of writing) with varying wireless capabilites. On Xbox consoles (or PC with the wireless USB adapter) all controllers use a proprietary Microsoft wireless protocol known as GIP. Bluetooth connectivity, however, is _not_ the same thing and varies between controller models. Some support bluetooth, and some don't. Of those that do, some are using the newer (currently unsupported) Bluetooth Low Energy (LE) standard or will switch to it after a firmware update. **The only supported models are the 1708 (Xbox One S) and 1797 (Xbox Elite V2) revisions. If these have been updated to a Bluetooth LE firmware (5.xx.xxxx.x and above), you will need to downgrade the firmware to the legacy version (see below).**. Controller model numbers can be found on the inside of the battery compartment, or the back of the controller in controllers with an internal battery.

For more details on the various controller revisions (with images), see [here](https://en.wikipedia.org/wiki/Xbox_Wireless_Controller#Summary).

***My Xbox One/Elite V2 controller used to connect and now it doesn't, what gives?***
As of late 2021, Microsoft introduced a new controller firmware that aims to bring Xbox One/Elite 2 controllers in line with the newer Series X|S controllers. Updating to this firmware switches the controller over to using Bluetooth Low Energy (LE), a newer bluetooth standard focused on low power consumption, which is not currently supported by Mission Control. If your controller firmware is version 5.xx.xxxx.x or above, you have the new LE firmware and will need to downgrade to the legacy one (see https://support.xbox.com/en-US/help/hardware-network/accessories/controller-firmware-reversion)

***Can you add support for Xbox 360 controllers?***
No, not currently. These don't use Bluetooth. Try sys-con with a wireless USB adapter.

***Can you add support for wake from sleep?***
Probably not. As far as I know, wake from sleep involves a controller sending a special control command to the Switch Bluetooth hardware. There is no way to make a non-switch controller send the command recognised by the Switch without modifying its hardware/firmware.

***Can you add bluetooth audio support?***
~~No. The bluetooth module on the switch only implements a small set of services required to make hid controllers work. Of this small set of services, only a handful of high-level functions are exposed to the rest of the system. Adding audio support would require implementing the services neccessary for audio transport, for which any sane person would require an open-source re-implementation of the bluetooth module in order to have access the low-level functions required to pull it off.~~ ~~As of firmware 12.0.0 Nintendo have added functions supporting Bluetooth audio. While the feature hasn't been enabled in official software, plutooo has created an experimental sysmodule called [nx-btred](https://github.com/plutooo/nx-btred) that enables Bluetooth audio in games that support recording. There isn't much benefit to me adding its functionality to Mission Control.~~ Since firmware 13.0.0 Nintendo now officially supports Bluetooth audio.

***My controller has an audio jack, can you add headset support?***
Unlikely. As far as I know, controllers supporting headset audio do so via proprietary or non-standard means. This would be a lot of work, not only to understand how it works for a particular controller, but also to integrate it into HOS somehow when it has no concept of a gamepad supporting audio. In the best-case event a controller was using some form of standard Bluetooth audio, you would still be subject to the usual bandwidth constraints of the console (choppy audio, laggy controller inputs etc). Just use regular headphones.

### How it works

Mission Control works by Man-In-The-Middling the `bluetooth` system module and intercepting its initialisation IPC commands and system events, and translating incoming/outgoing data to convince the Switch that it's communicating with an official Pro Controller.

To achieve this, the `btdrv.mitm` module obtains the handles to `bluetooth` system events and shared memory when the system attempts to initialise them over IPC via the `btm` and `hid` modules. It then creates its own secondary versions of these and passes their handles on instead of the original. This allows modifications to be made to any data buffers before notifying (or not) the system. Additionally, the `WriteHidData` IPC command is intercepted to translate or drop outgoing requests to the controller. In the case of the latter, fake responses can be written directly to the buffer in shared memory.

Intercepting initialisation IPC commands also allows homebrew to properly make use of the `bluetooth` service. Normally, calling any of the IPC commands that would initialise or finalise system events would either crash the console, or invalidate the event handles held by system processes. With `btdrv.mitm` we are able to hand out alternative event handles when homebrew attempts to initialise an interface, and redirect the real system events to those instead of the events held by system processes.

exefs patches to the `bluetooth` module are provided to enable the pairing of Wii/WiiU and other controllers that makes use of legacy pincode pairing, Xbox Elite 2 Wireless controllers, and to relax device class checks added on newer firmwares to also allow devices identifying as keyboard or joystick to be connected.

exefs patches to the `btm` module have been added to skip over calls to `nn::bluetooth::hal::CloseHidConnection` when a controller fails to respond correctly to the broadcom vendor command sent by `nn::bluetooth::hal::SetTsi`. This prevents all affected controllers from being disconnected immediately after connection, and eliminates the need to manually flag certain controllers with a `settsi_disable.flag` file.

The `btm` service is now also MITM'd, allowing for faking controller names on the fly while retaining the original names in the pairing database.

### Building from source

First, clone the repository to your local machine and switch to the newly cloned directory
```
git clone --recurse-submodules https://github.com/ndeadly/MissionControl.git
cd MissionControl
```

~~Mission Control currently uses a custom fork of `libnx` that adds Bluetooth service wrappers and type definitions.~~ Official libnx master is now used to build Mission Control. At the time of writing, the libnx distributed by devkitPro can be used without the need to build it yourself. This may change if `Atmosphere-libs` updates to use bleeding edge `libnx` commits not present in the official release. In any case, you can build the included `libnx` submodule from source with the following commands.

```
cd lib/libnx
make && make install
```

Next build `libstratosphere`. If you encounter any build errors, you may be missing required dependencies (refer to https://github.com/Atmosphere-NX/Atmosphere/blob/master/docs/building.md)
```
cd ../Atmosphere-libs/libstratosphere
make
```

Finally, build and package the distribution .zip. This will build the `mc.mitm` sysmodule and package it up with bluetooth exefs patches. 
```
cd ../..
make dist
```

The resulting package can be installed as described above.

### Credits

* [__switchbrew__](https://switchbrew.org/wiki/Main_Page) for the extensive documention of the Switch OS.
* [__devkitPro__](https://devkitpro.org/) for the homebrew compiler toolchain.
* __SciresM__ for his dedicated work on the [Atmosphère](https://github.com/Atmosphere-NX) project, libstratosphere and general helpfulness with all things Switch related.
* __misson20000__ for his handy debug monitor [Twili](https://github.com/misson20000/twili) and IPC logger [Ilia](https://github.com/misson20000/ilia)
* __dekuNukem__, __CTCaer__, __shinyquagsire23__ and others for their work in reversing and documenting the switch controller communication protocol.
* __Banz99__ for ongoing code contributions, discussing ideas, testing and generally keeping me on my toes.
* __friedkeenan__ for helping to test Wii extension controller support.
* __DatenThielt__ for helping debug the bluetooth service remotely with his Xbox Elite Series 2 controller in order for me to develop patches to enable it to be successfully paired with the console.
* Everyone else over at the __ReSwitched__ discord server who helped answering technical questions.

### Support

If you like this project, please consider supporting me to continue its development :)


<a href="https://ko-fi.com/J3J01BZZ6"><img border="0" alt="ko-fi" src="https://www.ko-fi.com/img/githubbutton_sm.svg" align="left"></a>