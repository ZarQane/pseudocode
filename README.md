Début
    ## Supposons que les valeurs d'argent et de prix sont déjà connues
    argent <- 12.47
    prix <- 1.14

    ## Vérifier que argent et prix sont strictement supérieurs à 0
    Si argent <= 0 OU prix <= 0
        Afficher "Montant et prix doivent être supérieurs à 0"
        Arrêter
    Fin Si

    ## Initialiser le nombre de bonbons à zéro
    bonbons <- 0

    ## Tant que l'argent est suffisant pour acheter au moins un bonbon
    Tant que argent >= prix
        ## Acheter un bonbon
        bonbons <- bonbons + 1
        ## Soustraire le prix d'un bonbon de l'argent disponible
        argent <- argent - prix
    Fin tant que

    ## Afficher le nombre maximum de bonbons que l'on peut acheter
    Afficher bonbons
Fin
