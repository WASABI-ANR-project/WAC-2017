class: center, middle, vertigo

# WASABI

##a two million song database project with audio and cultural metadata <br> plus WebAudio enhanced client applications

<hr>

Michel Buffa - INRIA / Wimmics<br>
Guillaume Pellerin - IRCAM<br>

### WAC 2017 - 22/08/2017 - QMUL
<img src="img/jim_horiz_blanc_1.png" height="100px" />

---
class: vertigo

#WASABI project

##Web Audio and SemAntic in the Browser for Indexation

- 42 months from 2016 Q4 to april 2020 Q2
- 750 k€ project granted by the french Research National Agency

## Partners

- INRIA (I3S)
- IRCAM (MIR + Musicology + Library)
- Deezer R&D
- Radio France Library
- Parisson

---
class: vertigo

#WASABI

##Objectives

- Propose some new methodologies to index music in the web and audio context
- Link semantics (linked metadata) + acoustics (MIR data) + machine learning
- Develop and publish some open source web services through original APIs

##Use cases

- augmented web music browsing
- data journalism
- music composing through big data
- plagiarism or influence detection

*wasabi website link*

---
class: vertigo, tight

#Semantic web

--

.pull-left[
- Documentations technico-musicales de référence sur des œuvres réalisées à l’Ircam ou en connexion directe avec cet institut
- Analyses multimédia
- Mise en relation avec l’ensemble des bases Ircam : Brahms, Sidney
- Objectifs

    - Faire connaître les œuvres à un public plus large
    - Montrer la relation entre l’idée musicale et les technologies utilisées
    - Identifier les nouveaux éléments du vocabulaire musicale qui émergent à travers ces œuvres
    - Offrir un support d’information aux interprètes
]

.pull-right[
.right[![image](img/brahms_home.png)]
]

---
class: vertigo, tight

.pull-left[

# Exemple de description

http://brahms.ircam.fr/analyses/metallics/


- Description

    - du principe de l’harmoniseur
    - du rôle de l’harmoniseur dans l’analyse de Metallics de Yan Maresz, notamment à l’événement 44 de la partition

- Mélange de texte, d’images fixes et de sons
]

.pull-right[
.right[![image-85](img/mettalics.png)]
]

---
class: vertigo, tight

#TimeSide

##audio processing framework for the web

https://github.com/Parisson/TimeSide

##Features

- Do asynchronous and fast audio processing with Python,
- Decode audio frames from any audio or video media format into numpy arrays,
- Analyze audio content with some state-of-the-art audio feature extraction libraries like Aubio, Yaafe, VAMP and Essentia as well as some pure python processors
- Visualize sounds with various fancy waveforms, spectrograms and other cool graphers,
- Transcode audio data in various media formats and stream them through web apps,
- Serialize feature analysis data through various portable formats,
- Playback and interact on demand through a smart high-level HTML5 extensible player,
- Index, tag and annotate audio archives with semantic metadata (see Telemeta which embed TimeSide).
- Deploy and scale your own audio processing engine through any infrastructure


---
class: vertigo, tight

#TimeSide

##audio processing framework for the web

https://github.com/Parisson/TimeSide

##Use cases

- Scaled audio computing (filtering, machine learning, etc)
- Web audio visualization
- Audio process prototyping
- Realtime and on-demand transcoding and streaming over the web
- Automatic segmentation and labelling synchronized with audio events
- Audio analysis web service

---
class: vertigo, tight

#TimeSide - examples

.pull-left[

##Telemeta

###Collaborative multimedia asset management system

https://github.com/Parisson/Telemeta

]

.pull-right[
.right[![image-60](img/telemeta.png)]
]

---
class: vertigo, tight

# Exemples de simulations en sciences physiques

.pull-left[
## Physion : accès au code et écriture de scripts Javascript

http://physion.net/
]

.pull-right[
.right[![image-85](img/physion.png)]
]


---
class: vertigo

# Manipulation de contenus sonores

.pull-left[
## Projet TaCEM, Université de Huddersfield, équipe de Michael Clarke

- Analyses interactives fondées sur l’écoute de sons extraits
- Exemple de Wind Chimes de Denis Smalley
- Zoom d’écoute : sélection et filtrage d’un son pré-défini
- Parcours d’une taxonomie de fragments sonores significatifs dans l’œuvre
- Variation des vitesses de lecture des fragments / celles choisies par le compositeur
- Tutorial 2 / Portraits polychromes

]

.pull-right[
.right[![image-85](img/tacem.png)]
]



---
class: vertigo

# Manipulations musicales génératives

.pull-left[
## JavaScript Systems Music

Reconstruction d’œuvres de Steve Reich et Brian Eno

http://teropa.info/blog/2016/07/28/javascript-systems-music.html

]

.pull-right[
.right[![image-85](img/reich.png)]
]



---
class: vertigo

.pull-left[
# Web Audio Resources

a list of curated resources related to the Web audio API :

https://github.com/alemangui/web-audio-resources

]

.pull-right[
![image-85](img/web-audio-resources.jpg)
]

---
class: vertigo

.pull-left[
# Pizzicato

A web audio Javascript library

https://alemangui.github.io/pizzicato/
]

.pull-right[
.center[![image-85](https://alemangui.github.io/pizzicato//img/logo.svg)]

]

---
class: center, middle, vertigo

# Vers un harmoniseur interactif Web Audio


---
class: vertigo, tight

.pull-left[

# Manipulation ⇔ écoute

## Prise en main d’un traitement sonore : l’harmoniseur

- Enrichissement de l’analyse de En Echo de Manoury (1993)
- Voix et temps réel
- Analyse en cours de finalisation
- Point de départ : version 2010 du patch Max de l’œuvre
- Sous-patch d’harmoniseur isolé
- 4 paramètres de pilotage : étendue de la transposition (en midicents), largeur de la fenêtre (de 0 à 127), délai temporel (en millisecondes), niveau de sortie
- Pas de zoom dans le son ou de reconstruction générative ici

]

.pull-right[
.right[![image-60](img/en_echo.png)]
]


---
class: vertigo, tight

.pull-left[
# Interface de manipulation

### Valeurs par défaut issues d’un état particulier dans l’œuvre jugé intéressant

- 4ème section “Mea Lux”, Chiffres 19 et 20
- Épaississement de la voix par les 4 harmonizers (transpositions micro-tonales)

### Réduction de l’espace des paramètres pour ouvrir à la manipulation par le lecteur

- Au départ 16 paramètres (4 par harmonizer)
    - 6 paramètres
    - 4 transpositions entre -100 et +100 midi-cents
]

.pull-right[
.right[![image-85](img/mea_lux.png)]
.right[![image-85](img/harmo_pd.png)]
]




---
class: vertigo, tight

.pull-left[
# Demonstration Harmonizeur Web Audio

[link](https://ircam-web.github.io/analyses-webaudio-effects/EnEchoHarmonizer/enEcho4harmonizer.html)

[code](https://github.com/Ircam-Web/analyses-webaudio-effects)

```
//--------------------------------------------------------------------------------------//
// HARMONIZER FAUST CODE
// Translated from the Max harmonizers used in En Echo by Philippe Manoury
// Author : Alain Bonardi
// January 2017
//--------------------------------------------------------------------------------------//
import("stdfaust.lib");

//--------------------------------------------------------------------------------------//
// DEFINITION OF CONTROLS
//--------------------------------------------------------------------------------------//
//transpositions in midicents between -2400 and 2400//
//initialized with Manoury's values in En Echo in the 4th piece Mea Lux at events 19 and 20
//the ambitus is -100 to 100 (one half-tone under, one half-tone above)
transposition1 = hslider("transposition1", 30, -100, 100, 1);
transposition2 = hslider("transposition2", 15, -100, 100, 1);
transposition3 = hslider("transposition3", -15, -100, 100, 1);
transposition4 = hslider("transposition4", -30, -100, 100, 1);

//harmonizer window between 0 and 127//
//initialized with Manoury's value of 50 in En Echo in the 4th piece Mea Lux at events 19 and 20//
//with the lineDrive the actual value is 19.7032
```
]

.pull-right[
<!--
<iframe id="frame" src="https://ircam-web.github.io/analyses-webaudio-effects/EnEchoHarmonizer/enEcho4harmonizer.html" scrolling="auto" frameborder="0" allowfullscreen="" width="100%">
-->
]

???
Latence


---
class: vertigo

# Faust ?

### un langage de programmation fonctionnel dédié aux traitements audio temps-réel

- open source (GRAME)
- compilation vers de très nombreux environnements
- online compiler : http://faust.grame.fr/onlinecompiler/
- playground : http://faust.grame.fr/faustplayground/

## Questions / verrous

- maîtrise la latence dans le cadre faust2webaudio (Script Processor)
- gestion des cartes audio
- export des paramètres / presets


---
class: vertigo

# Conclusion

### Mise à disposition d’un harmoniseur modélisé depuis une œuvre mixte

- Absence d’installation spécifique : un navigateur suffit
- Mise en œuvre sur les sons du compositeur ou au micro
- Code Faust efficace et multi-cibles
- Code modifiable et réutilisable

## Développements futurs

- Personnalisation de l’interface, pour l’instant générée automatiquement
- Bibliothèque de modules de traitement => thésaurus
- Ensemble de presets propres aux œuvres et aux utilisateurs
- Nouvelle conception des analyses
- Associant modules manipulables et conteneurs temporels universels

---
class: center, middle, vertigo

# Merci !

<hr>
### JIM 2017 - 19/05/2017 - IRCAM
<img src="img/jim_horiz_blanc_1.png" height="100px" />
