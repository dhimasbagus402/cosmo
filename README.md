# Cosmo

A living island at the top of your Windows screen: music and synced lyrics, a focus timer, tasks, system stats, a clipboard history, a shelf for files, an FPS overlay and more.

**Website:** https://cosmo.dhimasbagus.my.id

**Download:** [Cosmo-Setup.exe](https://github.com/dhimasbagus402/cosmo/releases/latest/download/Cosmo-Setup.exe) (Windows 10 and 11, installs for your account only, no admin needed). Once installed, Cosmo updates itself: look for **Update** in Settings › Features or the right-click menu.

The installer isn't code-signed yet. If SmartScreen shows "Windows protected your PC", choose **More info**, then **Run anyway**.

This repository holds Cosmo's releases, its website (`docs/`) and its add-ons. The source code is kept private.

## What leaves your PC

- **Lyrics:** the song's title, artist and length are sent to [LRCLIB](https://lrclib.net) to find synced lyrics. With **Extra lyric sources** switched on (Settings › Features, off by default), songs LRCLIB doesn't have are also looked up on NetEase Cloud Music. Results are kept in `%APPDATA%\Cosmo\lyrics`, so each song is looked up once.
- **Updates:** Cosmo asks GitHub for the latest release of this repository, a few seconds after it starts and then once a day. No data about you is sent. It can be switched off with **Check for updates**.
- **Add-ons:** downloaded from this repository's releases, only when switched on.

Everything else (tasks, clipboard history, settings, files on the shelf) stays on your PC, in `%APPDATA%\Cosmo`.

## Add-ons

### Kanji readings

Cosmo shows Japanese and Korean lyrics in Latin letters (**Romanized lyrics**). Kana and hangul need nothing extra; kanji need a dictionary of readings. That dictionary is an optional download of about 9 MB: switch on **Kanji readings for lyrics** under ADD-ONS in Settings › Features. Switching it off deletes it again.

The file, `cosmo-ja-readings.txt`, is published under the [addons release](https://github.com/dhimasbagus402/cosmo/releases/tag/addons). It is made from the [JMdict](https://www.edrdg.org/wiki/index.php/JMdict-EDICT_Dictionary_Project) and [KANJIDIC2](https://www.edrdg.org/wiki/index.php/KANJIDIC_Project) files, which are the property of the [Electronic Dictionary Research and Development Group](https://www.edrdg.org/) and are used in conformance with the Group's [licence](https://www.edrdg.org/edrdg/licence.html). Like its sources, it is licensed under [Creative Commons Attribution-ShareAlike 4.0](https://creativecommons.org/licenses/by-sa/4.0/).

It also maps simplified Chinese characters, which some lyrics sites use for Japanese songs, to the Japanese kanji they stand for. That mapping comes from the Unihan database in the [Unicode Character Database](https://www.unicode.org/ucd/), © Unicode, Inc., used under the [Unicode License v3](https://www.unicode.org/license.txt).
