# Architecture — Elyne Acta

[English](architecture.en.md) · [Présentation](../README.md)

## Flux simplifié

Demande → EIE et orchestration Acta → proposition d'outil → contrôle applicatif → exécution bornée → mémoire et journal Acta.

## Composants et frontières

- Acta emploie une application locale, un moteur d'inférence EIE, SQLite WAL pour l'état, et une recherche FTS5 combinée à des embeddings multilingues.
- Son ledger cognitif est propre à Acta : chaînage SHA-256, authentification HMAC et ancre selon le profil décrit. Il ne remplace ni le ledger ni les décisions d'EAS Defense.
- L'atelier de code et les outils réseau sont distincts de la conversation. Le confinement et les permissions doivent être vérifiés pour le service et la version déployés, pas déduits de leur description.

Ce schéma textuel décrit l'architecture du produit. Il ne remplace pas une vérification sur un build, un matériel et une configuration précis. Les [éléments de preuve](evidence.md) indiquent ce qui a été effectivement documenté.
