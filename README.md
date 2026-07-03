# Meetup Octo (OCaml-Toulouse)

## Événements

### Quand aura lieu le prochain meetup ?

Nous postons les annonces sur la mailing list [ocaml-toulouse@groupes.renater.fr](https://groupes.renater.fr/sympa/info/ocaml-toulouse), abonnez-vous !

### Où ont lieu les meetups ?

TBD

## Exposés précédents

#### 11 octobre 2022
  * Erik Martin Dorel, de l'IRIT, qui présentera la plateforme d'apprentissage [LearnOCaml](https://ocaml-sf.org/learn-ocaml/), son histoire et ses fonctionalités et développements récents
    * Le logiciel learn-ocaml est à la fois une plateforme d'apprentissage de la programmation, dotée de fonctionnalités d'auto-évaluation très expressives, personnalisables par l'enseignant, et un projet logiciel distribué sous licence libre qui évolue régulièrement. Après un résumé de l'historique du développement de learn-ocaml, nous survolerons ses principales fonctionnalités (± récentes et ± connues) avant de conclure par une ou plusieurs démos, si le temps le permet.
    * [slides](https://www.irit.fr/~Erik.Martin-Dorel/exposes/2022-W41_learn-ocaml_meetup.pdf)
  * David Declerck, d'OCamlPro, qui présentera la bibliothèque [OCaml Canvas](https://github.com/ocamlpro/ocaml-canvas), permettant un rendu vectoriel multi plateforme

#### 17 janvier 2023
  * Aurélie Hurault - Toulouse INP - IRIT : Retour d'utilisation d'OCaml pour la partie pratique d'un cours de compilation (Niveau M1)
    * Dans le cadre du cours de "Traduction des Langages" donnés aux élèves ingénieurs de l'ENSEEIHT, ils doivent développer un compilateur pour un petit langage impératif. Deux versions précédentes de ce cours utilisaient des technologiques du monde Java (outil maison puis XText). Aujourd'hui, le compilateur est réalisé en OCaml en utilisant notamment Menhir pour l'analyse lexicale et syntaxique, et ppx_inline_test pour les jeux de tests. Les avantages et les limites de cette version seront discutés. 
  * Anthony Scemama - CNRS - LCPQ : Utilisation d'OCaml dans le contexte du calcul haute performance (HPC)
    * QMC=Chem est un code de calcul HPC qui utilise des méthodes Monte Carlo quantique (QMC) pour la chimie. La particularité des méthodes de Monte Carlo est qu'elles sont massivement parallélisables, mais aussi qu'elles permettent d'implémenter la tolérance aux pannes. Dans le contexte du HPC, le standard de communication est la bibliothèque MPI, qui est intolérante aux pannes, et qui n'était donc pas adapté à mes besoins.
J'ai donc développé un code en OCaml pour permettre à des processus Fortran mono-coeur de communiquer avec un serveur via un échange de messages typés, permettant au code de tourner en parallèle. Aujourd'hui, ce code tourne de manière routinière avec plus de 10000 coeurs et avec une efficacité parallèle presque idéale. J'ai utilisé la même approche pour paralléliser un code de chimie quantique utilisant des méthodes déterministes (Quantum Package), et cette approche m'a permis de faire communiquer le supercalculateur du meso-centre CALMIP (Toulouse) et celui du CRIANN (Rouen) pour la recherche de valeurs propres de grandes matrices avec une excellente efficacité parallèle.
Pourquoi OCaml? Parce qu'avec un autre langage je n'aurais pas été capable d'écrire un code correct...

#### 27 juin 2023
  * Mathieu Barbin : un langage de description pour la programmation de circuits numériques synchrones
    * Il était une fois, lorsque j'étais étudiant, j’ai suivi un cours d’architecture des ordinateurs... Le projet du cours consistait à implémenter un simulateur de circuits digitaux synchrones avec pour objectif final la conception d’un microprocesseur capable de piloter un calendrier digital. Avec mon binôme, nous avons implémenté en OCaml un langage de description de circuits inspiré du langage 2Z utilisé dans les polycopiés du cours, et nous avons développé notre microprocesseur “visa” dans ce langage.
Début 2023 (soit 15 ans plus tard), j’ai retrouvé ce projet dans mes archives, et j’ai eu envie de lui donner une seconde vie. J’ai réécrit certaines parties en m’appuyant sur des fonctionnalités, bibliothèques et outils apparus dans l'écosystème OCaml depuis la version initiale, comme les gadt, ppx, opam, dune, ocamlformat, menhir, core, tsdl & bogue pour les parties graphiques, mdx & docusaurus pour la doc, etc.
Mon talk portera sur ce projet. Tout d’abord j’introduirai le langage, puis je présenterai différents circuits en démo, dont le microprocesseur visa. 
  * Anthony Scemama, du LCPQ : la librairie QCaml, une bilbiothèque d'algorithmes pour la chimique quantique
    * QCaml est une bibliothèque d'algorithmes pour la chimie quantique. Les langages les plus utilisés en chimie quantique sont Fortran, C et C++ car les calculs sont souvent très coûteux. On voit apparaître depuis une dizaine d'années des codes en Python où la performance est réduite mais où l'effort de développement est réduit. OCaml paraît être un meilleur choix que Python, car il permet de générer du code performant et plus sûr.
Je montrerai comment OCaml a facilité l'implémentation d'algorithmes difficiles à programmer en Fortran. Je montrerai aussi comment QCaml peut être utilisé interactivement à l'aide de Notebooks Jupyter ou org-mode, pour développer de nouvelles méthodes de calcul, ou bien en mode compilé pour réaliser des calculs de production.


## Contact

Les organisateurs du meetup sont:

- Raja Boujbel ([email](raja.boujbel@ocamlpro.com))
- [Erik Martin-Dorel](https://www.irit.fr/~Erik.Martin-Dorel/) ([email](erik@martin-dorel.org))
- [Basile Pesin](https://vertmo.org/) ([email](basile.pesin@vertmo.org))
- [Loïc Sylvestre](https://www.loicsylvestre.com/) ([email](loïc.sylvestre@utoulouse.fr))
