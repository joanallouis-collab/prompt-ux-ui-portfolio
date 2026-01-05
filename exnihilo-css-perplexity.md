CSS additionnel Wordpress:

Fonts:


/*titre et description page d'accueil*/

.uagb-ifb-desc{
	font-family: "bauhaus 93";
}
h1.uagb-ifb-title{
	font-family: "bauhaus 93";
}

@media (max-width: 768px) {
  h1.uagb-ifb-title {
    font-size: 60px !important; /* taille plus petite pour mobile */
  }
}

/*titre des pages*/

h1.uagb-heading-text{
	font-family: "bauhaus 93";
}


h4.uagb-ifb-title{
	color: white;
	font-family: "bauhaus 93";
}
h2.uagb-heading-text{
		color: white;
	font-family: "bauhaus 93";
}
h3.uagb-heading-text{
		color: white;
}
h1.uagb-ifb-title-prefix{
		color: white;
	font-family: "bauhaus 93";
}

.uagb-ifb-title-wrap h1.uagb-ifb-title {
    font-size: 70px; /* Desktop */
}
@media (max-width: 768px) {
    .uagb-ifb-title-wrap h1.uagb-ifb-title {
        font-size: 40px; /* Mobile */
    }
}

/* description et paragraphes des pages*/

p.uagb-ifb-desc{
	font-family: "Rubik";
}
p{
	font-family: "Rubik";
}



Modifications Woocommerce:

/* supression du fil d'ariane sans la page boutique*/

.woocommerce-breadcrumb, 
.breadcrumb-trail,
.ast-breadcrumbs {
    display: none;
}

/*Suppression de l'affichage du nombre d'article sur la page boutique*/

.woocommerce-result-count {
    display: none !important;
}


/*suppression de la loupe sur photo produit dans pages produits*/

.woocommerce-product-gallery__trigger{
	display: none !important;
}

.orderby{
	display: none !important;
}


/* Descendre le contenu de la page panier*/

.woocommerce-cart-form{
	margin-top: 120px !important;
}

/* Descendre la photo principale des pages produit*/

.single-product #content {
  padding-top: 100px;
}


/* Remonter le header pages produits*/

.entry-header {
	margin-top: 0px !important;
}


/*Supprimer l'icone panier au hover de la photo produit*/

.ast-on-card-button{
	display: none;
}

/* Baisser notification "panier mis à jour" dans page panier au clic sur "mettre à jour le panier"*/

.woocommerce-message{
	margin-top: 100px;
}

.woocommerce-error{
	margin-top: 100px;
}

/* Marges sur le contenu des pages produits WooCommerce */

.single-product .site-main {
  margin-left: 30px; /* marge gauche */
  margin-right: 30px; /* marge droite */
}



/* Format uniforme pour toutes les images du catalogue produits WooCommerce */

.woocommerce ul.products li.product img {
  width: 100% ;
  aspect-ratio: 4 / 6;    
  height: auto;             /* pour compatibilité large */
  object-fit: cover;        /* rogne l'image sans la déformer */
  background: #fff;
  display: block;
  max-width: 100%;
  min-height: 0;
}


/* Ajouter de l’espace au dessus du contenu de la page checkout WooCommerce */

.woocommerce-checkout .site-main,
.woocommerce-checkout .content-area {
  margin-top: 120px;
  padding-top: 0;
}

/* Ajouter une marge sur tout le contenu du catalogue sauf le header */

.archive.woocommerce .site-main {
  margin-left: 24px;
  margin-right: 24px;
}

/* Forcer le header catalogue à être full-width et sans marges/paddings latéraux */

.archive.woocommerce .woocommerce-products-header,
.archive.woocommerce .woocommerce-products-header > *,
.archive.woocommerce .woocommerce-products-header img {
  margin-left: 0 ;
  margin-right: 0 ;
  padding-left: 0 ;
  padding-right: 0 ;
  width: 100vw;
  max-width: 100vw;
  position: relative;
  left: 50%;
  right: 50%;
  transform: translateX(-50%);
  box-sizing: border-box;

}
