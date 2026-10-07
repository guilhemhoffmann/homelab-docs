# Homelab Documentation

Documentation MkDocs du homelab et du studio.

## Démarrage local

```bash
python -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
mkdocs serve
```

Puis ouvrir :

`http://127.0.0.1:8000`

## Android / Termux

```bash
cd ~/homelab-docs
source ~/venvs/mkdocs/bin/activate
git pull
mkdocs serve
```

## Principe

La documentation décrit **l'état réel du système**, pas l'état souhaité.
