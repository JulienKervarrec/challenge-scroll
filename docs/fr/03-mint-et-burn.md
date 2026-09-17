# Création et destruction de l’offre

TONCONTRAT expose mint et burn comme fonctions publiques. mint permet à l’appelant de créer des unités pour une adresse donnée, tandis que burn détruit des unités depuis l’adresse appelée selon le code présent. Aucune restriction de rôle n’apparaît dans ce fichier autour de ces fonctions. Ce choix doit être documenté comme une propriété de conception à vérifier avant tout usage en production, et non comme une vulnérabilité automatiquement démontrée.
