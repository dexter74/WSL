### Utilisation 
```
```


### I. Arguments pour l’exécution des fichiers binaires Linux

``
wsl.exe [Argument] [Options...] [Ligne de commande]
``


```powershell
wsl.exe                              Si aucune ligne de commande n’est fournie, wsl.exe démarre l’interpréteur de commandes par défaut.
 --exec, -e <Ligne de commande>      Exécutez la commande spécifiée sans utiliser le shell Linux par défaut.
   --cd <Répertoire>                 Définit le répertoire spécifié comme répertoire de travail actuel.
   --distribution, -d <Distribution> Exécutez la distribution spécifiée.
   --user, -u <Nom d’utilisateur>    Éxécute en tant qu’utilisateur spécifié.
   --system    
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


### III. Arguments pour la gestion des distributions dans le sous-système Windows pour Linux :














```powershell
wsl.exe
                           Lance un Shell pour la distribution du système.
```
