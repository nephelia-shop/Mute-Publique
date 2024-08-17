# NepheliaShop Mute

## Description

Ce plugin permet de muter et unmute des joueurs sur votre serveur.

## Commandes

| Commande     | Description            | Utilisation                                               | Permission                              |
|--------------|------------------------|-----------------------------------------------------------|-----------------------------------------|
| **mute**     | Mute un joueur         | /mute <player> <jour> <heure> <minute> <seconde> <raison> | nepheliashop.permissions.mute           |
| **unmute**   | Unmute un joueur       | /unmute <player>                                          | nepheliashop.permissions.unmute         |
| **mutelist** | Liste des joueurs mute | /mutelist                                                 | nepheliashop.permissions.mutelist       |

## Messages Configurables

Les messages affichés par le plugin sont entièrement configurables dans le fichier de configuration *(`config.yml`)*. Voici les différents messages disponibles :

```yaml
messages:
  muted: "§cVous êtes mute pendant §6{DAYS} jour(s), {HEURES} heure(s), {MINUTES} minute(s), {SECONDES} seconde(s) §cpar §6{STAFF} §cpour §6{RAISON}"
  target-muted: "§aVous avez bien mute {TARGET} pendant {DAYS} jour(s), {HEURES} heure(s), {MINUTES} minute(s), {SECONDES} seconde(s) pour {RAISON}"
  target-already-mute: "§c{TARGET} est déjà mute"
  target-unmuted: "§a{TARGET} a été unmute"
  target-not-mute: "§c{TARGET} n'est pas mute"
  mutelist:
    header: "§7- §fListe des joueurs mute :\n"
    mute: "§7- §6{TARGET} §fpour §6{RAISON} §fpar §6{STAFF} §fpendant §6{DAYS} jour(s), {HEURES} heure(s), {MINUTES} minute(s), {SECONDES} seconde(s)\n"
```

*Les données sont stockées dans une base de données SQLite. Le plugin utilise la bibliothèque [libasynql](https://github.com/poggit/libasynql) pour gérer les opérations de base de données de manière asynchrone, ce qui permet d'assurer de bonnes performances sans bloquer le thread principal du serveur.*

## Fonctionnalités

- ✅ Mute et Unmute des joueurs
- ✅ Liste des joueurs mute
- ✅ Messages configurables
- ✅ Stockage des données avec SQLite
- ❌ Await System pour plus d'optimisation ( [await-std](https://github.com/SOF3/await-std/tree/master/src/SOFe/AwaitStd) )
- ❌ Support de la base de données JSON
- ❌ Support de la base de données MySQL

## Support et Suggestions

Pour toute demande de support ou suggestion, veuillez rejoindre notre [Discord](https://discord.gg/pocketmine).
