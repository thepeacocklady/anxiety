# intro

`SceneSetup.intro();`

# intro-play-button

(...51)

[HRÁT!](#intro-start) `publish("intro-to-game-1"); Game.OVERRIDE_CHOICE_LINE=true;`

# intro-start

(...500)

`clearText()`

n3: Předtím, než začneme, *rozhodni se* jak chceš číst.

`publish("show_options_bottom")`

# intro-start-2

n3: Náš příběh začíná...

```
publish("hide_tabs");
clearText();
```

(...1000)

`publish("intro-to-game-2")`

n2: TOHLE JE ČLOVĚK

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

n: A TOHLE JE JEHO ÚZKOST

n: _TY_ JSI TA ÚZKOST

(#act1_normal)


# act1_normal

```
hong({body:"putaway"});
sfx("rustle");
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: Ne. Nein, nada, niet, neposlouchám. Radši zkouknu mobil.

```
sfx("rustle2");
hong({body:"phone1", mouth:"neutral", eyes:"neutral"})
```

n: TVŮJ ÚKOL JE CHRÁNIT TVÉHO ČLOVĚKA PŘED *OHROŽENÍM*

`bb({eyes:"look", mouth:"small_lock", body:"fear"})`

b: Uff! Ty zahazuješ svůj život sjížděním Twitteru! Už zase!

```
bb({eyes:"normal", mouth:"normal", body:"normal"});
hong({eyes:"annoyed"});
```

h: Wow. Přemýšlím, proč si častěji prostě jen tak nesednu a nepřemýšlím...

`hong({eyes:"neutral"});`

n: RYCHLE, VARUJ HO, ŽE JE *OHROŽENÝ!*

```
bb({eyes:"look"});
```

[Ale ne, koukej na ty příšerný zprávy!](#act1d_news)

[Ale ne, není ten tweet mezi řádky náhodou o *nás*?](#act1d_subtweet)

[Koukej, GIF s kočičkou, co pije mléko](#act1d_milk)


# act1d_milk

`hong({mouth:"smile", eyes:"surprise"});`

h: Heh, jů, to je sladký, tak--

```
hong({mouth:"shock", eyes:"shock"});
bb({body:"scream"});
Game.OVERRIDE_TEXT_SPEED = 1.8;
```

b: KOČKY NESTRÁVÍ MLÉKO A TY JSI HROZNÝ ČLOVĚK, PROTOŽE SI UŽÍVÁŠ TÝRÁNÍ ZVÍŘAT


(...200)

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
attack("20p", "bad");
publish("hp_show");
```



