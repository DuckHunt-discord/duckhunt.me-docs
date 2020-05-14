# Changer les paramètres / Liste des paramètres

Pour définir un paramètre, utilisez `dh!settings set <paramètre> <valeur>`

Vous pouvez voir les paramètres ayant été modifiés avec la commande `dh!settings modified`

Pour réinitialiser un paramètre à sa valeur par défaut, vous pouvez utiliser `dh!settings reset <paramètre>`

Note : Un booléen est un type de variable pouvant être défini par `true` ou `false`. `true` correspond à "oui" ou "vrai", et `false` correspond à "non" ou "faux". Par exemple, `true` sur `announce_level_up` veut dire que les messages de montée de niveau seront envoyés.

<table>
  <thead>
    <tr>
      <th style="text-align:left">Param&#xE8;tre</th>
      <th style="text-align:left">Type</th>
      <th style="text-align:left">Valeur par d&#xE9;faut</th>
      <th style="text-align:left">Commentaire</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left">announce_level_up</td>
      <td style="text-align:left">bool&#xE9;en</td>
      <td style="text-align:left">True</td>
      <td style="text-align:left">Activer ou pas les messages de mont&#xE9;e de niveau.</td>
    </tr>
    <tr>
      <td style="text-align:left">bang_lag</td>
      <td style="text-align:left">d&#xE9;cimal</td>
      <td style="text-align:left">0.5</td>
      <td style="text-align:left">Temps en seconde entre le tir et la r&#xE9;ponse du bot. Peut &#xEA;tre
        mis &#xE0; 0 pour &#xEA;tre d&#xE9;sactiv&#xE9;.</td>
    </tr>
    <tr>
      <td style="text-align:left">chance_to_kill_on_missed</td>
      <td style="text-align:left">entier</td>
      <td style="text-align:left">5</td>
      <td style="text-align:left">Probabilit&#xE9; en pourcentage qu&#x2019;un chasseur tue quelqu&#x2019;un
        lors d&#x2019;un tir rat&#xE9;.</td>
    </tr>
    <tr>
      <td style="text-align:left">clover_max_exp</td>
      <td style="text-align:left">entier</td>
      <td style="text-align:left">10</td>
      <td style="text-align:left">Exp&#xE9;rience bonus maximale donn&#xE9;e par un tr&#xE8;fle</td>
    </tr>
    <tr>
      <td style="text-align:left">clover_min_exp</td>
      <td style="text-align:left">entier</td>
      <td style="text-align:left">1</td>
      <td style="text-align:left">Exp&#xE9;rience bonus minimale donn&#xE9;e par un tr&#xE8;fle</td>
    </tr>
    <tr>
      <td style="text-align:left">delete_commands</td>
      <td style="text-align:left">bool&#xE9;en</td>
      <td style="text-align:left">True</td>
      <td style="text-align:left">Param&#xE8;tre anti-spam : supprimer les messages contenant les commandes</td>
    </tr>
    <tr>
      <td style="text-align:left">disable_decoys_when_ducks_are_sleeping</td>
      <td style="text-align:left">bool&#xE9;en</td>
      <td style="text-align:left">True</td>
      <td style="text-align:left">Emp&#xEA;che l&#x2019;utilisation de leurres quand les canards dorment.
        (Voir les param&#xE8;tres <code>sleeping_ducks_start</code> et <code>sleeping_ducks_stop</code>)</td>
    </tr>
    <tr>
      <td style="text-align:left">duck_frighten_chance</td>
      <td style="text-align:left">entier</td>
      <td style="text-align:left">5</td>
      <td style="text-align:left">Probabilit&#xE9; qu&#x2019;un canard s&#x2019;enfuie lors d&#x2019;un
        tir, en pourcentage.</td>
    </tr>
    <tr>
      <td style="text-align:left">ducks_per_day</td>
      <td style="text-align:left">entier</td>
      <td style="text-align:left">48</td>
      <td style="text-align:left">Nombre de canards par jour dans un salon textuel.</td>
    </tr>
    <tr>
      <td style="text-align:left">emoji_used</td>
      <td style="text-align:left">texte</td>
      <td style="text-align:left">:duck:</td>
      <td style="text-align:left">Emoji utilis&#xE9; si le param&#xE8;tre <code>emoji_ducks</code> est activ&#xE9;.</td>
    </tr>
    <tr>
      <td style="text-align:left">exp_won_per_duck_killed</td>
      <td style="text-align:left">entier</td>
      <td style="text-align:left">10</td>
      <td style="text-align:left">Points d&#x2019;exp&#xE9;rience gagn&#xE9;s lorsque un chasseur a tu&#xE9;
        un canard.</td>
    </tr>
    <tr>
      <td style="text-align:left">killed_mentions</td>
      <td style="text-align:left">bool&#xE9;en</td>
      <td style="text-align:left">True</td>
      <td style="text-align:left">Mentionner ou pas les personnes se faisant tirer dessus par un chasseur.</td>
    </tr>
    <tr>
      <td style="text-align:left">language</td>
      <td style="text-align:left">texte</td>
      <td style="text-align:left">en_EN</td>
      <td style="text-align:left">Langue utilis&#xE9;e par le bot. Utilisez le format codedulangage_CODEDUPAYS
        (<code>fr_FR </code>pour le fran&#xE7;ais de France, <code>hu_HU</code>, <code>en_US</code> pour
        l&apos;anglais am&#xE9;ricain&#x2026;). Si le langage n&apos;est pas trouv&#xE9;,
        le serveur se mettra par d&#xE9;faut en anglais.</td>
    </tr>
    <tr>
      <td style="text-align:left">mention_in_topscores</td>
      <td style="text-align:left">bool&#xE9;en</td>
      <td style="text-align:left">False</td>
      <td style="text-align:left">Mentionner les chasseurs dans le tableau de score (Cela ne notifiera personne).</td>
    </tr>
    <tr>
      <td style="text-align:left">multiplier_miss_chance</td>
      <td style="text-align:left">d&#xE9;cimal</td>
      <td style="text-align:left">1</td>
      <td style="text-align:left">Changer la probabilit&#xE9; pour un chasseur de rater son tir. Plus la
        valeur est &#xE9;lev&#xE9;e, plus la probabilit&#xE9; de rater est haute.</td>
    </tr>
    <tr>
      <td style="text-align:left">pm_most_messages</td>
      <td style="text-align:left">bool&#xE9;en</td>
      <td style="text-align:left">False</td>
      <td style="text-align:left">Envoyer les messages non-importants par message priv&#xE9; (rechargement,
        achats&#x2026;)</td>
    </tr>
    <tr>
      <td style="text-align:left">prefix</td>
      <td style="text-align:left">texte</td>
      <td style="text-align:left">!</td>
      <td style="text-align:left">Pr&#xE9;fixe utilis&#xE9;. Si un autre bot utilise le m&#xEA;me pr&#xE9;fixe
        que DuckHunt, vous pouvez le changer. Peu importe le param&#xE8;tre, le
        bot r&#xE9;pondra tout le temps au pr&#xE9;fixe <code>dh!</code>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">randomize_mechanical_ducks</td>
      <td style="text-align:left">entier</td>
      <td style="text-align:left">0</td>
      <td style="text-align:left">Param&#xE8;tre &#xE0; trois niveaux. &#xC0; 0, un canard m&#xE9;canique
        sera totalement unique. &#xC0; 1, le cri du canard m&#xE9;canique sera
        comme un canard normal. &#xC0; 2, le canard m&#xE9;canique sera exactement
        comme un canard normal.</td>
    </tr>
    <tr>
      <td style="text-align:left">show_super_ducks_life</td>
      <td style="text-align:left">bool&#xE9;en</td>
      <td style="text-align:left">False</td>
      <td style="text-align:left">Affiche la vie des super canards lorsqu&#x2019;ils ne sont pas tu&#xE9;s</td>
    </tr>
    <tr>
      <td style="text-align:left">sleeping_ducks_start</td>
      <td style="text-align:left">entier</td>
      <td style="text-align:left">0</td>
      <td style="text-align:left">
        <p>&#xC0; utiliser avec <code>sleeping_ducks_stop</code>, pour d&#xE9;finir
          une intervalle avec le syst&#xE8;me horaire militaire (format 24) o&#xF9;
          les canard dormiront, et donc n&#x2019;appara&#xEE;tront pas. Le param&#xE8;tre
          &#xAB; ducks_per_day &#xBB; sera toujours pris en compte. Important : L&#x2019;heure
          utilis&#xE9; par le bot est en UTC+0. Tapez la commande dh!time pour voir
          l&#x2019;heure actuelle pour le bot.
          <br />Exemple :</p>
        <p><code>dh!settings set sleeping_ducks_start 22</code>
        </p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">sleeping_ducks_stop</td>
      <td style="text-align:left">entier</td>
      <td style="text-align:left">0</td>
      <td style="text-align:left">Voir le param&#xE8;tre <code>sleeping_ducks_start</code>. Exemple : <code>dh!settings set sleeping_ducks_stop 10</code>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">ducks_chance</td>
      <td style="text-align:left">entier</td>
      <td style="text-align:left">100</td>
      <td style="text-align:left">Probabilit&#xE9; qu&apos;un nouveau canard soit normal. (Plus la valeur
        est grande, plus il y a des chances que ce soit ce type de canard. 0 veut
        dire qu&apos;il n&#x2019;appara&#xEE;tra jamais.)</td>
    </tr>
    <tr>
      <td style="text-align:left">super_ducks_chance</td>
      <td style="text-align:left">entier</td>
      <td style="text-align:left">5</td>
      <td style="text-align:left">Probabilit&#xE9; qu&apos;un nouveau canard soit un super canard.</td>
    </tr>
    <tr>
      <td style="text-align:left">baby_ducks_chance</td>
      <td style="text-align:left">entier</td>
      <td style="text-align:left">2</td>
      <td style="text-align:left">Probabilit&#xE9; qu&apos;un nouveau canard soit un b&#xE9;b&#xE9; canard.</td>
    </tr>
    <tr>
      <td style="text-align:left">mother_of_all_ducks_chance</td>
      <td style="text-align:left">entier</td>
      <td style="text-align:left">1</td>
      <td style="text-align:left">Probabilit&#xE9; qu&apos;un nouveau canard soit la M&#xE8;re de tous les
        canards.</td>
    </tr>
    <tr>
      <td style="text-align:left">super_ducks_exp_multiplier</td>
      <td style="text-align:left">d&#xE9;cimal</td>
      <td style="text-align:left">1.1</td>
      <td style="text-align:left">
        <p>L&#x2019;exp&#xE9;rience gagn&#xE9;e quand un super canard est tu&#xE9;
          se calcule avec la formule</p>
        <p>Voir aussi le param&#xE8;tre <code>exp_won_per_duck_killed</code>, l&apos;exp&#xE9;rience
          gagn&#xE9;e lorsque un chasseur tue un canard.</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">super_ducks_maxlife</td>
      <td style="text-align:left">entier</td>
      <td style="text-align:left">7</td>
      <td style="text-align:left">Vie maximale d&#x2019;un super canard.</td>
    </tr>
    <tr>
      <td style="text-align:left">super_ducks_minlife</td>
      <td style="text-align:left">entier</td>
      <td style="text-align:left">3</td>
      <td style="text-align:left">Vie minimale d&#x2019;un super canard.</td>
    </tr>
    <tr>
      <td style="text-align:left">tax_on_user_give</td>
      <td style="text-align:left">entier</td>
      <td style="text-align:left">5</td>
      <td style="text-align:left">Pourcentage de points d&#x2019;exp&#xE9;rience supprim&#xE9; lorsque un
        joueur en envoi avec la commande <code>dh!send_exp</code>. Mettre &#xE0;
        0 pour d&#xE9;sactiver la taxe.</td>
    </tr>
    <tr>
      <td style="text-align:left">time_before_ducks_leave</td>
      <td style="text-align:left">entier</td>
      <td style="text-align:left">660</td>
      <td style="text-align:left">Temps en secondes avant qu&#x2019;un canard parte s&#x2019;il n&#x2019;est
        pas tu&#xE9;.</td>
    </tr>
    <tr>
      <td style="text-align:left">tts_ducks</td>
      <td style="text-align:left">bool&#xE9;en</td>
      <td style="text-align:left">False</td>
      <td style="text-align:left">Essaye de parler avec la commande <code>/tts</code> quand un canard appara&#xEE;t.
        Param&#xE8;tre exp&#xE9;rimental.</td>
    </tr>
    <tr>
      <td style="text-align:left">user_can_give_exp</td>
      <td style="text-align:left">bool&#xE9;en</td>
      <td style="text-align:left">True</td>
      <td style="text-align:left">D&#xE9;fini si la commande <code>dh!send_exp</code>, qui permet d&#x2019;envoyer
        des points d&#x2019;exp&#xE9;rience, est autoris&#xE9;e.</td>
    </tr>
    <tr>
      <td style="text-align:left">users_can_find_objects</td>
      <td style="text-align:left">bool&#xE9;en</td>
      <td style="text-align:left">True</td>
      <td style="text-align:left">D&#xE9;fini si des objets peuvent &#xEA;tre trouv&#xE9;s al&#xE9;atoirement
        dans un buisson quand un chasseur tue un canard.</td>
    </tr>
  </tbody>
</table>