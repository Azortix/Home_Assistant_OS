<img src="Ressources/HAOS-logo.png" width="25%">

## 🎯 Présentation générale du projet

Ce projet fait partie d’un ensemble de travaux réalisés autour de Proxmox. Il a pour objectif de documenter l’installation de HAOS (Home Assistant Operating System) sur une machine virtuelle Proxmox.

À l’origine, ce projet est destiné à un usage domestique.

### 🔎 Qu'est ce que Home Assistant ?

Home Assistant est une plateforme open-source de domotique qui permet de contrôler, centraliser et automatiser les appareils d’une maison intelligente.  
Compatible avec de nombreux appareils et ecosystèmes. Tout se fait localement, sans dépendance au cloud.

### 🏗️ Type d'infrastructure

**Version de Proxmox utilisée** : 9.1.4  
**Stockage** : LVM-thin local (local-lvm)  
**Adresse IP** : 192.168.1.43  
**Port** : 8123  
**Stratégie de sauvegarde** : Snapshots avant mise à jour. + Backup hebdomadaire, rétention 4 backup.  

Nous entrerons plus en détail sur les caractéristiques de la VM dans Doc.md  

## 🚀 Fonctionnalités mises en place

Par exemple :

Snapshots automatiques

Sauvegardes régulières

## 🔄 Améliorations futures

Un cluster proxmox sera envisagé

L'installation de **Proxmox Backup Server** pour fluidifier le processus de sauvegarde et leurs emplacement

Plus de fonctionnalités

## 📚 Compétences mises en œuvre

Documentation technique en anglais

Virtualisation (Proxmox VE)

Réseau (bridge, IP statique)

Troubleshooting

## ❓Q&A

> - La méthode d'installation via le script est-elle recommandée ?

Oui, l'installation via le script est plus simple, plus dirigé, tout en maintenant la personnalisation possible selon les besoins.

> - Pourquoi importe-t-on une image disque plutôt qu'un ISO

Tout est déjà installé et configuré dans l'image disque (.img, .vdi, .qcow2, etc.). Cela peut éviter les erreurs.  

> - Pourquoi utiliser une VM et pas un conteneur LXC ?

Home Assistant OS est un système complet, pas seulement une application. C’est la méthode officielle recommandée.
