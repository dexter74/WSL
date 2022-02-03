### Utilisation 
```
wsl.exe [Argument] [Options...] [Ligne de commande]
```


### I. Lancer une commande sur la Distribution
```powershell
wsl.exe
```

### II. Arguments de gestion du sous-système Windows pour Linux :
```powershell
wsl.exe 
 --list
   --online                          Lister les distributions Linux
  
 --install                           Installer d’autres distributions de sous-système Windows pour Linux.
   --distribution, -d                Télécharge et installe une distribution par nom.
   --set-default-version             Définir la version par défaut de WSL. (Dafaut: 2)
   --shutdown                        Met fin immédiatement à toutes les distributions en cours d’exécution et à l’ordinateur virtuel WSL 2 d’utilité légère.
   --status                          Afficher l’état du sous-système Windows pour Linux.
   --update                          Si aucune option n’est spécifiée, le noyau WSL 2 est mis à jour vers la version la plus récente.
     --rollback                      Revenir à la version précédente du noyau WSL 2.
```





```powershell
wsl.exe
 --exec, -e <Ligne de commande>          Exécutez la commande spécifiée sans utiliser le shell Linux par défaut.
  --cd <Répertoire>                      Définit le répertoire spécifié comme répertoire de travail actuel.
  --distribution, -d <Distribution>      Exécutez la distribution spécifiée.
  --user, -u <Nom d’utilisateur>         Éxécute en tant qu’utilisateur spécifié.
  --system                               Lance un Shell pour la distribution du système.
```
