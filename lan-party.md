# LAN-Party mit Enshrouded

Enshrouded im eigenen WLAN, mit einem Dedicated Server auf einem Rechner im Netz. Bis zu 16 Spieler bauen, craften und kämpfen gemeinsam.

## Was ihr braucht

1. Einen Rechner als Server, unter Windows.
2. Den Enshrouded Dedicated Server, kostenlos über Steam (Bibliothek, Filter "Werkzeuge") oder per SteamCMD mit anonymem Login (App-ID 2278520).
3. Pro Spieler einen Rechner mit Enshrouded über Steam.
4. Ein gemeinsames Netz, alle im selben WLAN oder LAN.

## Server einrichten

1. Den Server-Ordner öffnen, zum Beispiel `C:\Program Files (x86)\Steam\steamapps\common\EnshroudedServer`.
2. `enshrouded_server.json` anpassen:
    1. `name`: der Servername, unter dem ihn alle finden.
    2. `slotCount`: maximal 16.
    3. `userGroups`: für jede Gruppe ein eigenes Passwort setzen, zum Beispiel Admin und Friend.
    4. `ip` (`0.0.0.0`) und `queryPort` (`15637`) bleiben unverändert.
3. `enshrouded_server.exe` starten. Der Steam-Client muss dafür nicht laufen.
4. Wenn die Windows-Firewall nachfragt, den Zugriff im privaten Netzwerk erlauben.
5. Die lokale IP des Server-Rechners notieren, in PowerShell mit `ipconfig` (IPv4-Adresse, zum Beispiel `192.168.0.10`).

## Mitspielen

1. Enshrouded starten und unter "Spielen" die Serverliste öffnen.
2. Den Server über seinen Namen suchen und beitreten.
3. Alternativ: in Steam unter "Ansicht", "Spielserver", "Favoriten" die Adresse `192.168.0.10:15637` hinzufügen.
4. Das Passwort der passenden Gruppe eingeben.

## Ohne Internet

1. Der Download des Servers braucht einmal Internet, danach läuft er auch offline.
2. Die Spieler starten Steam vorher einmal online und dann im Offline-Modus.
3. Noch zu testen: ob die Serverliste den Server ohne Internet anzeigt oder ob der Weg über die Favoriten nötig ist.

## Spielstände

1. Die Welt liegt im Server-Ordner unter `savegame`.
2. Vor jeder Party eine Kopie dieses Ordners anlegen.

## Quellen

1. [Offizielle Installationsanleitung](https://enshrouded.zendesk.com/hc/en-us/articles/16051370691485-Dedicated-Server-Installation-on-Steam)
2. [Offizielle Konfigurationsanleitung](https://enshrouded.zendesk.com/hc/en-us/articles/16055441447709-Dedicated-Server-Configuration)
3. [Offizielle Dedicated-Server-FAQ](https://enshrouded.zendesk.com/hc/en-us/articles/16056312924957-Dedicated-Server-FAQ)
4. `enshrouded_server_readme.txt` im Server-Ordner
