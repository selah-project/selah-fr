# Contribuer à la version française de Selah

Merci d'aider cette version à devenir plus exacte, plus claire et plus
naturelle. Nul besoin d'être spécialiste pour signaler un problème :
expliquez ce que vous observez, apportez les éléments dont vous
disposez et distinguez une certitude d'une suggestion.

## Signalement ou demande de modification

- Ouvrez une **issue** quand la lecture demande discussion, qu'il
  existe plusieurs options possibles, ou que vous ne savez pas comment
  l'enregistrement aligné doit changer.
- Ouvrez une **pull request** quand l'erreur et le remplacement exact
  sont clairs.
- Pour les bogues de l'application, ou les questions privées de
  sécurité, de comptes ou de données personnelles, utilisez
  [le support de Selah](https://selahproject.com/support).

## Ce qu'il faut inclure

Indiquez le livre, le chapitre, le verset et le token hébreu ; le texte
actuel ; le texte proposé ; la raison du changement ; et la source
lexicale, grammaticale, contextuelle ou publiée qui l'appuie. Dites
aussi si vous êtes locuteur natif du français et si vous lisez
directement l'hébreu.

## Comment modifier un enregistrement

Les fichiers sont dans `<livre>/<chapitre>/<verset>.json`.

- Modifiez `translation` et le `gloss` du token concerné quand les deux
  sont touchés.
- Conservez `book`, `chapter`, `verse`, `ref`, les valeurs hébraïques
  `surface`, l'ordre et le nombre des tokens, sauf si vous signalez un
  défaut d'alignement.
- Ne changez pas les champs de modèle, de niveau, de date ou d'autre
  provenance pour présenter la correction comme une génération
  nouvelle.
- Conservez les conventions des chevrons, des Noms divins et de `⟨את⟩`.
- Évitez les changements de pure forme et les corrections sans rapport.

Vérifiez le JSON modifié :

```bash
python3 -m json.tool genesis/1/1.json >/dev/null
```

L'hébreu vient d'abord. Quand deux lectures sont défendables, expliquez
la différence au lieu de présenter une préférence comme une certitude.
Ne copiez pas une traduction moderne protégée par le droit d'auteur.

## Travail assisté par IA

Déclarez tout usage substantiel de modèles de langue ou de traduction
automatique, y compris le contrôle humain effectué. N'envoyez pas de
réécritures massives sans relecture. Qui contribue répond de chaque mot
proposé.

## Licence, attribution et relecture

En contribuant, vous déclarez en avoir le droit et acceptez que le
matériel incorporé soit distribué sous
[CC BY-SA 4.0](LICENSE.md). L'historique Git conserve le registre
public et l'attribution. L'équipe de maintenance compare la proposition
à l'hébreu, aux conventions, aux sources et à l'alignement. Elle peut
l'accepter, la réviser avec vous, attendre plus d'éléments ou la
refuser en expliquant pourquoi. Critiquez la lecture, non la personne.

## Conduct

Be honest, be kind, show your evidence. Distinguish certainty from
suggestion. The maintainers weigh and decide.
