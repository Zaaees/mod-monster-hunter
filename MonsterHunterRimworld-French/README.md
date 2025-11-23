# Monster Hunter RimWorld - Traduction Française

![Version](https://img.shields.io/badge/version-1.0-blue.svg)
![RimWorld](https://img.shields.io/badge/RimWorld-1.3%20|%201.4%20|%201.5-green.svg)
![Langue](https://img.shields.io/badge/langue-Français-blue.svg)

## 📖 Description

**Monster Hunter RimWorld - French Translation** est un mod de traduction française communautaire pour le mod [Monster Hunter RimWorld](https://steamcommunity.com/sharedfiles/filedetails/?id=XXXXX) créé par AsG_Alligator.

Ce mod traduit l'intégralité du contenu de Monster Hunter RimWorld en français, vous permettant de profiter pleinement de l'expérience de chasse aux monstres dans votre langue.

## ✨ Contenu Traduit

- ✅ **Interface utilisateur** : Tous les menus, boutons et paramètres
- ✅ **Créatures** : Noms et descriptions de tous les monstres (petits monstres, grands monstres, dragons anciens)
- ✅ **Objets** : Nourriture, équipements, ressources et matériaux
- ✅ **Incidents** : Événements d'apparition de monstres et guerres de territoire
- ✅ **Recettes** : Recettes de cuisine et de fabrication
- ✅ **Effets** : Buffs, debuffs et conditions de santé
- ✅ **Paramètres** : Options de configuration du mod

## 📋 Prérequis

### Mods Requis

1. **Monster Hunter RimWorld** (AsGAlligator.MHRW)
   - Ce mod de traduction ne fonctionne **PAS** sans le mod principal
   - Téléchargez-le sur Steam Workshop ou GitHub

2. **Harmony** (brrainz.harmony)
   - Requis par le mod principal
   - [Lien Steam Workshop](https://steamcommunity.com/sharedfiles/filedetails/?id=2009463077)

3. **Vanilla Expanded Framework** (OskarPotocki.VanillaFactionsExpanded.Core)
   - Requis par le mod principal
   - [Lien Steam Workshop](https://steamcommunity.com/sharedfiles/filedetails/?id=1854607105)

### Versions de RimWorld Supportées

- RimWorld 1.3
- RimWorld 1.4
- RimWorld 1.5

## 📥 Installation

### Installation Manuelle

1. **Téléchargez** le fichier ZIP du mod de traduction
2. **Extrayez** le contenu dans votre dossier Mods de RimWorld :
   - **Windows** : `C:\Program Files (x86)\Steam\steamapps\common\RimWorld\Mods\`
   - **Mac** : `~/Library/Application Support/Steam/steamapps/common/RimWorld/Mods/`
   - **Linux** : `~/.steam/steam/steamapps/common/RimWorld/Mods/`

3. **Lancez RimWorld** et activez le mod dans le gestionnaire de mods

### Via Steam Workshop (Si disponible)

1. **Abonnez-vous** au mod sur Steam Workshop
2. **Lancez RimWorld** - le mod sera automatiquement téléchargé
3. **Activez** le mod dans le gestionnaire de mods

## ⚙️ Configuration

### Ordre de Chargement

**IMPORTANT** : L'ordre de chargement des mods est crucial pour le bon fonctionnement de la traduction.

```
1. Harmony
2. Core (RimWorld)
3. Royalty (si installé)
4. Ideology (si installé)
5. Biotech (si installé)
6. Anomaly (si installé)
7. Vanilla Expanded Framework
8. Monster Hunter RimWorld
9. Monster Hunter RimWorld - French Translation  ← CE MOD
```

Le mod de traduction **DOIT** être chargé **APRÈS** Monster Hunter RimWorld.

### Vérification de l'Installation

1. Lancez RimWorld
2. Allez dans **Options** → **Langue**
3. Sélectionnez **Français** si ce n'est pas déjà fait
4. Créez ou chargez une partie
5. Vérifiez que les textes du mod Monster Hunter sont en français

## 🎮 Utilisation

Une fois installé et activé correctement, le mod fonctionne automatiquement. Tous les textes de Monster Hunter RimWorld apparaîtront en français :

- Les **notifications** d'apparition de monstres
- Les **descriptions** des créatures dans l'onglet Animaux
- Les **noms** des objets et nourriture
- Les **paramètres** du mod dans Options → Paramètres des mods

## 🐛 Problèmes Connus

### Textes Toujours en Anglais

**Solution** : Vérifiez que :
- Le mod de traduction est bien **activé**
- Il est placé **APRÈS** Monster Hunter RimWorld dans l'ordre de chargement
- Vous avez **redémarré** RimWorld après l'activation

### Traduction Incomplète

**Solution** :
- Cette traduction est un travail communautaire en cours
- Signalez les textes non traduits dans les Issues GitHub
- Les contributions sont les bienvenues !

### Conflit avec d'Autres Mods de Traduction

**Solution** :
- Désactivez les autres mods de traduction française pour Monster Hunter RimWorld
- Un seul mod de traduction doit être actif à la fois

## 🤝 Contribution

Les contributions sont les bienvenues ! Voici comment vous pouvez aider :

### Signaler des Erreurs

- Ouvrez une **Issue** sur GitHub avec :
  - Le texte en anglais
  - La traduction actuelle (si elle existe)
  - Votre suggestion de traduction
  - Une capture d'écran si possible

### Proposer des Améliorations

- Créez une **Pull Request** avec vos modifications
- Assurez-vous de suivre la structure XML de RimWorld
- Testez vos changements en jeu avant de soumettre

### Structure des Fichiers

```
MonsterHunterRimworld-French/
├── About/
│   └── About.xml                  # Métadonnées du mod
├── Common/
│   └── Languages/
│       └── French/
│           ├── Keyed/             # Traductions avec clés
│           │   ├── Incidents.xml
│           │   └── UI.xml
│           └── DefInjected/       # Traductions injectées
│               ├── ThingDef/
│               ├── HediffDef/
│               ├── RecipeDef/
│               └── ...
└── README.md
```

## 📝 Notes de Version

### Version 1.0 (2025-11-23)

- ✅ Traduction initiale complète
- ✅ Support RimWorld 1.3, 1.4, 1.5
- ✅ Traduction de l'interface utilisateur
- ✅ Traduction des incidents de monstres
- ✅ Traduction de la nourriture et des objets
- ✅ Traduction des effets et buffs

## 📜 Licence

Ce mod de traduction est distribué sous licence MIT (ou équivalent).

Le contenu traduit appartient aux auteurs originaux du mod Monster Hunter RimWorld.

## 🙏 Crédits

### Mod Original
- **AsG_Alligator** - Créateur de Monster Hunter RimWorld

### Traduction Française
- **Communauté RimWorld Francophone**
- Contributeurs : [Voir la liste des contributeurs]

### Remerciements Spéciaux
- La communauté RimWorld pour son soutien
- Les testeurs bénévoles
- Ludeon Studios pour RimWorld

## 🔗 Liens Utiles

- **Monster Hunter RimWorld (Original)** : [Steam Workshop](https://steamcommunity.com/)
- **Discord RimWorld FR** : [Rejoignez-nous](https://discord.gg/rimworld-fr)
- **Forum RimWorld** : [Section Mods](https://ludeon.com/forums/)
- **GitHub** : [Repository](https://github.com/)

## 💬 Support

Pour toute question ou problème :

1. Consultez la section **Problèmes Connus** ci-dessus
2. Recherchez dans les **Issues** GitHub si le problème a déjà été signalé
3. Créez une **nouvelle Issue** avec tous les détails
4. Rejoignez le **Discord RimWorld FR** pour obtenir de l'aide

---

**Bon jeu et bonne chasse sur la Bordure !** 🎯🐉

*Ce mod n'est pas affilié à Capcom ou à la franchise Monster Hunter.*
