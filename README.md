# WatchMeDigi

Android TV aplikacija.

[Preuzmi najnoviji APK](https://github.com/sikira/watchmedigi/raw/refs/heads/main/dist/latest/WatchMeDigi.apk)

Downloader: [1727311](http://aftv.news/1727311)

## Config ažuriranja

`config.json` u korijenu ovog javnog repozitorija služi samo za opcionalnu ponudu
nadogradnje. Release skripta nakon uspješnog builda i kopiranja APK-a automatski ažurira
`latestVersionCode`, `latestVersionName` i `apkUrl` iz `app/version.properties`. Koristi URL konkretnog izdanja da verzija i APK ostanu usklađeni.
`schemaVersion` ostaje 1. U režimu `--build-only` izmjene ostaju lokalne; `--publish` ih commitira i objavljuje.
Ostala polja se čuvaju. Pri promjeni verzije `releaseNotes` se postavlja na naziv
novog izdanja; za isto izdanje postojeće bilješke ostaju sačuvane.

Config je javan; ne upisuj tajne. Klijent prihvata HTTPS APK URL samo iz
`sikira/watchmedigi` repozitorija na `github.com`. Polja za blokadu i obavezno
ažuriranje nisu podržana. Postojeće stare instalacije dobijaju ovu provjeru tek
nakon ručne instalacije novog APK-a koji sadrži UpdateChecker.
