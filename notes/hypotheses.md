# Audit Dataset

Nombre de lignes :
180371

Nombre de colonnes :
43

Valeurs manquantes :
0

Doublons :
61522 (~34%)

Colonnes catégorielles :
- proto
- service
- state

Colonnes numériques :
40

Colonnes constantes :
0

Classes déséquilibrées :
Oui

Premières hypothèses :

H1 : proto, service et state seront importantes.

H2 : Les variables numériques contiennent probablement
des signatures réseau discriminantes.

H3 : Les classes rares (Worms, Shellcode, Backdoor,
Analysis) seront les plus difficiles à prédire.

H4 : Les doublons devront être étudiés avant toute suppression.

H5 : LightGBM et CatBoost devraient être de très bons candidats.

H5 : Certaines attaques semblent produire des signatures réseau extrêmement répétitives.