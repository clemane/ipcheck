# ipcheck

Toutes vos infos réseau en un coup d'œil, directement dans le terminal.

```
  ╔══════════════════════════════════╗
  ║         ipcheck  v1.0            ║
  ╚══════════════════════════════════╝

  IP publique      203.0.113.42
  IP locale        192.168.1.100
  IPv6             2001:db8::1
  Localisation     Montréal, Quebec, CA
  FAI              AS12345 Mon FAI Inc.
  DNS              127.0.0.53 → 1.1.1.1 (Cloudflare)
  VPN              Non détecté
  ────────────────────────────────────
  Latence          12.3ms (google.com)
```

## Prérequis

- Python 3.10+
- `ping` et `dig` (présents par défaut sur la plupart des distributions Linux)

## Installation

```bash
# Cloner le dépôt
git clone https://github.com/GlobalTi/ipcheck.git
cd ipcheck

# Rendre le script exécutable
chmod +x ipcheck

# Copier dans le PATH
sudo cp ipcheck /usr/local/bin/
```

La commande `ipcheck` est maintenant disponible partout dans le terminal.

## Utilisation

```bash
# Infos réseau de base
ipcheck

# Avec test de débit (download + upload via Cloudflare)
ipcheck --speed
```

## Désinstallation

```bash
sudo rm /usr/local/bin/ipcheck
```
