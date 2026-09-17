# Cotation et calldata

index.ts demande une cotation avant de construire la transaction. La réponse de cotation fournit notamment les données d’appel et les informations nécessaires à la signature. Le script réutilise ensuite ces éléments pour composer la transaction brute. Cette séparation entre estimation et exécution impose de contrôler que les paramètres réellement signés correspondent encore à la cotation affichée.
