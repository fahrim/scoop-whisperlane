# whisperlane — Scoop bucket

Scoop manifests for [whisperlane](https://github.com/fahrim/whisperlane), a
free, open source, local-first dictation tool for Windows. Hold a key, talk,
release, and the words appear where your caret already is.

## Install

```powershell
scoop bucket add whisperlane https://github.com/fahrim/scoop-whisperlane
scoop install whisperlane
```

## Update

```powershell
scoop update
scoop update whisperlane
```

whisperlane has its own updater as well. If you installed it with Scoop,
update it with Scoop: the in-app updater installs over the Scoop-managed copy,
and `scoop status` will then report a mismatch.

Speech models are downloaded by the application on first use, not by Scoop.

## Notes

- The manifest points at the NSIS installer and installs with `/D`, so the
  application lives in the Scoop directory and is removed with it.
- The installer is not Authenticode-signed. Scoop downloads it directly rather
  than through a browser, which usually avoids the SmartScreen prompt that a
  browser download triggers.
