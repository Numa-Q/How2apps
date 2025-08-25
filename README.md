# How2apps
Les éléments communs à toutes les apps

## erreur CORS app.js
index.html:1  Access to script at 'file:///C:/Users/....../Downloads/mini-crm-v0.0.2/app.js' from origin 'null' has been blocked by CORS policy: Cross origin requests are only supported for protocol schemes: chrome-extension, chrome-untrusted, data, edge, http, https, isolated-app.
app.js:1   Failed to load resource: net::ERR_FAILED

Pour éviter cette erreur, modifiez la façon dont le fichier app.js est chargé dans votre index.html. En retirant type="module" et en utilisant l'attribut defer à la place, le script se chargera correctement sans déclencher cette erreur de sécurité. L'application devrait maintenant fonctionner comme prévu lorsque vous ouvrez le fichier index.html.

## les modales
Toutes les modale utilisées dans l'application doivent être sur le même modele: stylées, centrées verticalement et horizontalement, fond grisé et flou.

## intéractions avec l'utilisateur: TOAST
Toutes les intéractions avec l'utilisateur doivent se faire via des toast affichés brièvement, dans une application desktop, en bas à droite de l'application.
