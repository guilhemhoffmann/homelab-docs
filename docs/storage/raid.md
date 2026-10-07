# RAID

## Règle fondamentale

!!! danger "Ne jamais improviser"
    Avant toute opération RAID, identifier précisément les disques, leur ordre, les métadonnées et le filesystem.

## Diagnostic Linux

```bash
lsblk -o NAME,SIZE,MODEL,SERIAL,FSTYPE
cat /proc/mdstat
mdadm --examine --scan
blkid
```

## Opération de récupération

Toujours privilégier une analyse en lecture seule avant toute écriture.
