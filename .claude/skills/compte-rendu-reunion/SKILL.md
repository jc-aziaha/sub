---
name: compte-rendu-reunion
description: Rédige le compte-rendu d'une réunion de recueil du besoin client à partir d'une transcription (Fathom ou autre), puis le compare au compte-rendu du Product Owner pour signaler les écarts, ambiguïtés et contradictions. À utiliser pour la première étape du projet.
---

# Compte-rendu de réunion de recueil du besoin

## Entrées
- La transcription brute, dans `docs/entrees/` (souvent un export HTML : ignore le balisage).
- Le compte-rendu rédigé par le Product Owner, quand il existe (pour la comparaison).

## Ton et style

Le compte-rendu doit se lire comme le récit fidèle d'un échange entre deux personnes, pas comme un export de transcription.
- **Rédige en phrases claires**, pas en fragments. Les tableaux servent à ranger l'information (besoins, actions), pas à remplacer le récit.
- **Raconte la situation de la cliente** : qui elle est, ce qu'elle vit, ce qui la gêne, ce qu'elle espère. Cite ses mots courts, entre guillemets, quand ils rendent bien ce qu'elle ressent.
- **Mets en avant ce qui compte pour elle** (ses priorités, ses craintes, ce qu'elle refuse), pas seulement ce qui a été dit.
- **Pas d'horodatages dans le corps du texte.** Le compte-rendu ne suit pas le déroulé minute par minute. Ne cite un horodatage que pour un passage douteux ou une ambiguïté que le Product Owner devra vérifier.
- **Ton professionnel et chaleureux**, neutre, sans jargon, compréhensible par la cliente si elle le lit.
- **Reste court** : un lecteur doit comprendre l'essentiel en deux minutes.

## Méthode

### 1. Lecture de la transcription
1. Lis la transcription en entier avant de rédiger.
2. Une transcription automatique contient des erreurs : mots mal reconnus, noms propres, chiffres, locuteurs mal identifiés. Quand un passage est douteux, ne le corrige pas : signale-le.
3. Si la transcription est incomplète (coupure, passage inaudible), dis-le en tête du compte-rendu.

### 2. Rédaction
1. Remplis `references/gabarit-compte-rendu-reunion.md`.
2. Sépare toujours trois niveaux : ce qui a été **dit**, ce qui a été **décidé**, ce qui reste **à confirmer**.
3. Attribue chaque demande ou engagement à son auteur (client ou Product Owner) quand la transcription le permet.
4. Numérote les besoins exprimés (`B-01`, `B-02`...) : ces identifiants serviront dans les documents suivants.
5. Le plan d'action donne pour chaque action un responsable et une échéance si elle a été citée, sinon `[À CLARIFIER]`.
6. Liste dans une section dédiée les **ambiguïtés** et les **contradictions**, avec la question à poser. **Hiérarchise** : garde celles qui bloquent la suite ou changent le périmètre, le budget ou le délai (une dizaine au plus), et regroupe ou omets les détails mineurs.
7. Ne qualifie pas le type de projet (site, application, autre) tant que la cliente ne l'a pas dit clairement.

### 3. Comparaison avec le compte-rendu du Product Owner
Quand le Product Owner a rédigé le sien, présente un tableau des écarts :

| Point | Dans les deux | Seulement chez le PO | Seulement chez Percy | Contradiction |
|---|---|---|---|---|

Pour chaque écart, cite la source dans la transcription. Propose une version fusionnée. Le Product Owner tranche.

### 4. Validation
Le brouillon reste dans le chat jusqu'à la validation explicite du Product Owner. Écris le fichier seulement ensuite, à l'emplacement qu'il indique.

## Règles
- Pas de reformulation qui change le sens ou le niveau de certitude (« peut-être » ne devient pas « oui »).
- Les informations personnelles de la cliente se limitent à ce qui est utile au projet.
- Un compte-rendu validé ne contient plus de marqueur `[À CLARIFIER]` : chaque point est tranché, ou devient un point « à confirmer » avec son responsable.
