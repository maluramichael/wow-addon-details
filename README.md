# wow-addon-details

Meine Kopie des WoW-Addons [Details! Damage Meter](https://github.com/Tercioo/Details-Damage-Meter) von Tercioo. Ich habe das Addon nicht geschrieben, ich habe es nur hierher gelegt, um einen Fehler zu beheben, der mich im Spiel gestört hat.

## Meine Änderung

In `Libs/PlayerInfo/PlayerInfo.lua` prüft `commHandler.SendData` jetzt, ob `encodedString` überhaupt gesetzt ist, bevor es weitergereicht wird. Ohne diese Prüfung lief ein `nil` in `SendCommMessage` und es gab einen Lua-Fehler, wenn eine der Encoding-Funktionen nichts zurückgab.

## Hinweis

Der Rest des Codes ist der Stand des Originals vom Dezember 2025 (Version `Details.20251225.14203.166`) und stammt von Tercioo und den anderen Mitwirkenden. Für alles außer der einen Zeile ist das Original-Repository die richtige Adresse. Lizenz siehe `LICENSE`.
