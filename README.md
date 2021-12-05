# TwilioQuest Pythonic Temple Extension

Extension for the Pythonic Temple in TwilioQuest.

## Deploy Checklist

- Ensure you have the latest changes you want to deploy on `main`
- Increment the version number in `package.json`
  - commit this change
  - push to remote
- Run `npm publish`
  - If you do not have access to this package contact Ryan Kubik or Kevin Whinnery
- Once published, update the `twilioquest-python` dependency in [the twilioquest repository](https://github.com/twilio/twilioquest) to use this latest deployed version
- Ensure no changes need to happen to [the twilioquest template extension](https://github.com/twilioquest/twilioquest-extension-template)
- Release a new TwilioQuest build with updated base dependency

# Extension pour le Temple Pythonique dans TwilioQuest

Extension pour le Temple Pythonique dans TwilioQuest.

## Liste de contrôle pour le déploiement

- Assurez-vous que vous avez les derniers changements que vous voulez déployer sur `main`.
- Incrémentez le numéro de version dans `package.json`
  - Livrez cette modification
  - pousser à distance
- Exécutez `npm publish`
  - Si vous n'avez pas accès à ce paquet, contactez Ryan Kubik ou Kevin Whinnery.
- Une fois publié, mettez à jour la dépendance `twilioquest-python` dans [le dépôt twilioquest] (https://github.com/twilio/twilioquest) pour utiliser la dernière version déployée.
- Assurez-vous qu'aucune modification ne doit être apportée à [l'extension de modèle twilioquest] (https://github.com/twilioquest/twilioquest-extension-template).
- Publiez une nouvelle version de TwilioQuest avec la dépendance de base mise à jour.

