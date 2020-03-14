# Admin commandos

Sommige commandos zijn meer complex dan anderen. Als dat zo is zullen deze in dikgedrukte letters staan. Er staan onder de lijst uitgebreid uitleg over deze commandos.

| Commando | uitleg |
| :--- | :--- |
| dh!setup | Dit is het eerste commando dat je moet gebruiken nadat je DuckHunt op een server hebt uitgenodigd. Het creëert de serverinstellingen en heeft een configuratiewizard om het jou gemakkelijker te maken. |
| dh!add\_channel | Gebruik dit na `dh!setup`dit commando op de kanalen waarin jij eenden wilt laten verschijnen.. |
| dh!del\_channel | Dit schakelt een kanaal uit dat is toegevoegd door `dh!add_channel`. |
| dh!del\_user | Dit verwijdert een gebruiker uit de database. |
| dh!del\_user\_id | zie `dh!del_user`, maar dan voor gebruikers die de server verlaten hebben |
| dh!add\_admin | Stel een ander persoon in als beheerder. Notitie: gebruikers met de admin machtiging ook als beheerders worden beschouwd. |
| dh!del\_admin | Verwijdert een serverbeheerder uit de beheerderslijst. |
| **dh!coin** | Forceert een eend om te spawnen. |
| dh!ducks | Toont het aantal eenden dat vandaag zal spawnen en de lijst met eenden op het kanaal. Het kan worden beschouwd als valsspelen. |
| dh!give\_exp &lt;player&gt; &lt;amount&gt; | Geeft een speler wat exp-punten. Dit is een cheat, niet te verwarren met `dh!send_exp.` |
| **dh!settings set &lt;parameter&gt; &lt;value&gt;** | Wijzig serverinstellingen. Je kunt naar de pagina [instellingen ](edit-settings-settings-list.md)gaan voor meer informatie. |
| dh!settings reset &lt;parameter&gt; | Reset een instelling naar de standaardwaarde. Gebruik dit commando, niet `dh!settings`, om parameters opnieuw in te stellen, anders kan dat problemen veroorzaken met bot-updates. |
| dh!game\_ban &lt;player&gt; | Ban een speler uit het spel. Je kunt beheerders niet bannen, dus probeer het niet :\) |
| dh!game\_unban &lt;player&gt; | un-ban een speler uit het spel. Ze zullen weer kunnen spelen. |
| dh!remove\_all\_scores\_and\_stats\_on\_this\_channel | Verwijdert de kanaalscores en statistieken van het kanaal. **Zorg ervoor dat je dit echt wilt doen!** Je kunt dit **niet** ongedaan maken. |

### Het "coin" commando

Het coin commando \(`dh!coin`\) spawnt een eend in het huidige kanaal. Dit kan alleen gedaan worden in kanalen die toegevoegd zijn med `dh!add_channel`. 

* `dh!coin` spawnt een simpele, normale eend.
* `dh!coin --super-duck --life 2` spawnt een supereend met 2 levens.
* `dh!coin --moad --life 6` spawnt een [MOAD](../players-guide/types-of-ducks.md) met 6 levens.
* `dh!coin --baby-duck` spawnt een baby eend.

### Het instellings gerelateerde commando

De lijst van instellingen en waarden ervan kun je vinden op de pagina [lijst van instellingen](edit-settings-settings-list.md).

