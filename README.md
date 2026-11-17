# mklean_Talent_AI — Template interactif V3

**MKLEAN Recruiting** · éditeur CLV TECH · prototype de démonstration multipage.

## Démarrer

- Ouvrir `index.html` dans Chrome ou Edge après extraction de l’archive.
- Vous pouvez également ouvrir `mklean_Talent_AI_Prototype.html` (fichier autonome).
- Aucune installation ni serveur n’est requis. Les données fictives sont conservées dans le `localStorage` du navigateur.

## Pages et fonctionnalités

**Talent & recrutement** : tableau de bord, CVthèque, import simulé PDF/DOCX, profil 360°, séquenceur carrière, taxonomie des compétences, recherche et matching local explicable, offres, Kanban recrutement, entretiens (rémunération, prétentions, mobilité, motivations), talents passifs, évaluations psychométriques pilotes, placements.

**Entreprise & CRM** : comptes entreprises, fiches enrichies, référentiel multi-secteur simplifié, contacts professionnels, activités, pipeline CRM, offres liées, signaux d’entreprise.

**Intelligence économique** : nomenclature HCP / CCIS illustrative, générateur d’études sectorielles / emploi / salaires / territoire / entreprises, aperçu imprimable PDF et export CSV, observatoire emplois et rémunérations agrégées avec taille d’échantillon, veille de signaux publics saisie.

**Relations multicanales** : sourcing LinkedIn (ouvertures depuis l’interface, journal interne, import CSV pilote), boîte WhatsApp fictive, réception simulée de CV, historique multicanal, rappels et opposition.

**Services** : espaces candidat et employeur (aperçu uniquement), copilote analytique à règles locales, tableaux de bord, paramètres et conformité.

## Limites importantes

- **Aucune API live** : ni LinkedIn, ni WhatsApp, ni web, ni modèle IA/Ollama ne sont connectés ; les messages restent simulés.
- Le matching de la démo utilise des règles transparentes et non de véritables embeddings sémantiques. Les études sont descriptives, non représentatives du marché marocain.
- Les tests Hogan nécessitent une licence ; les inventaires IPIP nécessitent une adaptation/validation méthodologique. Aucun score clinique ou psychométrique réel n’est produit.
- La classification HCP/CCIS est un *exemple de structure* et doit être remplacée par un référentiel officiel importé/versionné et ses mappings vérifiés.
- Le backend Django doit assurer authentification, permissions granulaires, confidentialité des rémunérations et tests, chiffrement, logs d’audit, validité des consentements, traitement sécurisé des documents et formalités CNDP applicables.
- Les fonctionnalités de génération PDF correspondent à l’impression navigateur ; l’export Excel/Word structuré requiert un backend.

## Structure

- `index.html` : application locale
- `app.js` : données fictives, routes et logique interactive
- `styles.css` : design system MKLEAN (logo blanc sur fond foncé)
- `assets/mklean-logo.png` : logo fourni, non redessiné
- `assets/clv-tech-logo.png` : logo secondaire de l’éditeur (pour usages futurs)

## Scénarios testables

1. Dashboard → Entreprises & CRM → Fiche compte → Ajouter interaction → Pipeline CRM.
2. Candidats → Fiche → Séquenceur → Entretien → Évaluations.
3. Études de marché → Sélectionner HCP, secteur et région → Générer → Imprimer/PDF ou CSV.
4. Entretiens → Nouvelle qualification volontaire → Observatoire emploi (statistiques agrégées).
5. LinkedIn → Déclaration / import pilote → Historique multicanal → Relance.
6. Veille emploi → Ajouter signal sourcé → Vérifier → Fiche entreprise.

**Version** : V3.0 · 2 novembre 2026 · Démonstration uniquement.
