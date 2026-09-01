---
title: Théorie de l’Information de Shannon / Entropie
aliases: [Entropie de Shannon, Théorie de l’Information]
tags: [principe, information, entropie, informatique]
domain: Systèmes-Formels
subdomain: Théorie-de-l-Information
authors: [Claude Shannon]
year: 1948
status: stable
related: [Deuxième-Principe-de-la-Thermodynamique]
---

# Théorie de l’Information de Shannon (Entropie de l’Information)

## Définition en une phrase
> L’information peut être quantifiée ; l’entropie d’un message mesure l’incertitude moyenne ou le nombre minimum de bits nécessaires pour l’encoder, établissant des limites fondamentales à la compression et à la communication fiable.

## Explication complète
Claude Shannon a défini l’entropie d’une variable aléatoire discrète \( X \) comme \( H(X) = -\sum p(x) \log_2 p(x) \). Cette quantité est le contenu moyen d’information par symbole et la borne inférieure du nombre moyen de bits nécessaires pour encoder les messages de cette source. Les théorèmes de capacité de canal donnent le taux maximal auquel l’information peut être transmise de façon fiable sur un canal bruyant. La théorie a créé le fondement mathématique de toute la communication numérique, de la compression de données et du codage.

## Explication à la manière de Feynman
Imaginez que vous voulez envoyer un message avec le moins possible de questions oui/non (bits). Si le message est complètement prévisible, vous n’avez besoin de presque aucun bit. S’il est complètement surprenant, vous en avez besoin de beaucoup. L’entropie de Shannon vous dit exactement combien de bits, en moyenne, sont nécessaires. Elle vous dit aussi combien de bruit vous pouvez tolérer avant que le message ne devienne irrécupérable.

## Métaphores et analogies clés

1. **« Vng mñn »** — Supprimer les voyelles compresse le message ; le contexte (redondance) permet encore de le récupérer.
2. **Dictionnaire de mots attendus** — Les messages courants reçoivent des codes courts ; les rares reçoivent des codes longs (comme le codage de Huffman).
3. **Compteur de surprise** — Plus un événement est surprenant, plus il porte d’information.

## Exemples concrets

1. **Compression de données** — ZIP, JPEG, MP3 s’approchent (mais ne peuvent pas dépasser) la limite d’entropie de la source.
2. **Codes correcteurs d’erreurs** — Le théorème de codage de canal de Shannon explique pourquoi nous pouvons envoyer des données presque sans erreur si nous restons en dessous de la capacité du canal (utilisé dans les communications spatiales profondes, la 5G, etc.).
3. **Langue anglaise** — L’entropie de l’anglais écrit est d’environ 1–1,5 bit par caractère en raison de sa forte redondance.

## Ancres quantitatives / de données
- Entropie : \( H(X) = -\sum p_i \log_2 p_i \)
- Fonction d’entropie binaire pour une pièce équitable : 1 bit
- Capacité de canal d’un canal bruyant : \( C = B \log_2 (1 + S/N) \) (Shannon-Hartley)

## Contexte historique et de découverte
L’article de Shannon de 1948 « A Mathematical Theory of Communication » a fondé le domaine. Il était motivé par des problèmes aux Bell Labs sur la transmission d’information sur des lignes téléphoniques bruyantes.

## Relations

### S’appuie sur / présuppose
- Théorie des probabilités
- Concept d’information comme réduction d’incertitude

### Influence / conduit à
- Toute la communication et le stockage numériques modernes
- Analogie formelle profonde avec l’entropie thermodynamique
- Apprentissage automatique (perte d’entropie croisée, etc.)

### Contraste avec
- Théories sémantiques de l’information (Shannon a délibérément ignoré le sens)

## Idées fausses courantes
- « La théorie de l’information traite du sens des messages. » → La théorie de Shannon traite des propriétés statistiques des signaux, pas de la sémantique.
- « Vous pouvez compresser n’importe quel fichier arbitrairement. » → La compression sans perte ne peut pas aller en dessous de l’entropie de la source en moyenne.

## Voir aussi
- [Deuxième Principe de la Thermodynamique](../../../Science/Physics/Thermodynamics/Second-Law-of-Thermodynamics.md)

## Tags
#principe #théorie-de-l-information #entropie #shannon #compression #communication
