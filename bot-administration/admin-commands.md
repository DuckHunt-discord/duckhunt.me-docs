# Commandes administrateurs

Certaines commandes sont plus compliquées que d'autres. Dans ce cas, elles sont indiquées en gras, et leurs arguments expliqués en détails après cette liste.

| Commande | Description |
| :--- | :--- |
| dh!setup | Ceci est la première commande à  utiliser après avoir invité DuckHunt dans un serveur. Elle crée les paramètres du serveur et a une aide intégrée pour vous aider. |
| dh!add\_channel | Après avoir utilisé dh!setup, utilisez cette commande sur le salon où vous voulez voir apparaître des canards pour y ajouter le bot.  |
| dh!del\_channel | Ceci supprime le bot d'un salon où il avait été ajouté. |
| dh!del\_user | Retire un utilisateur de la base de données. |
| dh!del\_user\_id | Retire un utilisateur de la base de données. Destiné aux joueurs ayant quitté le serveur. |
| dh!add\_admin | Désigne un autre administrateur du serveur comme admin pour le bot. Les utilisateurs avec la permission Administrateur sont aussi considérés comme administrateurs. |
| dh!del\_admin | Retire un admin de la liste des admins. |
| **dh!coin** | Fait apparaître un canard. |
| dh!ducks | Montre le nombre de canards qui vont apparaître, et la liste des canards sur le canal. Peut être considéré comme de la triche. |
| dh!give\_exp &lt;player&gt; &lt;amount&gt; | Donne de l'exp à un joueur. Ceci est de la riche, à ne pas confondre avec dh!send\_exp. |
| **dh!settings set &lt;parameter&gt; &lt;value&gt;** | Modifie les paramètres du serveur. Voir la [page ](edit-settings-settings-list.md)correspondante pour en savoir plus.  |
| dh!settings reset &lt;parameter&gt; | Remet un paramètre à sa valeur par défaut. Utilisez cette commande plutôt que dh!settings set pour réinitialiser des paramètres, afin d'éviter les problèmes lors des mises à jour. |
| dh!game\_ban &lt;player&gt; | Bannit un joueur du jeu. Vous ne pouvez pas bannir les admins, n’essayez pas :\) |
| dh!game\_unban &lt;player&gt; | Débannit un joueur. il pourra jouer de nouveau. |
| dh!remove\_all\_scores\_and\_stats\_on\_this\_channel | Supprime tous les scores et statistiques d'un canal. Soyez sûr de vraiment vouloir faire ça, cette action ne peut pas être annulée. |

### La commande `dh!coin`

la commande `dh!coin` fait apparaitre un canard sur le canal. Evidemment, cette commande ne peut être utilisée que sur un canal actif. 

* `dh!coin` fait apparaître un canard simple, tout à fait normal.
* `dh!coin --super-duck --life 2` fait apparaître un super-canard avec deux points de vie.
* `dh!coin --moad --life 6` fait apparaître un

   MOAD avec six points de vie.

* `dh!coin --baby-duck` fait apparaître un bébé canard.

### La commande `dh!settings`

La liste des paramètres et des valeurs est décrite en détail sur la page [Liste des paramètres](edit-settings-settings-list.md). 

