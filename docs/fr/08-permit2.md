# Signature Permit2

Le script examine quote.permit2.eip712 et, lorsqu’il est présent, prépare une signature de données typées. Il encode ensuite la longueur de la signature puis ajoute la signature aux données de transaction. Ce format dépend du contrat et du protocole attendus par la cotation. Toute modification de l’ordre, du domaine ou de la longueur peut rendre la transaction invalide ou signer un message différent de celui prévu.
