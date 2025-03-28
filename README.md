# code-app

<?php
$image_url = "https://m.ahstatic.com/is/image/accorhotels/HCM_P_0001226:11by5?fmt=webp&op_usm=1.75,0.3,2,0&resMode=sharp2&iccEmbed=true&icc=sRGB&dpr=on,1.5&wid=1459&hei=663&qlt=80"
?>
<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <title>Sofitel Marrakech informatoqui & IT | 5-étoiles </title>
    
    <style>
           /* Styles existants */
        body {
            background-image : url('<?php echo $image_url;?>');
            background-size: 100% 100%;
            background-attachment: fixed;
            
        }
       

        header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 10px 20px;
        }

        header h1 {
            font-size: 80px;
            color: maroon;
            font-weight: bold;
            margin: 0;
        }

        .ace-header-navigation__logo {
            display: flex;
            align-items: center;
            gap: 20px;
        }

        .ace-header__logo--image {
            height: 70px;
        }

        .container {
            padding: 2;
            background-color: rgba(255, 255, 255, 0.8);
            border-radius: 10px;
            margin: 220px;
        }

        .hidden-menu {
            display: none;
            position: fixed;
            top: 20px;
            left: 20px;
            background-color: rgba(255, 255, 255, 0.8);
            padding: 10px;
            border-radius: 5px;
        }

        .hidden-menu a {
            display: block;
            text-decoration: none;
            color: black;
            margin: 5px 0;
        }

        .hidden-menu-toggle {
            position: fixed;
            top: 20px;
            left: 20px;
            background-color: rgba(255, 255, 255, 0.8);
            padding: 10px;
            border-radius: 5px;
            cursor: pointer;
        }

        .hidden-menu-toggle:hover + .hidden-menu {
            display: block;
        }

        .hidden-menu:hover {
            display: block;
        }

        .form-group {
            margin-bottom: 15px;
        }

        .form-group label {
            display: block;
            margin-bottom: 5px;
        }

        .form-group input, .form-group textarea {
            width: 100%;
            padding: 8px;
            box-sizing: border-box;
        }

        .form-group button {
            padding: 10px 20px;
            background-color: maroon;
            color: white;
            border: none;
            cursor: pointer;
        }

        .form-group button:hover {
            background-color: darkred;
        }

        .produit-form {
            border: 1px solid #ccc;
            padding: 10px;
            margin-bottom: 10px;
            background-color: rgba(255, 255, 255, 0.8);
            background-size : 200px 300px ;
        }

        .fournisseur-form {
            border: 1px solid #ccc;
            padding: 10px;
            margin-top: 10px;
            background-color: rgba(255, 255, 255, 0.8);
        }

        .apropos-content {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .apropos-text {
            flex: 1;
            margin-right: 20px;
        }

        .apropos-image {
            flex: 1;
            text-align: right;
        }

        .apropos-image img {
            max-width: 100%;
            height: auto;
            border-radius: 10px;
            
        }

        /* Nouveau style pour aligner les champs sur la même ligne */
        .produit-form .form-group {
            display: flex;
            gap: 10px;
            align-items: center;
        }

        .produit-form .form-group label {
            flex: 1;
            margin-bottom: 0;
        }

        .produit-form .form-group input {
            flex: 2;
        }

        .header-menu {
            position: absolute;
            top: 50px;
            right: 80px;
        }

        .header-menu ul {
            list-style: none;
            margin: 0;
            padding: 0;
            display: flex;
            gap: 30px;
        }

        .header-menu ul li {
            display: inline;
        }

        .header-menu ul li a {
            text-decoration: none;
            color: maroon;
            font-weight: bold;
            font-size: 25px;
        }

        .header-menu ul li a:hover {
            text-decoration: underline;
        }
    </style>
</head>

    
<body class="accueil">
    
    <header>
        <!--LOGO for desktop-->
        <div class="ace-header-navigation__logo ace-header-navigation__logo--desktop">
            <div class="ace-logoheader1">
                <div class="ace-logo">
                    <div class="brand-logo ace-header__logo">
                        <a href="https://sofitel.accor.com/en.html" class="ace-header__logo--link">
                            <img src="/content/dam/brands/sof/global-marketing/brand-identity/logos/Logo%20Header.svg" alt="Sofitel" class="ace-header__logo--image"/>
                        </a>
                    </div>
                </div>
            </div>
            <div class="ace-logoheader2">
                <div class="ace-logo">
                    <div class="brand-logo ace-header__logo">
                        <a href="https://sofitel.accor.com/en.html" class="ace-header__logo--link">
                            <img src="/content/dam/brands/sof/global-marketing/brand-identity/logos/Icone%20Header.svg" alt="Cultural link" class="ace-header__logo--image"/>
                        </a>
                    </div>
                </div>
            </div>
        </div>
        <!-- Menu -->
        <nav class="header-menu">
            <ul>
                <li><a href="#accueil" onclick="changerPage('accueil')">Accueil</a></li>
                <li><a href="#apropos" onclick="changerPage('apropos')">À propos</a></li>
                <li><a href="#produit" onclick="changerPage('produit')">Produit</a></li>
                <li><a href="#contact" onclick="changerPage('contact')">Contact</a></li>
            </ul>
        </nav>
    </header>

     <!-- Menu -->
    <nav class="header-menu">
        <ul>
            <li><a href="#accueil" onclick="changerPage('accueil')">Accueil</a></li>
            <li><a href="#apropos" onclick="changerPage('apropos')">À propos</a></li>
            <li><a href="#produit" onclick="changerPage('produit')">Produit</a></li>
            <li><a href="#contact" onclick="changerPage('contact')">Contact</a></li>
        </ul>
    </nav>
    
    

    <div class="container" id="accueil">
        <h1> Sofitel Marrakech </h1>
        <p>Bienvenue sur le site de Sofitel Marrakech IT.</p>
    </div>

    <div class="container" id="apropos">
        <h2>À propos</h2>
        <div class="apropos-content">
            <div class="apropos-text">
                <p>Sofitel Hotels & Resorts est une marque d'hôtels de luxe basée à Paris, et détenue par le groupe AccorHotels. Créé en 1964, Sofitel s’est rapidement développée en France et à l’international.</p>
                <p>Email : sofitelstock@gmail.com</p>
                <p>Numéro de téléphone : 05242-28700</p>
            </div>
            <div class="apropos-image">
                <img src="Imag 2.jpg" alt="Sofitel Marrakech">
            </div>
        </div>
    </div>

    <div class="container" id="produit">
        <h2>Produit</h2>
        <div class="form-group">
            <button onclick="ajouterColonne()">+ Ajouter</button>
        </div>
        <div id="colonnes"></div>
    </div>

    <div class="container" id="contact">
        <h2>Contact</h2>
        <div style="display: flex; justify-content: space-between;">
            <div>
                <p>Email : sofitelstock@gmail.com</p>
                <p>Numéro de téléphone : 05242-28700</p>
                <p>Localisation : <a href="https://www.google.com/maps/place/Rue+Harroun+Errachid,+Quartier+de+l'hivernage,+40000+MARRAKECH,+Morocco" target="_blank">Rue Harroun Errachid, Quartier de l'hivernage, 40000 MARRAKECH, Morocco</a></p>
            </div>
            <div>
                <div class="form-group">
                    <label for="nom">Nom</label>
                    <input type="text" id="nom">
                </div>
                <div class="form-group">
                    <label for="telephone">Téléphone</label>
                    <input type="text" id="telephone">
                </div>
                <div class="form-group">
                    <label for="email">Email</label>
                    <input type="email" id="email">
                </div>
                <div class="form-group">
                    <label for="probleme">Problème</label>
                    <textarea id="probleme" rows="3"></textarea>
                </div>
                <div class="form-group">
                    <button onclick="envoyerMessage()">Connectez-nous</button>
                </div>
            </div>
        </div>
    </div>

    <script>
        function changerPage(page) {
            document.body.className = page;
        }

        window.onload = function () {
            const hash = window.location.hash.substring(1);
            if (hash) {
                changerPage(hash);
            }
        };

        let produits = [];
        let fournisseurs = [];

        function ajouterColonne() {
            const colonnes = document.getElementById('colonnes');
            const nouvelleColonne = document.createElement('div');
            nouvelleColonne.className = 'produit-form';
            nouvelleColonne.innerHTML = `
                <div class="form-group">
                    <label for="id_produit">ID Produit</label>
                    <input type="text" class="id_produit">
                </div>
                <div class="form-group">
                    <label for="nom_produit">Nom Produit</label>
                    <input type="text" class="nom_produit">
                </div>
                <div class="form-group">
                    <label for="quantite">Quantité</label>
                    <input type="text" class="quantite">
                </div>
                <div class="form-group">
                    <label for="id_fournisseur">ID Fournisseur</label>
                    <input type="text" class="id_fournisseur" onfocus="afficherFournisseur(this)">
                </div>
                <div class="form-group">
                    <label for="date_expiration">Date Expiration</label>
                    <input type="date" class="date_expiration">
                </div>
                <div class="form-group">
                    <button onclick="enregistrerProduit(this)">Enregistrer</button>
                </div>
                <div class="fournisseur-form" style="display: none;">
                    <div class="form-group">
                        <label for="nom_fournisseur">Nom Fournisseur</label>
                        <input type="text" class="nom_fournisseur">
                    </div>
                    <div class="form-group">
                        <label for="contact_fournisseur">Contact Fournisseur</label>
                        <input type="text" class="contact_fournisseur">
                    </div>
                    <div class="form-group">
                        <label for="telephone_fournisseur">Téléphone Fournisseur</label>
                        <input type="text" class="telephone_fournisseur">
                    </div>
                    <div class="form-group">
                        <label for="email_fournisseur">Email Fournisseur</label>
                        <input type="email" class="email_fournisseur">
                    </div>
                    <div class="form-group">
                        <button onclick="enregistrerFournisseur(this)">Enregistrer Fournisseur</button>
                    </div>
                </div>
            `;
            colonnes.appendChild(nouvelleColonne);
        }

        function afficherFournisseur(input) {
            const fournisseurForm = input.parentElement.parentElement.querySelector('.fournisseur-form');
            fournisseurForm.style.display = 'block';
        }

        function enregistrerProduit(bouton) {
            const formulaire = bouton.parentElement.parentElement;
            const produit = {
                id_produit: formulaire.querySelector('.id_produit').value,
                nom_produit: formulaire.querySelector('.nom_produit').value,
                quantite: formulaire.querySelector('.quantite').value,
                id_fournisseur: formulaire.querySelector('.id_fournisseur').value,
                date_expiration: formulaire.querySelector('.date_expiration').value,
            };
            produits.push(produit);
            console.log('Produit enregistré :', produit);
            alert('Produit enregistré avec succès !');
        }

        function enregistrerFournisseur(bouton) {
            const formulaire = bouton.parentElement.parentElement;
            const fournisseur = {
                nom_fournisseur: formulaire.querySelector('.nom_fournisseur').value,
                contact_fournisseur: formulaire.querySelector('.contact_fournisseur').value,
                telephone_fournisseur: formulaire.querySelector('.telephone_fournisseur').value,
                email_fournisseur: formulaire.querySelector('.email_fournisseur').value,
            };
            fournisseurs.push(fournisseur);
            console.log('Fournisseur enregistré :', fournisseur);
            alert('Fournisseur enregistré avec succès !');
        }

        function envoyerMessage() {
            const nom = document.getElementById('nom').value;
            const telephone = document.getElementById('telephone').value;
            const email = document.getElementById('email').value;
            const probleme = document.getElementById('probleme').value;
            alert(`Message envoyé par ${nom}, Téléphone: ${telephone}, Email: ${email}, Problème: ${probleme}`);
        }
    </script>
    <script>
        function changerPage(page) {
            // Masquer toutes les sections
            document.querySelectorAll('.container').forEach(section => {
                section.style.display = 'none';
            });

            // Afficher la section correspondante
            document.getElementById(page).style.display = 'block';
        }

        // Afficher la page d'accueil par défaut
        window.onload = function () {
            changerPage('accueil');
        };
    </script>
    
</body>
</html>
