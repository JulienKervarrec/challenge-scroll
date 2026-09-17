# Niveau de frais

ExactInputSingleParams reçoit la valeur 3000 pour fee, correspondant au niveau de frais Uniswap V3 commenté dans le fichier. Le pool disponible doit effectivement exister pour cette paire et ce niveau. Une valeur codée en dur rend le contrat moins adaptable aux marchés dont la liquidité est concentrée ailleurs. Ce paramètre doit être confronté au réseau et à la liquidité ciblée avant chaque intégration.
