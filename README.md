# vagrant-ubuntu
vagrant image ubuntu

1. Exportez la machine virtuelle de votre PC actuel en utilisant la commande suivante dans un terminal :

```powershell
vagrant package --output nom_machine.box
# Remplacez "nom_machine" par le nom de votre machine virtuelle. 
# Cette commande va créer un fichier "nom_machine.box" qui contient tous les 
# fichiers nécessaires pour la machine virtuelle.
```

1. Copiez le fichier "nom_machine.box" sur votre autre PC, soit via un disque dur externe ou une clé USB, soit via un transfert de fichier en réseau.
2. Importez la machine virtuelle sur votre autre PC en utilisant la commande suivante dans un terminal :

```powershell
vagrant box add nom_machine nom_machine.box
# Cette commande va ajouter la machine virtuelle à votre bibliothèque Vagrant.
```

1. Créez un dossier pour votre nouvelle machine virtuelle et initialisez-le avec Vagrant en utilisant la commande suivante dans un terminal :

```powershell
mkdir nouveau_dossier # Remplacez "nouveau_dossier" par le nom du dossier que vous voulez créer pour votre nouvelle machine virtuelle.
cd nouveau_dossier
vagrant init nom_machine
vagrant up
```
