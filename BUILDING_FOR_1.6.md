# Compilation pour RimWorld 1.6

## Situation actuelle
Le dossier `1.6/` ne contient actuellement pas d'Assemblies. RimWorld utilisera automatiquement les DLL de la version 1.5 via son mécanisme de fallback, ce qui devrait fonctionner pour la plupart des fonctionnalités.

## Pour compiler les DLL spécifiquement pour RimWorld 1.6

Si vous souhaitez compiler les DLL pour RimWorld 1.6, voici les étapes :

### Prérequis
- Visual Studio 2019 ou plus récent, OU .NET Framework SDK 4.7.2+
- RimWorld 1.6 installé

### Étapes

1. **Mettre à jour les références dans le fichier .csproj**
   - Ouvrir `Source/MonsterHunterRimworld/MonsterHunterRimworld/MonsterHunterRimworld.csproj`
   - Modifier les chemins des références pour pointer vers RimWorld 1.6 :
     - `Assembly-CSharp.dll` (dans `RimWorld/RimWorldWin64_Data/Managed/`)
     - `UnityEngine.dll` et `UnityEngine.CoreModule.dll` (même dossier)
   - Changer le `OutputPath` de `..\..\..\MHRW\1.5\Assemblies\` vers `..\..\..\1.6\Assemblies\`

2. **Créer le dossier de sortie**
   ```bash
   mkdir -p 1.6/Assemblies
   ```

3. **Compiler**
   - Avec Visual Studio : Ouvrir la solution et compiler en mode Release
   - Avec MSBuild (ligne de commande) :
     ```bash
     msbuild Source/MonsterHunterRimworld/MonsterHunterRimworld.sln /p:Configuration=Release
     ```

4. **Copier la DLL**
   ```bash
   cp Source/MonsterHunterRimworld/MonsterHunterRimworld/bin/Release/MonsterHunterRimworld.dll 1.6/Assemblies/
   ```

### Alternative : Utilisation sans compilation

Le mod devrait fonctionner correctement sans DLL spécifique pour 1.6. RimWorld utilisera automatiquement les DLL de 1.5 qui sont généralement compatibles, sauf si des changements majeurs d'API ont été introduits.

### Changements potentiels nécessaires pour 1.6

Si la compilation échoue ou si des erreurs runtime apparaissent, vous devrez peut-être :
- Mettre à jour les appels d'API qui ont changé entre 1.5 et 1.6
- Vérifier les patches Harmony pour la compatibilité
- Consulter les notes de version de RimWorld 1.6 pour les breaking changes

## Test

Après compilation (ou sans DLL 1.6), testez le mod en :
1. Lançant RimWorld 1.6
2. Activant le mod
3. Créant une nouvelle partie
4. Vérifiant que les colons apparaissent et que le mod fonctionne

## Note importante

Les fichiers `1.6/Assemblies/` et `1.6/Mods/Pawnmorpher/` ont été supprimés car ils contenaient des DLL compilées pour RimWorld 1.5 qui causaient des problèmes de compatibilité avec la version 1.6.
