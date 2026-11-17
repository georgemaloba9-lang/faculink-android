# FACULINK Android

Application Android native qui ouvre le site FACULINK dans une WebView.

- Site : https://faculink.xo.je/
- Application ID : com.orbiba.faculink
- Build APK de test : GitHub Actions > Build FACULINK APK > Artifacts

## Générer l'APK

1. Téléverser tout le contenu de cette archive à la racine du dépôt GitHub `faculink-android`.
2. Ouvrir l'onglet Actions.
3. Sélectionner `Build FACULINK APK`.
4. Cliquer sur `Run workflow`, puis confirmer.
5. À la fin, télécharger l'artefact `FACULINK-debug-apk`.

L'APK généré est un APK de test signé avec la clé de débogage de la compilation. Pour distribuer des mises à jour stables, il faudra ensuite configurer une clé de signature release conservée dans les secrets GitHub.

## Icône

L'icône incluse est provisoire. Remplacer `app/src/main/res/drawable/ic_launcher.xml` par les ressources du logo FACULINK avant la version finale.

## Notes

Cette version utilise Android WebView, pas Trusted Web Activity. Elle ne nécessite donc ni manifeste PWA ni fichier Digital Asset Links. Une connexion Internet est nécessaire.
