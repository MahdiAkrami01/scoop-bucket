# Scoop Bucket

<!-- Uncomment the following line after replacing placeholders -->
[![Tests](https://github.com/MahdiAkrami01/scoop-bucket/actions/workflows/ci.yml/badge.svg)](https://github.com/MahdiAkrami01/scoop-bucket/actions/workflows/ci.yml) [![Excavator](https://github.com/MahdiAkrami01/scoop-bucket/actions/workflows/excavator.yml/badge.svg)](https://github.com/MahdiAkrami01/scoop-bucket/actions/workflows/excavator.yml)

Custom Bucket for [Scoop](https://scoop.sh), the Windows command-line installer.

## ✅ How to add this bucket?

```pwsh
scoop bucket add akrami https://github.com/MahdiAkrami01/scoop-bucket
```

## 🗑 How to remove this bucket?

```pwsh
scoop bucket rm akrami
```

## 🚀 How to fix the Scoop slow download problem?

```pwsh
scoop install aria2
```

```pwsh
scoop config aria2-warning-enabled false
scoop config aria2-split 16
scoop config aria2-max-connection-per-server 16
```

## 📱 Avaiable apps

- Thorium Browser ([install](docs/thorium.md))
- PHP Multiple Versions ([install](docs/php.md))
