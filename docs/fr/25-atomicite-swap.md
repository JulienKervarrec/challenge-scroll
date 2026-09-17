# Atomicité du swap

Dans SimpleTokenSwap, le transfert du token entrant, l’approbation puis l’appel au routeur appartiennent à la même transaction. Un revert annule l’ensemble des effets d’état de cette transaction. Cette propriété ne supprime pas les risques de paramétrage, de liquidité ou de destinataire. Elle doit être distinguée d’une confirmation applicative reçue avant la finalité.
