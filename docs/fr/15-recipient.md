# Destinataire de la sortie

Le paramètre recipient est transmis directement à exactInputSingle. Les tokens de sortie ne sont donc pas nécessairement envoyés à msg.sender. Cette distinction est importante pour les interfaces et les signatures : l’adresse affichée à l’utilisateur doit être celle réellement signée. Un contrôle applicatif doit empêcher un destinataire inattendu ou nul selon les règles du protocole.
