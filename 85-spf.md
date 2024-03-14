---
layout: page
title: SPF
permalink: spf.html
---

## Réglages SPF

Les réglages SPF sont un moyen d'empêcher les envois de spam depuis un domaine email.

Pour des informations plus complètes, se référer à l'article Wikipédia [Sender Policy Framework](https://fr.wikipedia.org/wiki/Sender_Policy_Framework).

Voici quelques exemples de réglages SPF:

`v=spf1 a mx ~all`


```
v=spf1 a mx ip4:195.70.4.147/24 ip4:94.126.18.188/24 ~all
```

Avec un réglage plus strict:

`v=spf1 mx -all` :  Allow domain's MXes to send mail for the domain, prohibit all others.

```
v=spf1 a/24 a:offsite.example.com/24 -all
```

Des outils de test pour vérifier le fonctionnement:

