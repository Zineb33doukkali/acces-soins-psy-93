# Acteurs du territoire – Accès aux soins psychologiques 93

## 🎯 Objectif
Ce document présente les principaux acteurs impliqués dans l’accès aux soins psychologiques pour les jeunes de **11 à 25 ans** en **Seine-Saint-Denis (93)**, ainsi que leurs **rôles** et **relations** dans le dispositif territorial.

---

## 🧩 1. Les acteurs du système

| **Acteur** | **Catégorie** | **Rôle principal** |
|-------------|----------------|--------------------|
| **Jeunes (11–25 ans)** | Public cible | Personnes concernées par les troubles psychologiques ; bénéficient d’un accompagnement et d’un suivi. |
| **Psychologues / Psychiatres** | Professionnels de santé | Assurent le diagnostic, le suivi thérapeutique et la coordination des soins psychologiques. |
| **Établissements scolaires** | Institutions éducatives | Repèrent les jeunes en difficulté, orientent vers les structures spécialisées, sensibilisent à la santé mentale. |
| **CMP / MDA** | Structures médico-sociales | Offrent un accompagnement psychologique gratuit, assurent la prise en charge des jeunes et de leurs familles. |
| **ARS Île-de-France** | Institution publique régionale | Coordonne et finance les dispositifs de santé mentale, planifie l’offre de soins et les politiques publiques. |
| **Collectivités locales (communes, département)** | Institutions territoriales | Soutiennent les structures locales, financent les programmes de prévention et d’accompagnement des jeunes. |
| **Hôpitaux / Dispositifs Psy (ex. Santé Psy Étudiant, Mon Soutien Psy)** | Structures de santé publique | Accueillent les jeunes en situation de crise ou nécessitant un suivi médical renforcé. |
| **Associations locales** | Acteurs associatifs et de terrain | Proposent écoute, prévention, accompagnement et actions sociales de proximité. |

---

## 🔁 2. Les relations entre acteurs

| **Lien entre acteurs** | **Type de relation** | **Exemple concret** |
|--------------------------|----------------------|----------------------|
| **Jeune ↔ Établissement scolaire** | Repérage / orientation | L’école identifie un élève en souffrance et le dirige vers un CMP. |
| **Jeune ↔ Psychologues / Psychiatres** | Prise en charge directe | Le jeune consulte un professionnel pour un suivi thérapeutique. |
| **Jeune ↔ Associations locales** | Accompagnement social | Participation à des ateliers d’écoute ou de soutien. |
| **Psychologues / Psychiatres ↔ ARS Île-de-France** | Régulation / financement | L’ARS finance les consultations du dispositif Santé Psy Étudiant. |
| **Établissements scolaires ↔ Collectivités locales** | Coopération locale | Mise en place de programmes de prévention santé à l’école. |
| **CMP / MDA ↔ Hôpitaux / Dispositifs Psy** | Coordination des soins | Orientation des cas complexes vers l’hôpital. |
| **Collectivités locales ↔ Associations locales** | Soutien financier et logistique | Subventions municipales aux structures d’aide psychologique. |

---

## 🧭 3. Lecture du schéma simplifié

Le schéma ci-dessous illustre la chaîne d’acteurs autour du jeune, depuis le repérage jusqu’à la prise en charge et le soutien :

```mermaid
classDiagram
    Animal <|-- Duck
    Animal <|-- Fish
    Animal <|-- Zebra
    Animal : +int age
    Animal : +String gender
    Animal: +isMammal()
    Animal: +mate()
    class Duck{
      +String beakColor
      +swim()
      +quack()
    }
    class Fish{
      -int sizeInFeet
      -canEat()
    }
    class Zebra{
      +bool is_wild
      +run()
    }
```
    A[Jeunes 11–25 ans] --> B[Psychologues / Psychiatres]
    A --> C[Établissements scolaires]
    A --> D[CMP / MDA]
    B --> E[ARS Île-de-France]
    C --> F[Collectivités locales]
    D --> G[Hôpitaux / Dispositifs Psy]
    F --> H[Associations locales]
    G --> H
