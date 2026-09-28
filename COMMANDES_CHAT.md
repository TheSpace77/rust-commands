# Commandes de chat — serveur Rust

Liste générée depuis les fichiers des plugins présents dans ce dossier. Les commandes sont écrites avec `/`, sauf `!pop` qui est volontairement utilisé tel quel. Certaines commandes sont réservées aux administrateurs ou nécessitent une permission Oxide ; elles restent listées car elles sont bien disponibles dans le chat.

> Les commandes marquées « configurable » utilisent ici leur valeur par défaut dans le code. Elles peuvent différer si leur fichier de configuration a été modifié sur le serveur.

| Commande | Plugin | Description |
|---|---|---|
| `/annonce` | XZBAnnouncer | Ouvre le panneau administrateur de création et gestion des annonces automatiques. |
| `/arena` | ObsidianFFA | Ouvre le menu de l’arène FFA. |
| `/auth` | DiscordAuth | Génère ou affiche le code permettant de lier son compte Rust au bot Discord. |
| `/authenticate` | DiscordAuth | Alias de `/auth`. |
| `/autocode` | ObsidianAutoLock | Ouvre le menu des préférences de verrouillage automatique par code. Configurable. |
| `/basegrenade` | ObsidianBaseGrenade | Ouvre le panneau de gestion des modèles et grenades de base. Configurable. |
| `/bfs [list\|give <événement> [quantité]\|testalarm\|stop]` | BattlefieldSignals | Liste, donne, teste ou arrête les événements Battlefield Signals ; administration uniquement. |
| `/bgrade <0-4\|t <secondes>\|help>` | BGrade | Active l’amélioration automatique des constructions placées : 0 désactive, 1 bois, 2 pierre, 3 métal, 4 blindé ; `t` définit la durée. |
| `/blacklist [additem\|deleteitem] "objet"` | BetterLoot | Affiche ou modifie la liste noire d’objets de BetterLoot. |
| `/bl-backup` | BetterLoot | Crée manuellement une sauvegarde de la configuration BetterLoot. |
| `/bl-restore` | BetterLoot | Restaure une sauvegarde BetterLoot. |
| `/cheatbike` | SuperVelo | Fait apparaître/utiliser le vélo rapide du plugin. |
| `/clean.inv` | InventoryCleaner | Alias de `/clearinv` : nettoie l’inventaire selon les droits accordés. |
| `/clear` | InventoryCleaner | Alias de `/clearinv`. |
| `/clear.inv` | InventoryCleaner | Alias de `/clearinv`. |
| `/clearinv` | InventoryCleaner | Nettoie l’inventaire du joueur ou la cible indiquée, selon les permissions. |
| `/copy <nom> [options]` | CopyPaste | Copie la construction ciblée et l’enregistre sous le nom donné. |
| `/copylist` | CopyPaste | Affiche les constructions sauvegardées par CopyPaste. |
| `/c4` | ObsidianRaid | Sélectionne/obtient le C4 lié au système de raid. |
| `/daynight` | XZBDayNight | Ouvre le menu de préférence d’affichage jour/nuit. Configurable. |
| `/deauth` | DiscordAuth | Dissocie son compte Rust du compte Discord. |
| `/deauthenticate` | DiscordAuth | Alias de `/deauth`. |
| `/debug.invis` | Vanish | Alias historique qui active/désactive Vanish. |
| `/fattack` | SpawnHeli | Rappelle votre hélicoptère d’attaque à proximité. |
| `/fheli` | SpawnHeli | Rappelle votre hélicoptère de transport. |
| `/fmoto` | SpawnHeli | Rappelle votre moto. |
| `/fmotorbike` | SpawnHeli | Alias de `/fmoto`. |
| `/fmini` | SpawnHeli | Rappelle votre minicoptère. |
| `/ffa [join\|leave]` | ObsidianFFA | Ouvre le menu FFA, rejoint l’arène avec `join` ou la quitte avec `leave`. |
| `/ffaadmin ...` | ObsidianFFA | Commandes de gestion de l’arène FFA, notamment du kit ; administration uniquement. |
| `/god [joueur]` | Godmode | Active/désactive l’invulnérabilité pour vous-même ou pour le joueur ciblé. |
| `/godlist` | Godmode | Alias de `/gods`. |
| `/godmode [joueur]` | Godmode | Alias de `/god`. |
| `/gods` | Godmode | Affiche les joueurs actuellement en godmode. |
| `/grade <0-4\|t <secondes>\|help>` | BGrade | Alias de `/bgrade`. |
| `/invis` | Vanish | Alias historique qui active/désactive Vanish. |
| `/inv` | Vanish | Consulte l’inventaire d’un joueur si vous avez la permission d’inspection. |
| `/inv.clean` | InventoryCleaner | Alias de `/clearinv`. |
| `/inv.clear` | InventoryCleaner | Alias de `/clearinv`. |
| `/invclean` | InventoryCleaner | Alias de `/clearinv`. |
| `/invclear` | InventoryCleaner | Alias de `/clearinv`. |
| `/inspect <joueur>` | InventoryViewer | Ouvre l’inventaire du joueur indiqué. |
| `/invspy <joueur>` | Vanish | Alias de `/inv` pour inspecter un inventaire. |
| `/killfeed [test]` | XZBKillFeed | Affiche/masque votre kill feed ; `test` montre un aperçu réservé aux administrateurs. |
| `/kit [nom]` | ObsidianKits | Ouvre le menu des kits ou réclame le kit indiqué. |
| `/looty "identifiant"` | BetterLoot | Télécharge/importe une table Looty par son identifiant. |
| `/mapnoteteleport` | MapNoteTeleport | Téléporte au marqueur de carte sélectionné ou gère cette téléportation selon la configuration. |
| `/menu` | ObsidianWelcome | Ouvre le menu d’accueil et d’informations du serveur. |
| `/mnt` | MapNoteTeleport | Alias de `/mapnoteteleport`. |
| `/myattack` | SpawnHeli | Fait apparaître votre hélicoptère d’attaque. |
| `/myheli` | SpawnHeli | Fait apparaître votre hélicoptère de transport. |
| `/mymini` | SpawnHeli | Fait apparaître votre minicoptère. |
| `/mymoto` | SpawnHeli | Fait apparaître votre moto. |
| `/mymotorbike` | SpawnHeli | Alias de `/mymoto`. |
| `/noattack` | SpawnHeli | Supprime votre hélicoptère d’attaque. |
| `/noheli` | SpawnHeli | Supprime votre hélicoptère de transport. |
| `/nomini` | SpawnHeli | Supprime votre minicoptère. |
| `/nomoto` | SpawnHeli | Supprime votre moto. |
| `/nomotorbike` | SpawnHeli | Alias de `/nomoto`. |
| `/paste <nom> [options]` | CopyPaste | Colle à votre position une construction sauvegardée. |
| `/pasteback` | CopyPaste | Replace la dernière construction collée à son emplacement précédent. |
| `/perms` | PermissionsManager | Ouvre le panneau de gestion des permissions et groupes. |
| `/points` | XZBPointShop | Affiche votre solde de points XZB. |
| `/pop` | Pop | Affiche votre temps de jeu personnel. |
| `/raid` | ObsidianRaid | Ouvre le panneau du système de raid. |
| `/remove` | StaffRemoveTool | Active/désactive l’outil de suppression d’entités visées ; réservé au staff. Configurable. |
| `/rocket` | RocketMode | Active/désactive le tir rapide de roquettes au clic gauche. |
| `/scoreboard` | XZBScoreboard | Ouvre le tableau des scores et statistiques. |
| `/shop [admin]` | XZBPointShop | Ouvre la boutique de points ; `admin` ouvre le mode administration si autorisé. |
| `/skin [show\|get\|purgecache\|add\|remove]` | Skins | Ouvre les skins, récupère l’identifiant du skin d’un objet, vide le cache ou gère les skins (admin). |
| `/skins` | Skins | Alias de `/skin`. |
| `/skins.skin [show\|get\|purgecache\|add\|remove]` | Skins | Commande interne également enregistrée par le plugin ; mêmes actions que `/skin`. |
| `/stacksizecontroller.itemsearch <recherche>` | StackSizeController | Cherche des objets afin de configurer leurs tailles de pile ; administration requise. |
| `/stacksizecontroller.listcategories` | StackSizeController | Liste les catégories d’objets disponibles pour les tailles de pile. |
| `/stacksizecontroller.listcategoryitems <catégorie>` | StackSizeController | Liste les objets d’une catégorie. |
| `/stacksizecontroller.setallstacks <taille>` | StackSizeController | Modifie la taille maximale de pile de tous les objets ; administration requise. |
| `/stacksizecontroller.setstack <objet> <taille>` | StackSizeController | Modifie la taille maximale de pile d’un objet. |
| `/stacksizecontroller.setstackcat <catégorie> <taille>` | StackSizeController | Modifie la taille maximale de pile d’une catégorie. |
| `/stacksizecontroller.vd` | StackSizeController | Génère le fichier des tailles de pile vanilla. |
| `/stats` | XZBScoreboard | Alias de `/scoreboard`. |
| `/supervelo` | SuperVelo | Active ou fait apparaître le vélo rapide. |
| `/top` | XZBScoreboard | Alias de `/scoreboard`. |
| `/uadmin` | UltraAdminPanel | Ouvre le panneau d’administration UltraAdminPanel. Configurable. |
| `/undo` | CopyPaste | Annule le dernier collage CopyPaste lorsque l’option est autorisée. |
| `/unlockbps [all\|refresh\|status\|missing\|joueur]` | UnlockAllBPs | Débloque les blueprints pour vous, tous les connectés, ou un joueur ; administration uniquement. |
| `/vanish [true\|false]` | Vanish | Active/désactive l’invisibilité. Les arguments permettent de forcer l’état. |
| `/vbed ...` | XZBVirtualBeds | Ouvre et pilote le panneau administrateur des lits/points de réapparition virtuels. |
| `/viewinv <joueur>` | InventoryViewer | Ouvre l’inventaire du joueur indiqué. |
| `/viewinventory <joueur>` | InventoryViewer | Alias de `/viewinv`. |
| `/xzbwm` | XZBWatermark | Ouvre le panneau administrateur du watermark. |
| `/zones` | XZBZones | Ouvre le panneau administrateur de gestion des zones. |
| `!pop` | Pop | Envoie le temps de jeu de l’auteur à tous les joueurs ; nécessite la permission du plugin. |

## Remarques

- Les plugins sans commande de chat déclarée ne figurent pas dans cette liste.
- `/autocode`, `/basegrenade`, `/daynight`, `/remove` et `/uadmin` sont configurables : vérifiez les fichiers de configuration du serveur si une commande ne répond pas.
- Les commandes d’administration restent visibles dans le chat, mais le plugin refusera leur exécution sans le niveau d’autorisation ou la permission nécessaire.
