# Landraw Boutique

## Description du Projet

Ce projet est une page responsive pour une boutique en ligne. La page comprend un en-tête, une section produit et un pied de page. Le design est visuellement attrayant et s'adapte bien aux différentes tailles d'écran grâce à l'utilisation de Bootstrap.

## Structure du Projet

- `index.html` : Contient la structure HTML de la page, incluant l'en-tête, la section produit et le pied de page.
- `styles.css` : Contient les styles CSS personnalisés pour la page.
- `img/` : Contient les images utilisées dans le projet.


## Explication du Code

### index.html

<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Boutique en ligne</title>
    <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/css/bootstrap.min.css">
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <!-- En-tête -->
    <header class="bg-dark text-white p-3">
        <div class="container">
            <div class="d-flex justify-content-between align-items-center">
                <h1 class="h3">Landraw Boutique</h1>
                <nav>
                    <ul class="nav">
                        <li class="nav-item"><a class="nav-link text-white" href="#home">Accueil</a></li>
                        <li class="nav-item"><a class="nav-link text-white" href="#products">Produits</a></li>
                        <li class="nav-item"><a class="nav-link text-white" href="#contact">Contact</a></li>
                    </ul>
                </nav>
            </div>
        </div>
    </header>

    <!-- Section produit -->
    <section id="products" class="py-5">
        <div class="container">
            <h2 class="text-center mb-5">Nos Produits</h2>
            <div class="row">
                <div class="col-md-3 col-sm-6 mb-4">
                    <div class="card h-100">
                        <img src="img/appareil_1.jpg" class="card-img-top" alt="Appareil Photo 1">
                        <div class="card-body">
                            <h5 class="card-title">Canon QL17</h5>
                            <p class="card-text">Le canon QL17 est un appareil photo.</p>
                            <a href="#" class="btn btn-custom">Acheter maintenant</a>
                        </div>
                    </div>
                </div>
                <div class="col-md-3 col-sm-6 mb-4">
                    <div class="card h-100">
                        <img src="img/objectif_1.jpg" class="card-img-top" alt="Objectif 2">
                        <div class="card-body">
                            <h5 class="card-title">Objectif 18-55mm</h5>
                            <p class="card-text">Zoom polyvalent très réactif et solide.</p>
                            <a href="#" class="btn btn-custom">Acheter maintenant</a>
                        </div>
                    </div>
                </div>
                <div class="col-md-3 col-sm-6 mb-4">
                    <div class="card h-100">
                        <img src="img/appareil_2.jpg" class="card-img-top" alt="Appareil Photo 2">
                        <div class="card-body">
                            <h5 class="card-title">Lumix S5</h5>
                            <p class="card-text">Le Lumix S5 est un appareil photo.</p>
                            <a href="#" class="btn btn-custom">Acheter maintenant</a>
                        </div>
                    </div>
                </div>
                <div class="col-md-3 col-sm-6 mb-4">
                    <div class="card h-100">
                        <img src="img/objectif_2.jpg" class="card-img-top" alt="Objectif 2">
                        <div class="card-body">
                            <h5 class="card-title">Canon 70-200mm</h5>
                            <p class="card-text">Zoom polyvalent très réactif et solide.</p>
                            <a href="#" class="btn btn-custom">Acheter maintenant</a>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Pied de page -->
    <footer class="bg-dark text-white p-4 text-center">
        <div class="container">
            <p>&copy; 2024 Landraw. Tous droits réservés.</p>
        </div>
    </footer>

    <script src="https://code.jquery.com/jquery-3.5.1.slim.min.js"></script>
    <script src="https://cdn.jsdelivr.net/npm/@popperjs/core@2.5.3/dist/umd/popper.min.js"></script>
    <script src="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/js/bootstrap.min.js"></script>
</body>
</html>


## styles.css

/* Global Styles */
body {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
    background-color: #f4f4f4;
}

header {
    background-color: #343a40;
}

header h1 {
    margin: 0;
}

header nav ul {
    list-style-type: none;
    margin: 0;
    padding: 0;
    display: flex;
}

header nav ul li {
    margin-left: 20px;
}

header nav ul li a {
    color: white;
    text-decoration: none;
}

header nav ul li a:hover {
    text-decoration: underline;
}

section#products {
    background-color: #ffffff;
    padding: 60px 0;
}

section#products h2 {
    font-size: 2.5rem;
    margin-bottom: 40px;
}

.card img {
    height: 200px;
    object-fit: cover;
}

footer {
    background-color: #343a40;
    color: white;
    padding: 20px 0;
}

/* Button Styles */
.btn-custom {
    background-color: #ff0000;
    color: white;
    border: none;
}

.btn-custom:hover {
    background-color: #cc0000;
    color: white;
}

/* Responsive Design */
@media (max-width: 768px) {
    header nav ul {
        flex-direction: column;
        align-items: center;
    }

    header nav ul li {
        margin-left: 0;
        margin-bottom: 10px;
    }

    .card img {
        height: auto;
    }
}


## Choix de conception
En-tête : L'en-tête contient le nom de la boutique et un menu de navigation. Le menu de navigation utilise les classes Bootstrap pour s'assurer qu'il soit réactif et bien aligné.
Section produit : La section produit utilise des cartes Bootstrap pour afficher les produits de manière organisée. Chaque carte produit contient une image, un titre, une description et un bouton "Acheter maintenant".

Pied de page : Le pied de page est simple et contient une ligne de copyright.
Boutons : Les boutons "Acheter maintenant" sont stylisés en rouge pour attirer l'attention des utilisateurs.
Responsive Design : Des requêtes multimédias sont utilisées pour s'assurer que la mise en page s'adapte correctement aux écrans plus petits.
