Ce hook est configuré pour s'exécuter avant chaque commit dans le dépôt Git. Il permet d'automatiser certaines actions ou de valider certaines conditions avant de réaliser un commit.

Pour activer le hook, suivez les étapes suivantes :
1. Copiez le fichier `pre-commit` dans le répertoire `.git/hooks/` de votre dépôt local.
2. Assurez-vous que le fichier `pre-commit` a les permissions d'exécution appropriées. Si nécessaire, exécutez la commande `chmod +x .git/hooks/pre-commit`.
3. Le hook sera maintenant exécuté automatiquement avant chaque commit.

Ce hook spécifique crée un fichier `commitInfo.txt` dans le répertoire `suivi/` contenant le texte "commit vérifié le <date et heure du jour>" si vous répondez "y" à la question "Sauvegarde de la base dans ce commit (y/[n]) ?" lors de l'exécution du hook.

Si vous ne souhaitez pas exécuter le hook pour un commit particulier, répondez "n" ou appuyez sur Entrée lorsqu'on vous demande de sauvegarder la base de données dans ce commit.

N'hésitez pas à ajuster ou personnaliser le script `pre-commit` selon vos besoins.
