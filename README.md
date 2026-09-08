# DmxUtilities — flux de mise à jour

Ce dépôt ne contient **pas** de code source. Il sert uniquement de flux de
publication [Sparkle](https://sparkle-project.org) pour DmxUtilities, dont les
sources vivent dans un dépôt privé.

Sparkle télécharge en HTTP anonyme et ne sait pas s'authentifier auprès de
GitHub : c'est la seule raison pour laquelle ce dépôt est séparé et public.

- `appcast.xml` — le flux interrogé par l'application
- `releases/` — les archives, signées EdDSA

Chaque archive est signée avec une clé privée qui ne quitte jamais le trousseau
de la machine de build. Une archive non signée par cette clé est refusée par
l'application, même si ce dépôt était compromis.
