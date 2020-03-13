---
description: still need to edit the comment
---

# Instellingen/ lijst van instellingen

Om een instelling aan te passen moet je `dh!settings set <paramter> <waarde>` gebruiken.

Je kunt de aangepaste instellingen zien met `dh!settings modified`  

Om een instelling te resetten, gebruik `dh!settings reset <parameter>`

<table>
  <thead>
    <tr>
      <th style="text-align:left">Parameter</th>
      <th style="text-align:left">Type</th>
      <th style="text-align:left">
        <p>standaard</p>
        <p>-waarde</p>
      </th>
      <th style="text-align:left">uitleg</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left">announce_level_up</td>
      <td style="text-align:left">bool</td>
      <td style="text-align:left">True</td>
      <td style="text-align:left">Schakel het level omhoog / omlaag aankondigen aan of uit</td>
    </tr>
    <tr>
      <td style="text-align:left">bang_lag</td>
      <td style="text-align:left">float</td>
      <td style="text-align:left">0.5</td>
      <td style="text-align:left">Tijd in seconden tussen het schot van een jager en wat er gebeurt. Dit
        kan worden uitgeschakeld door het in te stellen op 0.</td>
    </tr>
    <tr>
      <td style="text-align:left">chance_to_kill_on_missed</td>
      <td style="text-align:left">integer</td>
      <td style="text-align:left">5</td>
      <td style="text-align:left">Kans in procent dat een jager iemand zal doden als hij een schot mist</td>
    </tr>
    <tr>
      <td style="text-align:left">clover_max_exp</td>
      <td style="text-align:left">integer</td>
      <td style="text-align:left">10</td>
      <td style="text-align:left">Maximale EXP bonus gegeven door een klavertje 4</td>
    </tr>
    <tr>
      <td style="text-align:left">clover_min_exp</td>
      <td style="text-align:left">integer</td>
      <td style="text-align:left">1</td>
      <td style="text-align:left">Minimale EXP bonus gegeven door een klavertje 4</td>
    </tr>
    <tr>
      <td style="text-align:left">delete_commands</td>
      <td style="text-align:left">bool</td>
      <td style="text-align:left">False</td>
      <td style="text-align:left">Anti-berichtenvloed: verwijder commandos van jagers na uitvoering</td>
    </tr>
    <tr>
      <td style="text-align:left">disable_decoys_when_ducks_are_sleeping</td>
      <td style="text-align:left">bool</td>
      <td style="text-align:left">True</td>
      <td style="text-align:left">Maak lokaas ineffectief wanneer eenden slapen (zie sleeping_ducks_start
        en sleeping_ducks_stop)</td>
    </tr>
    <tr>
      <td style="text-align:left">duck_frighten_chance</td>
      <td style="text-align:left">integer</td>
      <td style="text-align:left">5</td>
      <td style="text-align:left">Kans in procent dat een eend bang wordt en wegvliegt als een jager op
        hem schiet.</td>
    </tr>
    <tr>
      <td style="text-align:left">ducks_per_day</td>
      <td style="text-align:left">integer</td>
      <td style="text-align:left">48</td>
      <td style="text-align:left">Aantal eenden dat elke dag op een kanaal zal spawnen</td>
    </tr>
    <tr>
      <td style="text-align:left">emoji_used</td>
      <td style="text-align:left">string</td>
      <td style="text-align:left">:duck:</td>
      <td style="text-align:left">Emoji gebruikt door de bot als de emoji_ducks-instelling is ingeschakeld</td>
    </tr>
    <tr>
      <td style="text-align:left">exp_won_per_duck_killed</td>
      <td style="text-align:left">integer</td>
      <td style="text-align:left">10</td>
      <td style="text-align:left">EXP punten verdiend door een jager per gedode eend</td>
    </tr>
    <tr>
      <td style="text-align:left">killed_mentions</td>
      <td style="text-align:left">bool</td>
      <td style="text-align:left">True</td>
      <td style="text-align:left">Wissel het mensen te noemen die door andere jagers worden neergeschoten
        om. Het kan vervelend zijn, dus je kunt het hier uitschakelen.</td>
    </tr>
    <tr>
      <td style="text-align:left">language</td>
      <td style="text-align:left">string</td>
      <td style="text-align:left">en_EN</td>
      <td style="text-align:left">Taal gebruikt door de bot. Gebruik het formaat 2lettertaalcode_2LETTERLANDCODE
        (<code>fr_FR</code>, <code>hu_HU</code>, <code>en_US</code>&#x2026;). Als
        de taal niet wordt gevonden, wordt deze standaard ingesteld op Engels.
        (P.S. fr_FR is Frans, niet Fries.Fries is niet ondersteund)</td>
    </tr>
    <tr>
      <td style="text-align:left">mention_in_topscores</td>
      <td style="text-align:left">bool</td>
      <td style="text-align:left">False</td>
      <td style="text-align:left">Noem jagers in de topscores (dit verzendt GEEN meldingen). lange namen
        kunnen het scorebord breken.</td>
    </tr>
    <tr>
      <td style="text-align:left">multiplier_miss_chance</td>
      <td style="text-align:left">float</td>
      <td style="text-align:left">1</td>
      <td style="text-align:left">Verander de kans om schieten te missen. Een lagere waarde zorgt ervoor
        dat jagers minder missen, een hogere waarde zorgt ervoor dat jagers meer
        missen.</td>
    </tr>
    <tr>
      <td style="text-align:left">pm_most_messages</td>
      <td style="text-align:left">bool</td>
      <td style="text-align:left">False</td>
      <td style="text-align:left">Stuur niet-essenti&#xEB;le antwoorden per DM naar een jager (!reload,
        !shop ...)</td>
    </tr>
    <tr>
      <td style="text-align:left">prefix</td>
      <td style="text-align:left">string</td>
      <td style="text-align:left">!</td>
      <td style="text-align:left">Voorvoegsel gebruikt door de bot. Als DuckHunt-commandos conflicteren
        met een andere bot, kunt u deze hier wijzigen. Ongeacht dzal DuckHunt altijd
        reageren op het voorvoegsel dh!</td>
    </tr>
    <tr>
      <td style="text-align:left">randomize_mechanical_ducks</td>
      <td style="text-align:left">integer</td>
      <td style="text-align:left">0</td>
      <td style="text-align:left">Parameter met 3 niveaus. Als het op 0 is ingesteld, heeft een mechanische
        eend een vast gekwaak. Indien ingesteld op 1, wordt zijn kwaken willekeurig.
        Op 2 is de mechanische eend niet te onderscheiden van een normale eend.</td>
    </tr>
    <tr>
      <td style="text-align:left">show_super_ducks_life</td>
      <td style="text-align:left">bool</td>
      <td style="text-align:left">False</td>
      <td style="text-align:left">Toon het leven van supereenden wanneer ze niet worden gedood, maar wel
        zijn geraakt.</td>
    </tr>
    <tr>
      <td style="text-align:left">sleeping_ducks_start</td>
      <td style="text-align:left">integer</td>
      <td style="text-align:left">0</td>
      <td style="text-align:left">Gebruikt met sleeping_ducks_stop om een &#x200B;&#x200B;interval te defini&#xEB;ren
        met behulp van 24-uurs tijd, waar de eenden niet zullen spawnen. De ducks_per_day
        instelling wordt ALSNOG waargemaakt. Je mag alleen uren invoeren in UTC.
        Voorbeeld: <code>dh!settings set sleeping_ducks_start 22</code>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">sleeping_ducks_stop</td>
      <td style="text-align:left">integer</td>
      <td style="text-align:left">0</td>
      <td style="text-align:left">Zie sleeping_ducks_start. Voorbeeld:<code>dh!settings set sleeping_ducks_stop 10</code>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">ducks_chance</td>
      <td style="text-align:left">integer</td>
      <td style="text-align:left">100</td>
      <td style="text-align:left">Kans dat een eend die spawnt als normale eend. (dit is een gewogen kanssysteem).</td>
    </tr>
    <tr>
      <td style="text-align:left">super_ducks_chance</td>
      <td style="text-align:left">integer</td>
      <td style="text-align:left">5</td>
      <td style="text-align:left">Kans op een eend die spawnt als supereend</td>
    </tr>
    <tr>
      <td style="text-align:left">baby_ducks_chance</td>
      <td style="text-align:left">integer</td>
      <td style="text-align:left">2</td>
      <td style="text-align:left">Kans op een eend die spawnt als babyeend</td>
    </tr>
    <tr>
      <td style="text-align:left">mother_of_all_ducks_chance</td>
      <td style="text-align:left">integer</td>
      <td style="text-align:left">1</td>
      <td style="text-align:left">Kans op een eend die spawnt als Moeder Van Alle Eenden (genoemd als MOAD
        in spel-jargon)</td>
    </tr>
    <tr>
      <td style="text-align:left">super_ducks_exp_multiplier</td>
      <td style="text-align:left">float</td>
      <td style="text-align:left">1.1</td>
      <td style="text-align:left">Verandert de super ducks EXP variabele in de volgende formule; (vraag
        de eigenaar als je het niet snapt)</td>
    </tr>
    <tr>
      <td style="text-align:left">super_ducks_maxlife</td>
      <td style="text-align:left">integer</td>
      <td style="text-align:left">7</td>
      <td style="text-align:left">Maximale levens van een supereend</td>
    </tr>
    <tr>
      <td style="text-align:left">super_ducks_minlife</td>
      <td style="text-align:left">integer</td>
      <td style="text-align:left">3</td>
      <td style="text-align:left">Minimale levens van een supereend</td>
    </tr>
    <tr>
      <td style="text-align:left">tax_on_user_give</td>
      <td style="text-align:left">integer</td>
      <td style="text-align:left">5</td>
      <td style="text-align:left">Percentage van exp dat als belasting zal worden ge-int wanneer een speler
        send_exp gebruikt. Dit kan worden uitgeschakeld door het in te stellen
        op 0.</td>
    </tr>
    <tr>
      <td style="text-align:left">time_before_ducks_leave</td>
      <td style="text-align:left">integer</td>
      <td style="text-align:left">660</td>
      <td style="text-align:left">Tijd in seconden voordat een eend zich verveelt als hij niet wordt gedood.</td>
    </tr>
    <tr>
      <td style="text-align:left">tts_ducks</td>
      <td style="text-align:left">bool</td>
      <td style="text-align:left">False</td>
      <td style="text-align:left">Probeert /tts te gebruiken als er eenden verschijnen. Experimenteel. (DEFUNCT)</td>
    </tr>
    <tr>
      <td style="text-align:left">user_can_give_exp</td>
      <td style="text-align:left">bool</td>
      <td style="text-align:left">True</td>
      <td style="text-align:left">Sta gebruikers toe om elkaar ervaringspunten te sturen met het commando <code>dh!send_exp</code>.</td>
    </tr>
    <tr>
      <td style="text-align:left">users_can_find_objects</td>
      <td style="text-align:left">bool</td>
      <td style="text-align:left">True</td>
      <td style="text-align:left">Sta gebruikers toe objecten in struiken te vinden. Sommige objecten zijn
        afval, sommige objecten zijn behulpzaam.</td>
    </tr>
  </tbody>
</table>