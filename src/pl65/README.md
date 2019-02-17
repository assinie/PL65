Fichier | Description
-----|------------
PL65-v0.plm | Correspond à la version ROM d'origine
PL65-v1.0.plm | Correction syntaxe code généré: (xxx)Y -> (xx),Y ainsi que pour les constantes ASCII: LDA #'A -> LDA #'A'
PL65-v1.1.plm | Ajout IFF, IF .flag
PL65-v1.2.plm | idem v1.1 mais utilise les nouvelles instructions de la v1.1 (sauf pour les labels en minuscules, pas encore supporté)
PL65-v1.3.plm | Ajout SET, CLR, STRING, id=.reg, minuscules et _ pour les identifiants, minuscules pour les instructions
PL65-v1.4.plm | idem v1.3 mais utilise les nouvelles instructions de la v1.3
