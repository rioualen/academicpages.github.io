---
title: "Assemblée Générale France Génomique [FR]"
collection: talks
type: "Poster"
permalink: /talks/2015-11-25_FranceGeno_poster
venue: "Novotel Paris 13 Porte d'Italie, Le Kremlin-Bicêtre"
date: 2015-11-25
location: "Paris, France"
---

[France Génomique](https://www.france-genomique.org/)

Développement de workflows pour l'analyse ChIP-seq sous Snakemake et déploiement d'une machine virtuelle sur le cloud IFB.


Le workpackage 2.6 de France Génomique s'articule autour de la régulation de l'expression des gènes, et s'inscrit dans une volonté d'encourager les efforts collectifs dans l'évalutation des outils existants, le développement de nouveaux outils et pipelines ainsi que la maintenance des ressources et leur mise à disposition pour le public. Ceci doit permettre, à terme, d'éviter la duplication des travaux et de capitaliser les connaissances et bonnes pratiques acquises ce faisant. 

--

Snakemake est une librairie basée sur le langage python, permettant de construire des workflows et utilisant la logique des règles et des cibles de GNU make. Elle permet de chaîner des opérations, de les paralléliser ou encore de réaliser du benchmarking, et ceci en utilisant les langages python, R ou shell.


Dans le cadre du WP2.6, nous avons développé un catalogue de règles collaboratif permettant de construire, brique par brique, des workflows ChIP-seq personnalisés afin de répondre à différentes questions biologiques. Celui-ci inclut des opérations allant du contrôle qualité au peak-calling, en passant par différents algorithmes de mapping. Une recherche de motifs peut également être effectuée via la suite logicielle RSAT implémentée. Le workflow a d'ores et déjà été appliqué à des cas d'étude variés tels que bactéries, levures ou drosophile.


Ce travail collaboratif a donné lieu à un projet git hébergé le service SourceSup/Renater, et comprend également un catalogue de règles adaptées au RNA-seq, avec l'ojectif de permettre des analyses intégrées.
Un manuel est en cours de rédaction pour faciliter l'installation et l'utilisation de Snakemake. Ceci permettra également de favoriser l'analyse en production et le benchmarking d'outils de peak-calling. Enfin une machine virtuelle, actuellement développée sur le cloud de l'Institut Français de Bioinformatique (IFB), permettra dès son déploiement l'usage des workflows par tout utilisateur en garantissant leur portabilité.

Poster available [here](http://rioualen.github.io/files/2015-11-25_FranceGeno_poster.pdf)


