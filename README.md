French version
# Login-avec-authentification-email
Système de connexion avec PHP, SQL, Bootstrap. 
Après une nouvelle inscription, l'utilisateur reçoit un e-mail qu'il doit confirmer pour terminer l'inscription. Il peut ensuite se connecter normalement.

L'utilisateur s'inscrit et reçoit un e-mail avec un lien de confirmation.

Le nouvel utilisateur ne peut se connecter qu'après confirmation.


L'utilisateur peut modifier son mot de passe s'il l'a oublié (après une tentative d'inscription ratée).

Il reçoit un lien par e-mail pour modifier son mot de passe.


- PHP Mailer et Gmail SMTP (librairie PHPMailer : https://sourceforge.net/projects/phpmailer/ )
- Grille Bootstrap et formulaires 
- Validation de la saisie (lors d'une nouvelle inscription) avec jQuery 
- Banque de données SQL : login.sql
- Images d'arrière-plan de : https://github.com/BlackrockDigital/startbootstrap by davidtmiller


<p align="centre">
  <img src="https://s19.postimg.org/vc7ghhter/index.png" width="280"/>
  <img src="https://s19.postimg.org/5bgadmsrn/neu_Anmelden.png" width="280"/>
  <img src="https://s19.postimg.org/eutni37s3/home.png" width="280"/>
</p>
<p align="center">
  <img src="https://s19.postimg.org/rie08cc2r/fpasswort.png" width="280"/>
  <img src="https://s19.postimg.org/hmcx8p6ar/resetpass.png" width="280"/>
  <img src="https://s19.postimg.org/id5neh8o3/resetpass2.png" width="280"/>
</p>

Mise à jour 20.01.17 Validation de la saisie avec Javascript (alternativement possible avec Parsley.js)
<p align="gauche">
  <img src="https://s19.postimg.org/8ux66bp5v/signup_valid.png" width="280"/>
</p>

Il manque encore le hashing du mot de passe (actuellement avec Md5).

Mise à jour 23.02.17 Bugs :
-Version obsolète de PHP Mailer : Message d'erreur lors de la nouvelle connexion de l'utilisateur "preg_replace() : The /e modifier is no longer supported".
-ligne d'objet manquante dans le mail de confirmation


<h2> Comment installer </h2>
- télécharger, décompresser, base de données : login.sql
- dans User Class PHP Mailer paramètres : Saisir l'email et le mot de passe
