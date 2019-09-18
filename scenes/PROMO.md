# intro

`SceneSetup.intro();`

# intro-play-button

(...51)

[PLAY!](#intro-start) `publish("intro-to-game-1"); Game.OVERRIDE_CHOICE_LINE=true;`

# intro-start

(...500)

`clearText()`

n3: Avant qu'on commence, a quelle vitesse veux-*tu* lire?

`publish("show_options_bottom")`

# intro-start-2

n3: Maintenant, commençons notre histoire...

```
publish("hide_tabs");
clearText();
```

(...1000)

`publish("intro-to-game-2")`

n2: CECI EST UN HUMAIN

(...600)

`clearText()`

(...300)

`publish("intro-to-game-3")`

# act1

```
SceneSetup.act1();
publish("hide_tabs");
music('battle', {volume:0.5});
```

(...300)

n: ET CECI EST L'ANXIÉTÉ DE CET HUMAIN

n: _TU_ EST L'ANXIÉTÉ

(#act1_normal)


# act1_normal

```
hong({body:"putaway"});
sfx("rustle");
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: Non. Je m'en fous, j'écoute pas. Je vais aller sur mon téléphone.

```
sfx("rustle2");
hong({body:"phone1", mouth:"neutral", eyes:"neutral"})
```

n: TON TRAVAIL EST DE PROTÉGER TON HUMAN DU *DANGER*

`bb({eyes:"look", mouth:"small_lock", body:"fear"})`

b: Oh! Tu es en train encore de passer ta vie sur Twitter!

```
bb({eyes:"normal", mouth:"normal", body:"normal"});
hong({eyes:"annoyed"});
```

h: Ouais, je me demande pourquoi je me pose pas pour écouter mes pensées plus souvent.

`hong({eyes:"neutral"});`

n: VITE, PRÉVIENS-LE D'UN *DANGER!*

```
bb({eyes:"look"});
```

[Oh non, regarde cet horrible article de news!](#act1d_news)

[Oh non, est-ce que ce tweet est à propos de *nous?*](#act1d_subtweet)

[Eh, un GIF d'un chat qui boit du lait](#act1d_milk)

# act1d_milk

`hong({mouth:"smile", eyes:"surprise"});`

h: Ah ouais c'est mignon, je--

```
hong({mouth:"shock", eyes:"shock"});
bb({body:"scream"});
Game.OVERRIDE_TEXT_SPEED = 1.8;
```

b: LES CHATS NE DIGÈRENT PAS LE LAIT ET ON EST UNE HORRIBLE PERSONNE POUR APPRÉCIER ÇA

(...200)

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
attack("20p", "bad");
publish("hp_show");
```



