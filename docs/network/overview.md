# Réseau

## Architecture logique

```text
Internet
   │
Routeur
   │
Switch principal
   ├── Management
   ├── Admin
   ├── Users
   ├── Guest
   ├── IoT
   └── Servers
```

## Principes

- Management séparé des utilisateurs.
- IoT isolé.
- Services serveurs sur un VLAN dédié.
- Accès distant via VPN/Tailscale lorsque pertinent.
