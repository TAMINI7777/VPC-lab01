# VPC-lab01
![Mon image](https://github.com/TAMINI7777/VPC-lab01/blob/main/map%20du%20vpc.webp)
## Introduction
Dans le cadre d'un cloud computing, un VPC (Virtual Private Cloud) s'apparente à un réseau privé virtuel, isolé au sein d'un cloud public. Il offre l'avantage de créer un réseau personnalisé, sécurisé et segmenté, tout en profitant des atouts du cloud computing tels que la flexibilité, l'évolutivité et la tarification à la demande.
### Etape I: Creation de notre VPC
Dans la barre de recherche de la console tape et selectionne VPC.
![](https://github.com/TAMINI7777/VPC-lab01/blob/main/Barre%20de%20recherche.png)

* Cliquer sur Creer VPC pour creer un VPC
* Selectionner VPC Uniquement
* Saisir le nom du VPC (Chez moi c'est **VPC-lab01**
* Saisir la plage d'adresse qu'on veut creer dans le VPC (Chez moi c'est **10.10.0.0/16**)
* Cliquer sur Creer et le tour est joué

  ![](https://github.com/TAMINI7777/VPC-lab01/blob/main/Creer-vpc.png)
  ![](https://github.com/TAMINI7777/VPC-lab01/blob/main/vpc-creer2.png)
  

### Etape I: Creation de notre VPC
* Cliquer sur **Sous-réesaux** en dessus de vpc
* Cliquer sur Creer un sous-réseau
* Selectioner notre notre VPC dans la liste deroulante
* Saisir le nom du sous-réseau
* Selectionner la zone de disponibilité
* Saisir la sous-plage d'adresse
Faites ceci pour les 3 autres sous-reseaux

> [!TIP]
> Pour continuer de créer d'autre sous-reseaux, cliquer sur **Ajouter un nouveau sous-réseau**
##   
![](https://github.com/TAMINI7777/VPC-lab01/blob/main/creer-sous-reseaux.png)
![](https://github.com/TAMINI7777/VPC-lab01/blob/main/sous-reseau2.png)
![](https://github.com/TAMINI7777/VPC-lab01/blob/main/sous-reseau3.png)
![](https://github.com/TAMINI7777/VPC-lab01/blob/main/sous-reseau4.png)
![](https://github.com/TAMINI7777/VPC-lab01/blob/main/subnets-creer.png)

#### Autoriser l'attribution d'adresse automatique
Cela va permettre à ce que chaque instance qui sera creer dans ces sous-réseaux d'avoir une adresse IP publique.
* Selectionner un sous-reseau public puis cliquer sur **action**
* Cliquer sur **Modifier les parametres du sous-reseaux**
* Cocher **Activer l'attribution automatique d'une adresse IPv4 publique**
![](https://github.com/TAMINI7777/VPC-lab01/blob/main/Autoriser%20l'attribution%20automatique00%20.png)
![](https://github.com/TAMINI7777/VPC-lab01/blob/main/Autoriser%20l'attribution%20automatique%20.png)
> [!IMPORTANT]
> Repeter la même chose pour l'autre sous-réseau public

### Etape 3: Creer la passerelle Internet
Toujours sur l'onglet subnets à gauche cliquer sur: **Passerelle Internet**
![](https://github.com/TAMINI7777/VPC-lab01/blob/main/pass-internet.png)
![](https://github.com/TAMINI7777/VPC-lab01/blob/main/nom-IGW.png)

#### Attacher la passerelle à notre VPC
Après la creation de notre passerelle, nous devons attacher notre passerelle internet à notre VPC.
 * Sur la page de notre passerelle créee cliquer sur **action**
 * cliquer sur **Attacher au vpc**
![](https://github.com/TAMINI7777/VPC-lab01/blob/main/pass-internet.png)
![](https://github.com/TAMINI7777/VPC-lab01/blob/main/nom-IGW.png)
![](https://github.com/TAMINI7777/VPC-lab01/blob/main/Attacher_au_vpc.png)
 
