| Menace STRIDE          | Exemple dans ton projet                        | Contre-mesure                             |
| ---------------------- | ---------------------------------------------- | ----------------------------------------- |
| **S**: Spoofing        | Login sans mot de passe via un endpoint oublié | Authentification forte, suppression route |
| **T**: Tampering       | Modifier un JWT pour devenir admin             | Signature JWT + validation serveur        |
| **R**: Repudiation     | L’utilisateur nie avoir supprimé son compte    | Journalisation avec horodatage            |
| **I**: Info Disclosure | Stack trace qui montre la DB dans une erreur   | Messages d’erreurs génériques             |
| **D**: DoS             | 1000 requêtes `/login`/sec pour saturer l’app  | Rate limiting, CAPTCHA                    |
| **E**: Privilege Elev. | Accès `/admin` en modifiant `/user` dans l’URL | Contrôle d’accès par rôle                 |
