# project-1-
it's the first project for try
#Pandas with Ouazani Hadil 
#for Biochimie Master Tlemcen...06/12/2025
#the project members :
#Allouche Ikram 
#Haimour Nourhene 
#Sabri Amel 
#Sidi Ikhlef Mortada 

import pandas as pd

#Données : Séquence ADN, Longueur, Pourcentage de GC 
data ={
    "Séquence": ["ATGCGTACGTA","GCTAGCTAGGCC","TAGCGCGTAAGT","TACGATCGTA","ATGAAAGGCTT","CGTACGTAGC","TTAACCGGAT"],
    "Longueur": [12,12,12,10,11,10,10],
    "Pourcentage GC": [50,60.67,58.33,40,45.45,60,50]
}

# Création d'un DataFrame (tableau pandas)
df = pd.DataFrame(data)
print("****************Création et affichage****************")

# Affichage du tableau 
print ("Tableau des séquences ADN:")
print(df,"\n\n")

#Opérations sur les tableaux :
print("**************** Opération ****************")

#1) Sélectionner la colonne "Longueur"
longueur = df["Longueur"]
print(longueur,"\n\n")

#2) Filtrer les séquences dont la longueur supérieur à 10
print("**************** Filtrage dont la longueur ****************")
# Filtrer les séquences dont la longueur supérieur à 10 
filtred_df = df[df["Longueur"] > 10]
print(filtred_df,"\n\n")

    
