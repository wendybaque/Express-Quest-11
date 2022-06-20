# 💪 Challenge
* 1. Tu vas d'abord modifier la méthode POST dans routes/movies.js. A l'intérieur de cette fonction, récupére le cookie de la requête de l'utilisateur et récupére le token (astuce : lis le Cookie Parser )

* 2. Utilise ce token pour obtenir l'identifiant de l'utilisateur. (tu devras peut-être ajouter une nouvelle fonction findByToken() dans ton modèle).

* 3. Ajoute un champ user_id dans la table movies. Il s'agira d'une clé étrangère faisant référence à l'"id" de la table "users".

* 4. Si un utilisateur est trouvé, crée le film et définis user_id comme étant son propriétaire. Si aucun utilisateur n'est trouvé, retourne un status 401.

* 5. Modifie la méthode GET dans routes/movies.js : Si un token est fourni, il ne doit retourner que les films créés par cet utilisateur.

# 🧐 Critères de validation
 * Ton application lit les tokens en utilisant un cookie
 * Tu peux créer des films et définir le propriétaire
 * Tu ne peux obtenir que les films que tu as créés
