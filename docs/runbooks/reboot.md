# Redémarrage

## Avant

- [ ] Identifier le service concerné.
- [ ] Vérifier les dépendances.
- [ ] Vérifier qu'aucune opération critique n'est en cours.

## Procédure

```bash
systemctl status SERVICE
systemctl restart SERVICE
systemctl status SERVICE
```

## Validation

- [ ] Service actif
- [ ] URL accessible
- [ ] Logs normaux
- [ ] Client fonctionnel
