---
version: alpha
name: Itaja — Malachite & Cuivre
description: >-
  Teal revisité, for Itaja — merchant of record and monetization infrastructure
  for African SaaS. Mineral green-teal primary, copper for money, warm ivory
  canvas. The metal and its patina, the two states of one material.
colors:
  # ——— palettes principales ———
  primary: "#0E5F52"
  secondary: "#0A1F1B"
  tertiary: "#C0703A"
  neutral: "#FAF8F3"

  # ——— surfaces ———
  surface: "#FAF8F3"
  surface-tint: "#ECEFE9"
  surface-raised: "#E2E9E3"
  surface-warm: "#F0E0D2"
  hairline: "#D7E1DB"
  on-surface: "#0A1F1B"
  on-surface-muted: "#0E5F52"
  on-primary: "#FAF8F3"

  # ——— échelle malachite (pigment de marque) ———
  malachite-900: "#0A4A40"
  malachite-800: "#0E5F52"
  malachite-700: "#1A7361"
  malachite-500: "#47A18E"
  malachite-400: "#5FB8A3"
  malachite-300: "#8ACFBC"
  malachite-100: "#D9F0E8"

  # ——— cuivre (l'argent) ———
  copper: "#C0703A"
  copper-light: "#E3B58C"
  on-copper: "#0A1F1B"

  # ——— états système ———
  success: "#0E5F52"
  on-success: "#FAF8F3"
  error: "#A5372A"
  on-error: "#FAF8F3"
  info: "#2C6BC4"
  on-info: "#FAF8F3"
  attention-surface: "#E2E9E3"
  attention-indicator: "#A5372A"

  # ——— séries de données : séparation de luminance vérifiée ———
  data-1: "#0A4A40"
  data-2: "#C0703A"
  data-3: "#E3B58C"
  data-4: "#47A18E"
  data-5: "#2C6BC4"

  # ——— bascule mode sombre ———
  surface-dark: "#0A1F1B"
  surface-dark-raised: "#10302A"
  on-surface-dark: "#FAF8F3"
  on-surface-dark-muted: "#E4DACA"
  primary-dark: "#5FB8A3"
  hairline-dark: "rgba(250,248,243,.12)"

typography:
  display:
    fontFamily: Bricolage Grotesque
    fontSize: 56px
    fontWeight: 800
    lineHeight: 1.02
    letterSpacing: "-0.035em"
  headline-lg:
    fontFamily: Bricolage Grotesque
    fontSize: 34px
    fontWeight: 700
    lineHeight: 1.08
    letterSpacing: "-0.025em"
  headline-md:
    fontFamily: Bricolage Grotesque
    fontSize: 24px
    fontWeight: 700
    lineHeight: 1.14
    letterSpacing: "-0.02em"
  headline-sm:
    fontFamily: Bricolage Grotesque
    fontSize: 19px
    fontWeight: 600
    lineHeight: 1.2
    letterSpacing: "-0.012em"
  headline-xs:
    fontFamily: Rubik
    fontSize: 16px
    fontWeight: 600
    lineHeight: 1.3
  body-lg:
    fontFamily: Rubik
    fontSize: 17px
    fontWeight: 400
    lineHeight: 1.65
  body-md:
    fontFamily: Rubik
    fontSize: 15px
    fontWeight: 400
    lineHeight: 1.6
  body-sm:
    fontFamily: Rubik
    fontSize: 13px
    fontWeight: 400
    lineHeight: 1.5
  label:
    fontFamily: Rubik
    fontSize: 11px
    fontWeight: 600
    lineHeight: 1.35
    letterSpacing: "0.09em"
  data-lg:
    fontFamily: JetBrains Mono
    fontSize: 21px
    fontWeight: 500
    lineHeight: 1.2
    letterSpacing: "-0.01em"
    fontFeature: "'tnum' 1, 'zero' 1"
  data-md:
    fontFamily: JetBrains Mono
    fontSize: 13px
    fontWeight: 500
    lineHeight: 1.5
    fontFeature: "'tnum' 1, 'zero' 1"
  code:
    fontFamily: JetBrains Mono
    fontSize: 13px
    fontWeight: 400
    lineHeight: 1.6
    fontFeature: "'tnum' 1, 'zero' 1"

rounded:
  none: 0
  sm: 6px
  md: 10px
  lg: 14px
  xl: 20px
  full: 9999px

spacing:
  base: 4px
  xs: 4px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 32px
  2xl: 48px
  3xl: 64px
  gutter: 24px
  margin: 32px
  max-width: 1200px
  measure: 640px
  control-height: 44px

components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.body-md}"
    rounded: "{rounded.md}"
    padding: 12px
    height: "{spacing.control-height}"
  button-primary-hover:
    backgroundColor: "{colors.malachite-900}"
  button-primary-active:
    backgroundColor: "{colors.secondary}"

  button-money:
    backgroundColor: "{colors.copper}"
    textColor: "{colors.on-copper}"
    typography: "{typography.body-md}"
    rounded: "{rounded.md}"
    padding: 12px
    height: "{spacing.control-height}"
  button-money-hover:
    backgroundColor: "{colors.copper-light}"

  button-secondary:
    backgroundColor: "{colors.surface-tint}"
    textColor: "{colors.primary}"
    typography: "{typography.body-md}"
    rounded: "{rounded.md}"
    padding: 12px
    height: "{spacing.control-height}"
  button-secondary-hover:
    backgroundColor: "{colors.surface-raised}"

  button-ghost:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.primary}"
    typography: "{typography.body-md}"
    rounded: "{rounded.md}"
    padding: 12px
  button-ghost-dark:
    backgroundColor: "{colors.surface-dark}"
    textColor: "{colors.on-surface-dark}"
    rounded: "{rounded.md}"
    padding: 12px

  input-field:
    backgroundColor: "{colors.surface-raised}"
    textColor: "{colors.on-surface}"
    typography: "{typography.body-md}"
    rounded: "{rounded.sm}"
    padding: 12px
    height: "{spacing.control-height}"
  input-field-error:
    backgroundColor: "{colors.surface-raised}"
    textColor: "{colors.error}"
  input-field-focus:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.on-surface}"

  checkbox:
    backgroundColor: "{colors.surface-raised}"
    textColor: "{colors.on-surface}"
    rounded: "{rounded.sm}"
    size: 18px
  checkbox-checked:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"

  radio:
    backgroundColor: "{colors.surface-raised}"
    textColor: "{colors.on-surface}"
    size: 18px
  radio-selected:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"

  chip-neutral:
    backgroundColor: "{colors.surface-raised}"
    textColor: "{colors.on-surface}"
    typography: "{typography.label}"
    rounded: "{rounded.full}"
    padding: 6px
  chip-settled:
    backgroundColor: "{colors.success}"
    textColor: "{colors.on-success}"
    typography: "{typography.label}"
    rounded: "{rounded.full}"
    padding: 6px
  chip-pending:
    backgroundColor: "{colors.copper}"
    textColor: "{colors.on-copper}"
    typography: "{typography.label}"
    rounded: "{rounded.full}"
    padding: 6px
  chip-failed:
    backgroundColor: "{colors.error}"
    textColor: "{colors.on-error}"
    typography: "{typography.label}"
    rounded: "{rounded.full}"
    padding: 6px
  chip-info:
    backgroundColor: "{colors.info}"
    textColor: "{colors.on-info}"
    typography: "{typography.label}"
    rounded: "{rounded.full}"
    padding: 6px

  card:
    backgroundColor: "{colors.surface-raised}"
    textColor: "{colors.on-surface}"
    rounded: "{rounded.lg}"
    padding: 16px
  card-money:
    backgroundColor: "{colors.surface-warm}"
    textColor: "{colors.on-surface}"
    rounded: "{rounded.lg}"
    padding: 16px
  card-dark:
    backgroundColor: "{colors.surface-dark}"
    textColor: "{colors.on-surface-dark}"
    rounded: "{rounded.lg}"
    padding: 16px
  card-dark-raised:
    backgroundColor: "{colors.surface-dark-raised}"
    textColor: "{colors.on-surface-dark}"
    rounded: "{rounded.lg}"
    padding: 16px
  card-editorial:
    backgroundColor: "{colors.surface-tint}"
    textColor: "{colors.on-surface}"
    rounded: "{rounded.lg}"
    padding: 24px

  kpi-value:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.on-surface}"
    typography: "{typography.data-lg}"
  kpi-label:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.on-surface-muted}"
    typography: "{typography.label}"
  kpi-trend:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.success}"
    typography: "{typography.data-md}"
  kpi-trend-dark:
    backgroundColor: "{colors.surface-dark}"
    textColor: "{colors.copper-light}"
    typography: "{typography.data-md}"

  amount-cell:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.on-surface}"
    typography: "{typography.data-md}"
  amount-cell-positive:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.success}"
    typography: "{typography.data-md}"
  amount-cell-negative:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.error}"
    typography: "{typography.data-md}"

  alert-attention:
    backgroundColor: "{colors.attention-surface}"
    textColor: "{colors.on-surface}"
    typography: "{typography.body-sm}"
    rounded: "{rounded.md}"
    padding: 12px
  alert-attention-rule:
    backgroundColor: "{colors.attention-indicator}"
    height: 2px
  alert-error:
    backgroundColor: "{colors.error}"
    textColor: "{colors.on-error}"
    typography: "{typography.body-sm}"
    rounded: "{rounded.md}"
    padding: 12px

  chart-series-1:
    backgroundColor: "{colors.data-1}"
    height: 8px
  chart-series-2:
    backgroundColor: "{colors.data-2}"
    height: 8px
  chart-series-3:
    backgroundColor: "{colors.data-3}"
    height: 8px
  chart-series-4:
    backgroundColor: "{colors.data-4}"
    height: 8px
  chart-series-5:
    backgroundColor: "{colors.data-5}"
    height: 8px

  divider:
    backgroundColor: "{colors.hairline}"
    height: 1px
  divider-dark:
    backgroundColor: "{colors.hairline-dark}"
    height: 1px

  button-primary-dark:
    backgroundColor: "{colors.surface-dark}"
    textColor: "{colors.primary-dark}"
    typography: "{typography.body-md}"
    rounded: "{rounded.md}"
    padding: 12px
  kpi-label-dark:
    textColor: "{colors.on-surface-dark-muted}"
    typography: "{typography.label}"

  list-item:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.on-surface}"
    typography: "{typography.body-md}"
    padding: 12px
  list-item-hover:
    backgroundColor: "{colors.surface-tint}"

  tooltip:
    backgroundColor: "{colors.secondary}"
    textColor: "{colors.on-surface-dark}"
    typography: "{typography.body-sm}"
    rounded: "{rounded.sm}"
    padding: 8px

  page:
    backgroundColor: "{colors.neutral}"
    textColor: "{colors.on-surface}"
---

# Itaja — Malachite &amp; Cuivre

> Variante « teal revisité ». Elle remplace le teal cyan d'origine par un pigment minéral et l'assortit
> d'un cuivre. L'autre direction du projet, chaude (ocre et bronze), vit dans `DESIGN.md`.

## Overview

Itaja est l'infrastructure de monétisation et le **merchant of record** des SaaS africains : encaisser, facturer, abonner, reverser. Le produit se consulte tous les jours sans se regarder — un tableau de bord de paiements, une API, un checkout embarqué. L'interface doit donc être **calme, dense et lisible**.

**L'idée de marque tient en une phrase : le cuivre et sa patine.** La malachite est un minerai de cuivre — littéralement le métal dans son autre état. Une seule matière, deux moments : **ce qui circule** (le cuivre, l'argent qui va au marchand) et **ce qui tient** (la patine, l'infrastructure qui dure). C'est exactement ce que fait Itaja, et aucun concurrent africain ne raconte cette histoire. Les deux pigments viennent du continent : la malachite de la ceinture de cuivre d'Afrique centrale, le cuivre de la manille qui servait de monnaie en Afrique de l'Ouest.

Cette direction répond aux objectifs du projet :

- **Être un merchant of record, pas une passerelle.** Le pigment est minéral et mat, jamais brillant : une matière qui rassure un trésorier, pas une app grand public. Itaja doit avoir l'air d'une institution, pas d'un produit marketing.
- **Rendre l'argent visible.** Le cuivre est la seule couleur chaude et il ne parle que d'argent : la part du marchand, les montants encaissés, les reversements à venir. Là où tout le secteur code le résultat financier en vert, Itaja le code en métal.
- **Revendiquer une identité africaine sans folklore.** La souveraineté technologique se dit avec deux minéraux, pas avec des motifs.
- **Laisser le produit du client au centre.** Environ 78 % d'un écran est un neutre chaud. La couleur est un événement.

Le contexte concurrentiel a guidé la teinte : le navy et le bleu sont le territoire occupé du paiement africain (Flutterwave `#262C55`, Paystack midnight blue, la convention documentée « dark navy ou slate blue + vert »). Le teal d'origine d'Itaja `#2E6D6D` était **exactement à 0° de teinte** de celui de Flutterwave `#00abab` — indistinguable par la teinte, seulement plus sombre. Le pigment retenu ici descend à **170°**, soit un vert minéral plus froid et nettement plus sombre : la famille reste voisine, la matière change. Ce qui différencie vraiment, c'est la paire — vert minéral et cuivre sont à **146° l'un de l'autre**, une opposition que personne n'occupe dans le secteur.

## Colors

Une famille minérale, un métal, quatre neutres chauds. La palette est volontairement étroite : un pigment de marque, un accent, des états.

- **Primary — Malachite `#0E5F52` :** vert minéral profond, mat, sans virage bleu. Titres, liens, actions, succès. Contraste 7,12:1 sur ivoire — il porte du texte sans difficulté.
- **Secondary — Nuit minérale `#0A1F1B` :** l'encre et les surfaces sombres. Un noir vert, pas un gris : c'est le même monde que la malachite, éteint. Contraste 16,16:1 sur ivoire. Remplace tout noir pur.
- **Tertiary — Cuivre `#C0703A` :** *l'argent*. Remplissage uniquement — jauges de revenus, part marchand, états d'attente, série 2 des graphiques. L'encre umber dessus donne 4,59:1. **Jamais en texte** : 3,52:1 sur ivoire.
- **Neutral — Ivoire `#FAF8F3` :** le fond. Un blanc chaud, jamais clinique. Un ivoire chaud sous un pigment froid, c'est ce qui empêche la marque de retomber dans le teal corporate.

**Le cuivre n'a qu'un registre, et c'est un aplat.** Un cuivre foncé aurait été nécessaire pour un usage en texte — il a été écarté : mesuré, il tombe à **29,9 unités** de la rouille d'erreur, deux bruns-rouges confondables dans un tableau où erreurs et montants cohabitent en permanence. Donc les montants s'écrivent en encre, le cuivre remplit. Et sur les remplissages de cuivre, **le survol éclaircit au lieu d'assombrir** — le métal chauffe — ce qui évite d'introduire un cuivre sombre.

**Deux familles d'états, jamais mélangées.** Les *états d'argent* (encaissé, en attente, reversé) utilisent la malachite et le cuivre. Les *états système* (succès, attention, erreur, information) utilisent la malachite, la rouille `#A5372A` et le bleu `#2C6BC4`. Un état système n'emprunte jamais la couleur de l'argent.

**L'attention ne se signale pas par un aplat.** Elle se compose d'une surface minérale pâle, d'un filet rouille de 2 px et d'une icône. Le vert mousse d'un succès distinct a été écarté : à **64 unités** de la malachite, il créait deux verts d'entreprise dans le même écran. **Le succès, c'est la malachite** — la marque et le positif ne font qu'un.

**Les séries de données forment une échelle de luminance avant d'être une échelle de teintes.** Ordre d'attribution fixe : malachite profonde → cuivre → cuivre clair → malachite claire → bleu. Les écarts de contraste entre paliers voisins vont de **1,66 à 2,72**, tous au-dessus du seuil de 1,35 : le graphique reste lisible pour un daltonien, qui perd la teinte mais garde la luminosité. Une rampe de neuf paliers avait été testée d'abord — sept des huit écarts tombaient sous le seuil, elle a été réduite à cinq.

## Typography

Deux familles pour le récit, une pour les chiffres. Les trois sont sous **SIL Open Font License 1.1** : usage commercial libre, auto-hébergement et embarquement autorisés.

- **Bricolage Grotesque (display) :** titres et chiffres clés. Grotesque à caractère, terminaisons légèrement adoucies — le seul actif de l'identité qu'un concurrent ne peut pas copier sans se trahir, et c'est elle qui empêche un système minéral de devenir froid. Graisses 600, 700, 800. Jamais en corps sous 15 px.
- **Rubik (corps & UI) :** paragraphes, interface, boutons, champs, labels. Angles légèrement arrondis, lisible en petit corps — ce qui compte sur les écrans d'entrée de gamme où passent les paiements mobile money. Graisses 400, 500, 600.
- **JetBrains Mono (données & code) :** montants, volumes, identifiants, extraits d'API. Chiffres tabulaires activés par `fontFeature` — sans quoi deux lignes de montants ne s'alignent pas et un tableau de paiements devient illisible.

**Règles.** Un seul rôle display par écran. Interlettrage négatif au-dessus de 24 px, positif sur les micro-labels en capitales. Hiérarchie par la taille et la graisse, jamais par la couleur seule. 66 caractères de ligne maximum. Aucun faux gras, aucun faux italique.

**En email**, replis obligatoires : `system-ui`, Arial/Helvetica, Courier.

## Layout

Mise en page **fluide à largeur maximale fixe** : 1200 px sur desktop, gouttière de 24 px, marge de 32 px. Ruptures à 640, 768, 1024 et 1280 px.

Échelle d'espacement en **base 4 px** avec des pas de 8. Les composants sont regroupés par containment : les éléments liés vivent dans une carte à rayon large et padding généreux, plutôt que séparés par des filets partout. Mesure de lecture plafonnée à 640 px, soit environ 66 caractères en corps 15 px.

Hauteur de contrôle standard : **44 px** pour tout élément interactif. Cible tactile confortable sur mobile, et alignement vertical d'une ligne de formulaire avec une cellule de tableau.

Les tableaux de montants s'alignent **à droite**, code devise compris.

## Elevation & Depth

Le système est **plat et tonal**. Aucune ombre diffuse : la profondeur se lit par contraste de surface.

Trois niveaux en mode clair, tous des teintes de malachite ou de cuivre sur ivoire : le fond `#FAF8F3`, la surface voilée `#ECEFE9`, la surface posée `#E2E9E3`. Plus une surface chaude `#F0E0D2`, teinte de cuivre, réservée aux encarts d'argent. En mode sombre, la progression s'inverse en luminance : `#0A1F1B`, puis `#10302A`.

La séparation entre deux surfaces voisines se fait par un **filet de 1 px** — `#D7E1DB` en clair, `rgba(250,248,243,.12)` en sombre.

**Règle du mode sombre.** Tous les aplats colorés décrochent du seuil de contraste non-textuel de 3:1 face à la nuit minérale — la rouille tombe à 2,60, le bleu à 3,27, la malachite profonde à 1,69. Ils restent lisibles *en eux-mêmes* grâce à leur encre, mais leur contour se confond avec le fond. Donc : **tout aplat porte un filet `rgba(250,248,243,.16)` en mode sombre**, et **la série 1 des graphiques bascule vers la malachite claire `#5FB8A3`** (7,24:1 au lieu de 1,69).

Le mode sombre n'est pas un gris : c'est la **nuit de malachite**, la même famille que le pigment, éteinte. C'est le pendant du canvas ivoire à l'autre bout de la luminosité.

## Shapes

Langage **arrondi et sobre**. Aucun angle vif : rayons de 6 à 20 px selon la taille de l'élément, plus `full` pour les pastilles de statut. Le rayon suit la surface — une puce ne prend pas le rayon d'une carte. Aucun élément ne mélange un angle vif et un angle arrondi dans la même vue.

La pastille de statut est **entièrement ronde** : c'est une forme, pas un bouton.

## Components

`button-primary` est la **seule action de haute emphase par écran** : malachite plein, encre ivoire, 7,12:1. Au survol il s'assombrit vers la malachite 900 ; à l'appui il descend jusqu'à la nuit minérale.

`button-money` porte **l'action sur l'argent** — reverser, retirer, programmer un payout — et non l'action principale du produit. Sa surface est le cuivre, son encre l'umber. **Le vert agit, le cuivre paie** : c'est la distinction structurelle de l'interface. Son survol éclaircit vers le cuivre clair, par choix documenté.

`input-field` et `input-field-error` partagent la même surface ; seul le texte change de couleur. L'erreur ne colore jamais le fond d'un champ.

Les `chip-*` couvrent les états d'un paiement : `chip-settled` (malachite), `chip-pending` (cuivre), `chip-failed` (rouille), `chip-info` (bleu), `chip-neutral` (surface posée). Libellé en majuscules espacées, corps `label`. Aucune ne repose sur la couleur seule — chacune porte un libellé explicite.

`card-money` est l'encart de revenus : surface teintée de cuivre, montant en `data-lg`, libellé en `label`. `card-editorial` porte les moments de marque. `card-dark` et `card-dark-raised` sont les surfaces de nuit, dans cet ordre d'élévation.

`amount-cell` et ses variantes traitent les montants en `data-md`, tabulaires, alignés à droite. Le signe est collé au montant ; jamais de parenthèses comptables.

`chart-series-1` à `-5` fixent l'ordre d'attribution des séries. Une série garde son rang d'un écran à l'autre.

`alert-attention` associe une surface minérale et un filet rouille — `alert-attention-rule` en est le filet de 2 px, isolé comme composant parce que c'est lui qui porte le sens. `alert-error` est le seul aplat rouge plein du système.

## Do's and Don'ts

- **Do** maintenir environ 78 % de neutre chaud, 9 % de surface minérale, 8 % de malachite, ≤ 2 % de nuit.
- **Do** réserver le cuivre aux montants, aux jauges de revenus et aux actions sur l'argent — le vert agit, le cuivre paie.
- **Do** écrire tous les montants en encre, en JetBrains Mono tabulaire, alignés à droite, code ISO 4217 en capitales après le montant (`25 000 XOF`).
- **Do** exprimer l'attention par la forme : surface minérale, filet rouille de 2 px, icône, libellé.
- **Do** porter un filet `rgba(250,248,243,.16)` sur tout aplat en mode sombre, et basculer la série 1 des graphiques vers la malachite claire.
- **Do** maintenir WCAG AA : 4,5:1 pour le texte courant, 3:1 pour le grand texte et les éléments d'interface.
- **Don't** écrire en cuivre — c'est une surface, jamais une encre (3,52:1 sur ivoire).
- **Don't** employer l'ombre, le dégradé ou le néon : la profondeur est tonale, la matière est mate.
- **Don't** introduire un cuivre sombre : il tomberait à 29,9 unités de la rouille d'erreur.
- **Don't** créer un vert de succès distinct de la malachite — le mousse `#3F6B2A` est à 64 unités du pigment, deux verts d'entreprise sur un même écran.
- **Don't** utiliser la malachite ou le cuivre comme état système, ni la rouille ou le bleu comme état d'argent.
- **Don't** colorer une devise. Le cuivre dit « argent qui circule », pas « XOF ».
- **Don't** utiliser une rampe de plus de cinq paliers pour des séries de données : la rampe complète comprime la luminance et devient illisible pour un daltonien.
- **Don't** mélanger un angle vif et un angle arrondi dans la même vue.
