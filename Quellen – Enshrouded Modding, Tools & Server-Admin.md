# Quellen – Enshrouded Modding, Tools & Server-Admin

Stand: Oktober 2026 (nach 1.0-Release)

---

## 1. Offizielle Quellen (Keen Games)

- **Dedicated Server FAQ / Config**  
  https://enshrouded.zendesk.com/hc/en-us  
  (bzw. die aktuellen Dedicated-Server-Artikel auf der offiziellen Support-Seite)

- **Steam Dedicated Server** (App-ID 2278520)  
  Kostenlos über SteamCMD installierbar.  
  Kein Kauf des Spiels nötig.

- **Server-Config-Datei**  
  `enshrouded_server.json` (wird beim ersten Start erzeugt)  
  Enthält userGroups (Admin/Friend/Guest/Visitor), gameSettingsPreset und alle gameSettings.

**Wichtig:** Es gibt **keine** offiziellen Admin-Konsolen-Befehle, kein RCON und kein Chat-Command-System. Alles läuft über Rollen-Passwörter + In-Game Social-Tab.

---

## 2. Modding / Toolkit / Loader

### Embervale Toolkit
- **Website / Download:** https://enshrouded.gamevault.in/mod  
- Creative Mode, Mod Creator (Werte patchen), Cinematic Camera, First Person, HUD aus, Enemy Placement, Terraforming usw.  
- Kostenlos für Client, Patreon-Version für Dedicated Server.  
- Standalone-App (kein Cheat Engine).

### Enshrouded Mod Loader (EML) + kfc-parser
- **GitHub:** https://github.com/Brabb3l/kfc-parser  
- **Dokumentation:** https://brabb3l.github.io/kfc-parser/  
- **Releases:** https://github.com/Brabb3l/kfc-parser/releases  
- Lua-basierter Loader (dbghelp.dll Proxy).  
- Patcht Spieldaten vor dem Start (Stackgrößen, Rezepte, XP, etc.).  
- Version 0.2.0 hat 1.0-Support.

### ember-platform / enshrouded-ember (Rust SDK)
- **GitHub:** https://github.com/zachthedev/enshrouded-ember  
- **crates.io:** ember-sdk, ember-platform, ember-enshrouded, ember-holistic  
- Tiefes Server-Modding in Rust (cdylib + Hooks + Reflection).  
- Noch 0.x / in Entwicklung. Sehr interessant für fortgeschrittenes Programmieren.

### Weitere Loader / Tools
- **ShroudForge:** https://github.com/bonsaibauer/shroudforge  
- **M182 Admin Panel (Nexus):** https://www.nexusmods.com/enshrouded/mods/168  
  Insert-Taste → Spawn Creatures/Items, PvP, Safe Zones, Teams usw. (nur Host muss installieren).

---

## 3. Server-Manager & Admin-Tools

### Desktop / Browser Manager
- **Enshrouded Server Manager (Crazyloon)**  
  https://github.com/Crazyloon/Enshrouded-Server-Manager  
  MIT, Profile, Auto-Backup, Restore, Update-Checks.

- **Enshrouded Server Manager by Zat** (Browser-basiert)  
  Reddit-Thread: https://www.reddit.com/r/Enshrouded/comments/1wafx7o/i_made_a_server_manager/  
  Multi-Server, Crash-Restart, JSON-Editor, User-Groups, FTP-Backups, Version 0.9.4 (Okt 2026).

- **SMM-Enshrouded:** https://github.com/SYSOFTEK/SMM-Enshrouded  
  Monitoring (CPU/RAM), Config-Editor, Konsolen-Anzeige.

- **YotaPower04 (Linux + GE-Proton):** https://github.com/YotaPower04/enshrouded-server-manager

- **WindowsGSM + Enshrouded-Plugin**  
  https://windowsgsm.com + Community-Plugin von ohmcodes.

### Config-Generatoren
- https://tools.supercraft.host/games/enshrouded (Config Generator + Save Rollback)
- Verschiedene Hosting-Panels (PlayNHost, EVLBOX, Loafhosts usw.) haben eigene Config-Editoren.

---

## 4. Monitoring & Server-Listen

- https://gamemonitoring.net (sehr viele Enshrouded-Server)
- BattleMetrics (Spieler-Tracking)
- Steam Server Browser + In-Game Serverliste

---

## 5. Wikis, Maps & Datenbanken

- **Offizielle Wiki:** https://enshrouded.wiki.gg  
- **enshrouded.tools:** https://www.enshrouded.tools (Map, Skill-Tree, Items, etc.)  
- **Pindrop:** https://pindrop.gg/enshrouded (sehr umfangreiche interaktive Map + Planner)  
- **MapGenie:** https://mapgenie.io (Enshrouded-Map)

---

## 6. VR / UEVR (nur zur Erinnerung)

- **UEVR (praydog):** https://github.com/praydog/UEVR  
- Funktioniert **nicht** mit Enshrouded (Holistic Engine).  
- Solarpunk (UE5) wäre theoretisch möglich.

---

## Kurze Notizen für dich

- Dedicated Server (App 2278520) = kostenlos.  
- Spiel selbst kostet ca. 35–40 €.  
- Embervale Toolkit + EML + ember-SDK sind die drei interessantesten Kandidaten fürs Weiterarbeiten.  
- Alles inoffiziell → immer Backups machen und Testwelten nutzen.

Viel Spaß beim Durchstöbern und beim 100-Days-of-Rust-Projekt!