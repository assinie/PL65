Fichier | Description
-----|------------
PL65-v0.plm | Correspond à la version ROM d'origine
PL65-v1.0.plm | Correction syntaxe code généré: (xxx)Y -> (xx),Y ainsi que pour les constantes ASCII: LDA #'A -> LDA #'A'
PL65-v1.1.plm | Ajout IFF, IF .flag
PL65-v1.2.plm | idem v1.1 mais utilise les nouvelles instructions de la v1.1 (sauf pour les labels en minuscules, pas encore supporté)
PL65-v1.3.plm | Ajout SET, CLR, STRING, id=.reg, minuscules et _ pour les identifiants, minuscules pour les instructions
PL65-v1.4.plm | idem v1.3 mais utilise les nouvelles instructions de la v1.3
PL65-v1.5.plm | Ajout INC .reg, DEC .reg, STACK .reg, UNSTACK .reg, id1=id2[.X|.Y], .reg=.reg|val, .regs<-id, .regs=##id, id<-.regs
PL65-v1.6.plm | idem v1.5 mais utilise les nouvelles instructions de la v1.5

**NOTES**
1. L'instruction STRING 'chaine' est un ajout personnel pour simplifier la gestion des chaînes de caractères. Elle écrit la chaîne avec le bit 7 du dernier caractère à 1. Exemple `STRING 'TEST'` génère `.BYT 'TES',$D4`.

2. Liste des flags:
	1. .C, .CARRY
	2. .O, .OVERFLOW, .V
	3. .N, .NEGATIVE
	4. .Z, .ZERO
	5. .D, .DECIMAL
	6. .I, .INTERRUPT

3. Liste des alias:
	1. .NOT -> ^
	2. .V -> .O
	3. CLEAR -> CLR

4. Liste de opérateur relationnels:
	1. <
	2. >=
	3. =
	4. ^=
	5. +
	5. -

