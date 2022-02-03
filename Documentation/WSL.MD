### I. Arguments pour l’exécution des fichiers binaires Linux
``
wsl.exe [Argument] [Options...] [Ligne de commande]
``
```powershell
wsl.exe                              Si aucune ligne de commande n est fournie, wsl.exe démarre l interpréteur de commandes par défaut.
 --exec, -e <Ligne de commande>      Exécutez la commande spécifiée sans utiliser le shell Linux par défaut.
   --cd <Répertoire>                 Définit le répertoire spécifié comme répertoire de travail actuel.
   --distribution, -d <Distribution> Exécutez la distribution spécifiée.
   --user, -u <Nom d utilisateur>    Éxécute en tant qu utilisateur spécifié.
   --system    
```

------------------------------------------------------------------------------------------------------------------
### II. Arguments de gestion du sous-système Windows pour Linux :
```powershell
wsl.exe 
 --list
   --online                          Lister les distributions Linux
  
 --install                           Installer d autres distributions de sous-système Windows pour Linux.
   --distribution, -d                Télécharge et installe une distribution par nom.
   --set-default-version             Définir la version par défaut de WSL. (Dafaut: 2)
   --shutdown                        Met fin immédiatement à toutes les distributions en cours d exécution et à l ordinateur virtuel WSL 2 d utilité légère.
   --status                          Afficher l état du sous-système Windows pour Linux.
   --update                          Si aucune option n est spécifiée, le noyau WSL 2 est mis à jour vers la version la plus récente.
     --rollback                      Revenir à la version précédente du noyau WSL 2.
```

------------------------------------------------------------------------------------------------------------------
### III. Arguments pour la gestion des distributions dans le sous-système Windows pour Linux :
```powershell
wsl.exe
   --export <Distribution> <Nom de fichier>
        Exporte la distribution dans un fichier tar.
        Le nom de fichier peut être-pour la sortie --for standard..

   --import <Distribution> <Emplacement d’installation> <Nom de fichier> [Options]
        Importe le fichier tar spécifié comme nouvelle distribution.
        Le nom de fichier peut être pour une entrée standard.

        Options :
            --version <Version>
                Spécifie la version à utiliser pour la nouvelle distribution.

   --list, -l [Options]
        Répertorie les distributions.

        Options :
            --all
                Lister toutes les distributions, y compris les distributions qui sont
                en cours d’installation ou de désinstallation.

            --quiet, -q
                Liste uniquement les distributions en cours d’exécution.

            --quiet, -q
                Afficher uniquement les noms de distribution.

            --verbose, -v
                Affiche les informations détaillées sur toutes les distributions.

            --online, -o
                Affiche une liste des distributions disponibles pour l’installation avec « wsl --install ».

    --set-default, -s <Distribution>
        Définit la distribution comme valeur par défaut.

    --set-version <Distribution> <Version>
        Modifie la version de la distribution spécifiée

    --terminate, -t <Distribution>
        Termine la distribution spécifiée.

    --unregister <Distribution>
        Annule l’inscription de la distribution et supprime le système de fichiers racine.

    --mount <Disque>
        Attache et monte un disque physique dans toutes les distributions WSL2.

        Options :
            --bare
                Attacher le disque à la WSL2, mais ne pas le monter.

            --type <Type>
                Système de fichiers à utiliser lors du montage d’un disque. S’il n’est pas spécifié, la valeur par défaut est ext4.

            --options <Options>
                Options de montage supplémentaires.

            --partition <Index>
                Index de la partition à monter. Si elle n’est pas spécifiée, la valeur par défaut est le disque entier.

    --unmount [Disque]
        Démonte et détache un disque de toutes les distributions WSL2.
        Démonte et détache tous les disques s’ils sont appelés sans argument.
```














```powershell
wsl.exe
```
