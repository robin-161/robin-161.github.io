Signal ist ein weithin anerkannter Instant-Messaging-Dienst, der nicht nur einfach zu bedienen, sondern auch privat und sicher ist. Die starke  Ende-zu-Ende-Verschlüsselung und der Metadatenschutz von Signal bieten die Gewissheit, dass nur du und die vorgesehenen Empfänger:innen die Kommunikation lesen können.
Hier möchte ich dich darüber informieren, wie du Signal richtig konfigurierst und absicherst.

# Signal-PIN festlegen und die Registrierungssperre aktivieren
Nachdem du dich bei Signal registriert hast, solltest du sofort deinen Signal-PIN festlegen und die Registrierungssperre aktivieren. Mit deinem Signal-PIN kannst du dein Profil, deine Einstellungen, deine Kontakte und deine Blockliste wiederherstellen, falls du einmal dein Gerät verlieren oder wechseln solltest.

> ⓘ Es gibt keine Zeichenbegrenzung für den Signal-PIN

Wenn jemand die Kontrolle über deine Telefonnummer erhält und sich neu bei Signal anmelden möchte, ist durch die Registrierungssperre dein Signal-PIN erforderlich. 

*Gehe zum aktivieren in deine Signal-Einstellungen wähle den Punkt "Konto" und aktiviere die Regestrierungssperre*

> ⓘ Die Registrierungssperre läuft nach 7 Tagen der Inaktivität ab. "Inaktivität" bedeutet, dass deine Signal-App innerhalb dieses Zeitraums keine Verbindung zu den Signal-Servern herstellt hat

Ohne diesen PIN kann der Angreifer sich erst nach 7 Tagen erneut anmelden und die damit verbundenen Informationen (Profil, Einstellungen, Kontakte & Blockliste) sind nicht mehr verfügbar.

**Wichtig:**
- Dein PIN ist kein Backup. Dein Nachrichtenverlauf ist nicht mit dieser PIN verknüpft und eine PIN kann nicht verwendet werden, um deinen Nachrichtenverlauf wiederherzustellen
- Dein PIN kann nicht zurückgesetzt oder wiederhergestellt werden
- Wenn du deine PIN vergessen hast und die Registrierungssperre aktiviert ist, ist dein Konto für 7 Tage gesperrt

Weitere Informationen über den Signal-PIN findest du auf der [Website von Signal](https://support.signal.org/hc/de/articles/360007059792-Signal-PIN).

# Sicherheitsnummern
Jede Signal-Unterhaltung hat eine eindeutige Sicherheitsnummer, die es dir ermöglicht, die Sicherheit deiner Nachrichten und Anrufe mit bestimmten Kontakten zu verifizieren.

Die Sicherheitsnummer ändert sich, wenn ein Kontakt zu einem neuen Telefon wechselt oder Signal neu installiert. Wenn sich eine Sicherheitsnummer häufig oder unerwartet ändert, kann dies ein Zeichen für einen [Man-in-the-Middle-Angriff](https://en.wikipedia.org/wiki/Man-in-the-middle_attack) sein. 

Die manuelle Überprüfung von Sicherheitsnummern ist gute Sicherheitspraxis für private Kommunikation. 

> ⓘ Falls eine Sicherheitsnummer als 'verifiziert' gekennzeichnet ist, muss jede Änderung dieser Nummer bestätigt werden, bevor eine neue Nachrichten gesendet werden

Weitere Informationen über Sicherheitsnummern findest du auf der [Website von Signal](https://support.signal.org/hc/de/articles/360007060632-Was-ist-eine-Sicherheitsnummer-und-weshalb-sehe-ich-dass-sie-sich-ge%C3%A4ndert-hat-).

# Verschwindene Nachrichten
Während die Kommunikation in Signal Ende-zu-Ende-verschlüsselt ist, sind die Nachrichten weiterhin auf den Geräten verfügbar, sofern sie nicht manuell gelöscht werden.

Es empfiehlt sich, in den Einstellungen von Signal die Option "Verschwindende Nachrichten" zu aktivieren, so dass alle Nachrichten, nach einer bestimmten Zeit verschwinden.

> ⓘ Diese Änderung gilt **nur** für neue Chats. Nachrichten aus Chats, die du vor der Änderung gestartet hast, verschwinden nicht automatisch

**Achtung:** Wenn jemand eine "Verschwindende Nachricht" erhält kann dieser eine Aufzeichnung, z.B. druch ein Bildschirmfoto, machen bevor die Nachricht verschwindet.

# Privatsphäre
Ich empfehle folgende Einstellungen:
- "Bildschirmsperre" aktivieren (sperrt die Signal-App mit der Bildschirmsperre deines Geräts)
- "Bildschirmsicherheit" aktivieren (Screenshots werden blockiert)
- "Inkognito-Tastatur" aktivieren (verhindert, dass deine Tastatur-App deine Unterhaltungen aufgrund von Personalisierung speichert)
- "Lesebestätigungen" deaktivieren (damit andere nicht sehen können, ob du ihre Nachrichten gelesen hast)
- "Tippindikatoren" deaktivieren (damit andere nicht sehen können, wenn du eine Nachricht tippst)
- "Linkvorschau senden" deaktivieren (damit es keine zusätzlichen Netzwerkverbindungen gibt)
- "Anzeigeindikatoren" für die Funktion "Vertraulicher Absender" aktivieren und die Einstellung "Von jedem zulassen" deaktiviert lassen

# Gruppen-Links
**Hinweis:** Sollte ein Gruppen-Link in die falschen Hände geraten und die Einstellung "Neue Mitglieder bestätigen" ist eingeschaltet, kann trotzdem  jede Person mit dem Link auf die Gruppenbeschreibung zugreifen. **Gruppenbeschreibungen sind also kein Ort für sensible Informationen wie z.B. Links zu nicht öffentlichen Daten oder Passwörter!**

# Gerätesicherheit
Signal nimmt Sicherheit sehr ernst, allerdings kann eine App nur einen gewissen Schutz bieten. Es ist sehr wichtig, die Gerätesicherheit auf beiden Seiten der Kommunikation zu berücksichtigen, um sicherzustellen, dass deine Unterhaltungen privat bleiben.

Ich empfehle ein aktuelles [GrapheneOS](https://grapheneos.org)- oder iOS-Gerät.

# Molly (Android)
Auf einem Android-Gerät kannst du [Molly](https://molly.im) nutzen, ein Fork der Signal-App, der umfangreiche Sicherheits- und Anti-Forensik-Funktionen bieten soll.

Molly hat eine Datenbankverschlüsselung im Ruhezustand implementiert, was bedeutet, dass du die Datenbank der App mit einer Passphrase verschlüsseln kannst, um sicherzustellen, dass keine der Daten ohne dich zugänglich ist.

> ⓘ Solange Molly gesperrt ist, erhälst du keine Benachrichtigungen über eingehende Nachrichten oder Anrufe, bis du die App entsperrst

Eine vollständige Liste der Funktionen von Molly findest du auf der [Website des Projekts](https://molly.im).

Vorbehalte:
- Molly wird alle zwei Wochen aktualisiert, um die neuesten Funktionen und Fehlerbehebungen von Signal aufzunehmen. Die Ausnahme sind Sicherheitsprobleme, die so schnell wie möglich behoben werden. Dennoch solltest du dir bewusst sein, dass es zu einer leichten Verzögerung im Vergleich zur Signal-App kommen kann
- Durch die Nutzung von Molly musst du dein Vertrauen auf eine weitere Partei ausweiten, da du nun sowohl dem Signal-Team als auch dem Molly-Team vertrauen musst

## Quellen:
- [Signal-Support](https://support.signal.org/hc/de)
- [Wiki der Letzten Generation - Signal sicher benutzen](https://wiki.letztegeneration.de/de/%C3%B6ffentlich/IT-Hilfe/Signal/Signal-sicher-benutzen)
- [blaeul.de - Signalgruppen und Einladungslinks](https://blaeul.de/sonnenschein/signalgruppen-und-einladungslinks)
- [Privacy Guides - 2022 Signal Configuration and Hardening Guide](https://blog.privacyguides.org/2022/07/07/signal-configuration-and-hardening/)
- [Infosec Handbook - How to use Signal more privacy-friendly](https://web.archive.org/web/20210705170700/https://infosec-handbook.eu/blog/signal-privacy/#configuration)
