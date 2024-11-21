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

***Läuft dies auf \<hier CFW einfügen\>?***
Nein. Mission Control wird nur unter Atmosphère ausgeführt. Dies ist kein Versuch, Benutzer anderer CFW auszusperren, Atmosphäre ist einfach die einzige, die die erforderlichen Erweiterungen zur MITM-Bluetooth-Kommunikation bereitstellt, die dieses Sysmodul möglich machen.

***Werde ich wegen der Verwendung davon online gesperrt?***
Derzeit gab es keine bestätigten Fälle von Sperren aufgrund der Ausführung von Mission Control. Dennoch trägt die Ausführung einer inoffiziellen Software unter CFW immer ein nicht zu vernachlässigendes Risiko einer Sperrung, und Nintendo könnte ihre Sperrkriterien jederzeit ändern. Obwohl Mission Control relativ sicher sein sollte, da es einfach einen Pro Controller emuliert, der angeschlossen ist, wäre es sicherlich möglich zu erkennen, dass Sie inoffizielle Controller an die Konsole angeschlossen haben, wenn Nintendo daran interessiert wäre. Verwenden Sie es nach eigenem Ermessen.

***Unterstützt dies USB-Controller?***
Nein, Mission Control unterstützt derzeit nur Bluetooth. Sie können vorerst cathery's [sys-con](https://github.com/cathery/sys-con) für USB-Controller verwenden.

***Funktioniert dies mit installiertem sys-con?***
Ja, die beiden können gleichzeitig ausgeführt werden, ohne Probleme zu verursachen.

***Meine Konsole stürzt beim Booten wegen dieses Sysmoduls ab. Was kann ich tun?***
Wenn Sie Abstürze beim Booten mit der Title-ID von Mission Control (`010000000000bd00`) sehen, liegt es wahrscheinlich entweder daran, dass Sie kürzlich auf eine neue Atmosphäre-Version aktualisiert haben und ein Update für Mission Control erforderlich ist, oder dass Sie eine alte Version von Atmosphäre verwenden, die nicht mit der neuesten Version von Mission Control kompatibel ist.
Abstürze in `sm` (Title-ID `0100000000000004`) können auf Versionsinkompatibilitäten zwischen Ihrer aktuellen Atmosphäre und einem oder mehreren Ihrer Homebrew-Sysmodule hinweisen. Dies kann durch Mission Control verursacht werden, oder es könnte ein anderes benutzerdefiniertes Sysmodul sein, das libstratosphere verwendet, selbst wenn es so aussieht, als ob Mission Control schuld ist (`ldn_mitm` und `emuiibo` sind häufige Übeltäter). Wenn Sie gerade Atmosphäre aktualisiert haben, sollten Sie immer überprüfen, ob auch Updates für die von Ihnen verwendeten Sysmodule veröffentlicht wurden.
Fehler beim Start von qlaunch (Title-ID `0100000000001000`) können darauf hinweisen, dass Sie zu viele benutzerdefinierte Sysmodule ausführen und die begrenzten Systemressourcen, die ihnen zur Verfügung stehen, aufgebraucht sind. Überprüfen Sie Ihren `/atmosphere/contents`-Ordner und stellen Sie sicher, dass Sie tatsächlich alles darin benötigen. Wenn Sie nicht wissen, was Sie tun, ist es möglicherweise einfacher, diesen Ordner vollständig zu löschen, Atmosphäre neu zu installieren und dann nur die benötigten Sysmodule explizit neu zu installieren.

***Ich habe Mission Control installiert, aber es passiert nichts. Hilfe!***
Mission Control ist hauptsächlich ein Hintergrundprozess. Es gibt keine visuellen Änderungen an Ihrem System, die darauf hinweisen, dass es installiert ist, außer dass Ihr Controller erfolgreich über die offiziellen Menüs von Nintendo verbunden ist. Wenn Sie die oben aufgeführten Verwendungs- und Kopplungsanweisungen befolgt haben und es nicht funktioniert, finden Sie hier eine grundlegende Fehlerbehebungsliste.
- Stellen Sie zunächst sicher, dass Sie die Konsole nach der Installation neu gestartet haben. Das Modul wird sonst nicht geladen.
- Stellen Sie sicher, dass sich Ihre Konsole nicht im Flugmodus befindet. Wenn dies der Fall ist, müssen Sie entweder den Flugmodus deaktivieren oder Bluetooth explizit unter den Flugmoduseinstellungen aktivieren.
- Bestätigen Sie, dass Mission Control läuft. Hierzu können Sie einen linken Joy-Con oder Pro Controller drahtlos verbinden und gleichzeitig die Tasten `DPAD_UP` + `MINUS` drücken. Dies fungiert als die Capture-Taste und nimmt einen Screenshot auf, wenn das

 Modul ausgeführt wird. Wenn Sie keine Benachrichtigung über den Screenshot sehen, wird Mission Control wahrscheinlich nicht geladen. Dies liegt normalerweise an einer schlechten Installation und kann aus mehreren Gründen passieren:
    - Archivbits wurden für einen oder mehrere Komponenten im Mission Control-Verzeichnisbaum festgelegt. Dies kann passieren, wenn Sie einen Mac zum Übertragen von Dateien verwenden oder Mission Control aus inoffiziellen Quellen beziehen. Versuchen Sie, das Archivbit-Fix-Tool von Hekate auszuführen.
    - Die von Ihnen verwendete Software hat die Dateien nicht ordnungsgemäß kopiert. Ich habe FTP-Clients gesehen, die leere Dateien überhaupt nicht kopieren, und Archivsoftware, die nicht direkt auf SD entpackt. Versuchen Sie, das .zip-Archiv zunächst auf Ihrem PC zu extrahieren, bevor Sie es übertragen, und verwenden Sie eine seriöse Übertragungsmethode wie Hekate UMS/Haze (das im Lieferumfang von Atmosphäre enthaltene USB-Übertragungstool) oder einen anständigen FTP-Client (ich benutze WinSCP unter Windows).
    - Sie haben die Installationsanweisungen nicht korrekt befolgt und Dateien ausgeschlossen oder an der falschen Stelle platziert.
    - SD-Kartenkorruption. Möglicherweise müssen Sie Ihre SD-Karte formatieren oder ersetzen.
- Überprüfen Sie, ob der Controller, den Sie verwenden möchten, in der Liste der unterstützten Controller enthalten ist. Stellen Sie insbesondere sicher, dass Sie ein kompatibles Modell eines Xbox-Controllers verwenden und dass Sie nicht auf die neuere Bluetooth-LE-Firmware aktualisiert haben. Controller, die Bluetooth LE verwenden, werden derzeit nicht unterstützt.
- Stellen Sie sicher, dass Ihr Controller kein inoffizieller Klon ist. Dies ist besonders häufig bei Dualshock 3 und 4 Controllern. Viele Klone funktionieren, aber es gibt einige, die einfach nicht funktionieren.
- Stellen Sie sicher, dass der Akku Ihres Controllers ausreichend geladen ist. Manchmal haben Controller genug Ladung, um mit der Kopplung zu beginnen, schalten sich jedoch immer wieder aus (bevor sie ihren Batteriestand an die Konsole melden können).
- Wenn Sie alles oben Genannte ausprobiert haben und nichts funktioniert, suchen Sie Hilfe auf meinem [Discord-Server](https://discord.gg/gegfNZ5Ucz).

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

### Funktionsweise

Mission Control funktioniert, indem es das `bluetooth`-Systemmodul mittels Man-In-The-Middle (MITM) abfängt und seine Initialisierungs-IPC-Befehle und Systemereignisse abfängt und eingehende/ausgehende Daten übersetzt, um die Switch davon zu überzeugen, dass sie mit einem offiziellen Pro Controller kommuniziert.

Um dies zu erreichen, erhält das `btdrv.mitm`-Modul die Handles zu den `bluetooth`-Systemereignissen und zum gemeinsamen Speicher, wenn das System versucht, sie über IPC über die `btm`- und `hid`-Module zu initialisieren. Es erstellt dann seine eigenen sekundären Versionen davon und übergibt stattdessen ihre Handles anstelle der Originalversionen. Dies ermöglicht Modifikationen an allen Datenpuffern, bevor das System benachrichtigt wird oder nicht. Darüber hinaus wird der IPC-Befehl `WriteHidData` abgefangen, um ausgehende Anfragen an den Controller zu übersetzen oder abzulehnen. Im Falle letzteres können gefälschte Antworten direkt in den gemeinsamen Speicherbuffer geschrieben werden.

Das Abfangen von Initialisierungs-IPC-Befehlen ermöglicht es auch Homebrew, den `bluetooth`-Dienst ordnungsgemäß zu nutzen. Normalerweise würde das Aufrufen eines der IPC-Befehle, die Systemereignisse initialisieren oder abschließen würden, die Konsole zum Absturz bringen oder die Ereignis-Handles, die von Systemprozessen gehalten werden, ungültig machen. Mit `btdrv.mitm` können wir alternative Ereignis-Handles bereitstellen, wenn Homebrew versucht, eine Schnittstelle zu initialisieren, und die echten Systemereignisse an diese weiterleiten, anstatt an die von Systemprozessen gehaltenen Ereignisse.

Exefs-Patches für das `bluetooth`-Modul werden bereitgestellt, um das Pairing von Wii/WiiU- und anderen Controllern zu ermöglichen, die eine Legacy-PIN-Code-Paarung verwenden, Xbox Elite 2 Wireless-Controller und um Geräteklassenüberprüfungen zu entspannen, die auf neueren Firmwareversionen hinzugefügt wurden, um auch Geräte zu ermöglichen, die sich als Tastatur oder Joystick identifizieren, verbunden zu werden.

Exefs-Patches für das `btm`-Modul wurden hinzugefügt, um Aufrufe von `nn::bluetooth::hal::CloseHidConnection` zu überspringen, wenn ein Controller nicht richtig auf den von `nn::bluetooth::hal::SetTsi` gesendeten Broadcom-Vendor-Befehl reagiert. Dies verhindert, dass alle betroffenen Controller sofort nach der Verbindung getrennt werden, und eliminiert die Notwendigkeit, bestimmte Controller manuell mit einer `settsi_disable.flag`-Datei zu markieren.

Der `btm`-Dienst wird nun ebenfalls MITM'd, was es ermöglicht, Controller-Namen während der Laufzeit zu fälschen, während die Originalnamen in der Pairing-Datenbank beibehalten werden.

### Erstellen aus dem Quellcode

Zuerst klonst du das Repository auf deinem lokalen Rechner und wechselst in das neu geklonte Verzeichnis:

```
git clone --recurse-submodules https://github.com/ndeadly/MissionControl.git
cd MissionControl
```

~~Mission Control verwendet derzeit eine benutzerdefinierte Gabelung von `libnx`, die Bluetooth-Service-Wrapper und Typdefinitionen hinzufügt.~~ Offizielles libnx-Master wird jetzt verwendet, um Mission Control zu erstellen. Zum Zeitpunkt des Schreibens kann das von devkitPro verteilte libnx ohne die Notwendigkeit, es selbst zu erstellen, verwendet werden. Dies kann sich ändern, wenn `Atmosphere-libs` aktualisiert wird, um bleeding-edge `libnx`-Commits zu verwenden, die im offiziellen Release nicht enthalten sind. In jedem Fall kannst du das enthaltene `libnx`-Teilmodul aus dem Quellcode erstellen mit den folgenden Befehlen.

```
cd lib/libnx
make && make install
```

Als nächstes erstellst du `libstratosphere`. Wenn du auf Buildfehler stößt, fehlen möglicherweise benötigte Abhängigkeiten (siehe https://github.com/Atmosphere-NX/Atmosphere/blob/master/docs/building.md)

```
cd ../Atmosphere-libs/libstratosphere
make
```

Schließlich erstellst und verpackst du die Vertriebs-Zip-Datei. Dabei wird das `mc.mitm`-Sysmodul erstellt und mit Bluetooth-Exefs-Patches verpackt.

```
cd ../..
make dist
```

Die resultierende Paketdatei kann wie oben beschrieben installiert werden.

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
