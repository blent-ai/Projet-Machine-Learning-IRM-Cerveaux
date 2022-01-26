<div align="center">
  <a href="https://blent.ai">
    <img src="https://blent-static-media.s3.eu-west-3.amazonaws.com/images/logo/logo_blent_300x.png" alt="Logo Blent.ai" width="200" />
  </a>

  <h2 align="center">Détection de tumeurs sur des images IRM de cerveaux</h2>

  <p align="center">
    Projet Computer Vision - <a href="https://blent.ai">Blent.ai</a>
    <br />
    <a href="https://blent.ai/app/projects" target="_blank"><strong>Explorer tous les projets »</strong></a>
</div>

<div align="center"><img src="https://cdn.static-media.blent.ai/images/projects/badge_mri.svg" width="120" alt="Badge du projet" /></div>

## À propos du projet

Une entreprise construit des appareils IRM, dont celles permettant d'effectuer des imageries de cerveaux. Elle souhaite délivrer un logiciel capable d'identifier automatiquement la présence de tumeurs ou de structures cancéreuses dans les images IRM, pour assister le diagnostic du médecin.

<div align="center"><img src="https://blent-learning-user-ressources.s3.eu-west-3.amazonaws.com/projects/60fb61/BraTS19_2013_11_1_flair_3d_2d.gif" alt="Vue animée BraTS" /></div>

Pour celle, elle cherche à utiliser des algorithmes de Computer Vision efficaces et adaptés pour la segmentation d'images.

L'objectif est de construire un **algorithme capable de détecter et segmenter la présence d'une tumeur** ou d'une structure cancéreuse sur une succession d'images en coupe (selon l'axe Z de la hauteur) d'un patient. Pour cela, le jeu de données BraTS 2019 contient de nombreuses images IRM à plusieurs coupes et contrastes différents de patients atteints d'une tumeur, ainsi que des segmentations de ces tumeurs réalisées à la main.

> TODO : Compléter cette partie pour apporter plus d'informations sur le contexte du projet.

## Étapes du projet

- [ ] Charger et redimensionner les images FLAIR en taille fixe 240 x 240 x 144
- [ ] Construire et entraîner un U-NET sur les images FLAIR à l'aide des segmentations
- [ ] Évaluer les performances du modèle pour satisfaire les contraintes du projet
- [ ] Publier le code source et les résultats sur GitHub

La description des étapes est disponible sur la page associée au projet.

> TODO : Cocher les cases au fur et à mesure de l'avancement.

## Résultats

| Taille du train |      Précision      |     Sensibilité     |
|:---------------:|:-------------------:|:-------------------:|
|        1k       | 00.00% ± 00.00% | 00.00% ± 00.00% |
|       10k       | 00.00% ± 00.00% | 00.00% ± 00.00% |
|       100k      | 00.00% ± 00.00% | 00.00% ± 00.00% |

> TODO : Il est possible d'ajouter des graphes pour apporter plus d'indications sur les résultats.

## Structure du projet

Le dépôt Git contient les éléments suivantes.

- `notebooks/` contient les Notebooks Jupyter du projet.
- `src/` contient les codes sources Python principaux du projet.
- `data/` contient les données du projet.
- `config/` contient les configurations et paramètres du projet.
- `LICENSE.txt` : licence du projet.
- `requirements.txt` : liste des dépendances Python nécessaires.
- `README.md` : fichier d'accueil.

## Premiers pas

Les instructions suivantes permettent de d'exécuter le projet sur son PC.

### Pré-requis

Le projet nécessite Python 3 d'installé sur le système.

> TODO : Ne pas hésiter à compléter/adapter cette partie en fonction des dépendances logicielles.

### Installation

1. Cloner le projet Git.
	```
	git clone https://github.com/UserName/ProjectName.git
	```
2. Installer les dépendances du fichier `requirements.txt` dans un environnement virtuel.
	**Linux / MacOS**
	```
	python3 -m venv venv/
	source venv/bin/activate
	pip install -r requirements.txt
	```
	**Windows**
	```
	python3 -m venv venv/
	C:\<chemin_dossir>\venv\Scripts\activate.bat
	pip install -r requirements.txt
	```

> TODO :
> - Remplir le fichier `requirements.txt` pour y ajouter les dépendances (NiBabel, NiLearn, TensorFlow, etc).
> - Compléter la procédure d'installation pour l'adapter en fonction des besoins (GPU, librairies externes).

### Démarrage

> TODO : Expliquer en quelques lignes et avec des exemples de ligne de commande comment l'utilisateur peut entraîner ou utiliser lui-même le modèle. 

## Licence

*Ce projet est proposé par <a href="https://blent.ai">Blent.ai</a>. Les données utilisées pour ce projet peuvent être soumises à des droits d'auteur et de propriété intellectuelle. Blent.ai ne peut être responsable des utilisations faites des données utilisées dans le cadre de ce projet.*

> TODO : Ajouter les licences supplémentaires au projet (autres données, outils propriétaires, etc).

## Citations

[1]  [B. H. Menze, A. Jakab, S. Bauer, J. Kalpathy-Cramer, K. Farahani, J. Kirby, et al. "The Multimodal Brain Tumor Image Segmentation Benchmark (BRATS)", IEEE Transactions on Medical Imaging 34(10), 1993-2024 (2015) DOI: 10.1109/TMI.2014.2377694](https://www.ncbi.nlm.nih.gov/pubmed/25494501)

[2]  [S. Bakas, H. Akbari, A. Sotiras, M. Bilello, M. Rozycki, J.S. Kirby, et al., "Advancing The Cancer Genome Atlas glioma MRI collections with expert segmentation labels and radiomic features", Nature Scientific Data, 4:170117 (2017) DOI: 10.1038/sdata.2017.117](https://www.ncbi.nlm.nih.gov/pubmed/28872634)

[3]  [S. Bakas, M. Reyes, A. Jakab, S. Bauer, M. Rempfler, A. Crimi, et al., "Identifying the Best Machine Learning Algorithms for Brain Tumor Segmentation, Progression Assessment, and Overall Survival Prediction in the BRATS Challenge", arXiv preprint arXiv:1811.02629 (2018)](https://arxiv.org/abs/1811.02629)  

[4]  [S. Bakas, H. Akbari, A. Sotiras, M. Bilello, M. Rozycki, J. Kirby, et al., "Segmentation Labels and Radiomic Features for the Pre-operative Scans of the TCGA-GBM collection", The Cancer Imaging Archive, 2017. DOI: 10.7937/K9/TCIA.2017.KLXWJJ1Q](https://doi.org/10.7937/K9/TCIA.2017.KLXWJJ1Q)

[5]  [S. Bakas, H. Akbari, A. Sotiras, M. Bilello, M. Rozycki, J. Kirby, et al.,](https://doi.org/10.7937/K9/TCIA.2017.KLXWJJ1Q) ["Segmentation Labels and Radiomic Features for the Pre-operative Scans of the TCGA-LGG collection", The Cancer Imaging Archive, 2017. DOI: 10.7937/K9/TCIA.2017.GJQ7R0EF](https://doi.org/10.7937/K9/TCIA.2017.GJQ7R0EF)
