# Remplacer un disque

!!! danger "Ne rien écrire avant identification"
    Ne pas formater, initialiser, créer un RAID ou monter en écriture avant d'avoir identifié précisément les disques et le filesystem.

## 1. Arrêter la machine

```bash
shutdown -h now
```

## 2. Identifier les disques

```bash
lsblk -o NAME,SIZE,MODEL,SERIAL,FSTYPE
```

## 3. Identifier le RAID

```bash
cat /proc/mdstat
mdadm --examine --scan
```

## 4. Identifier le filesystem

```bash
blkid
```

## 5. Monter en lecture seule si nécessaire

```bash
mount -o ro /dev/sdX1 /mnt/recovery
```

## Validation

- [ ] disque identifié
- [ ] numéro de série confirmé
- [ ] RAID identifié
- [ ] filesystem identifié
- [ ] données accessibles
- [ ] sauvegarde disponible
