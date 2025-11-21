## Visuals

https://github.com/okadus/roll20-penombre/blob/main/assets/img/case_de_penombre.webp?raw=true (l'harmonique)

https://github.com/okadus/roll20-penombre/blob/main/assets/img/de_case_checked.webp?raw=true (atout checkbox cochée)

https://github.com/okadus/roll20-penombre/blob/main/assets/img/de_case_unchecked.webp?raw=true (atout checkbox décochée)

https://github.com/okadus/roll20-penombre/blob/main/assets/img/frise_plus_grande_sur_fond_clair.webp?raw=true (bannière)

https://github.com/okadus/roll20-penombre/blob/main/assets/img/logo_penombre_sur_fond_clair.webp?raw=true (logo pénombre)

https://github.com/okadus/roll20-penombre/blob/main/assets/img/potentiel.webp?raw=true (Potentiel)

https://github.com/okadus/roll20-penombre/blob/main/assets/img/marron.webp?raw=true (barre marron)

https://github.com/okadus/roll20-penombre/blob/main/assets/img/doree.webp?raw=true (barre or)

https://github.com/okadus/roll20-penombre/blob/main/assets/img/grise.webp?raw=true (barre grise)

https://github.com/okadus/roll20-penombre/blob/main/assets/img/fond-coupe-petit.webp?raw=true (fond coupe petit)

https://github.com/okadus/roll20-penombre/blob/main/assets/img/fond-coupe.webp?raw=true (fond coupe)

https://github.com/okadus/roll20-penombre/blob/main/assets/img/fond.webp?raw=true (fond)

## Fonts

https://github.com/okadus/roll20-penombre/blob/main/assets/fonts/P22Freely.otf (P22Freely.otf)
https://github.com/okadus/roll20-penombre/blob/main/assets/fonts/P22Freely.ttf (P22Freely.ttf)

https://github.com/okadus/roll20-penombre/blob/main/assets/fonts/cattedrale-regular.otf (cattedrale-regular.otf)

## Colors

#bfa285

## Macros

### harmonique

&{template:harmonique} [[floor([[1d@{nuit}cs@{nuit}cf1]]/4) ]] [[floor([[1d20cs20cf1]]/4) ]] {{title=@{character_name}}} {{carac=Nuit}} @{rtype}}} {{jet_brut_harm=$[[0]]}} {{r_harmonique=$[[1]]}} {{jet_brut_merv=$[[2]]}} {{r_merveilleux=$[[3]]}} {{difficulte=[[?{Difficulté|1}]]}} {{max_harm=[[@{nuit}]]}} {{max_merv=[[20]]}} {{un=[[1]]}}

### atout

&{template:harmonique} [[20]] [[1]] [[?{Difficulté|0}]] [[?{Harmonique|Nuit,@{nuit}|Âme,@{ame}|Nature,@{nature}|Esprit,@{esprit}|Étincelle,@{etincelle}}]] [[[[floor([[1d?{Harmonique}]]/4)]] + [[@{atout_nd6}d6>4]] ]] [[[[floor([[1d20]]/4)]] + [[@{atout_nd6}d6>4]] ]] {{title=@{character_name}}} @{rtype}}} {{max_merv=$[[0]]}} {{un=$[[1]]}} {{difficulte=$[[2]]}} {{max_harm=$[[3]]}} {{jet_brut_harm=$[[4]]}} {{jet_brut_merv=$[[6]]}} {{r_harmonique=$[[10]]}} {{r_merveilleux=$[[11]]}}

### atout 2

&{template:harmonique} [[20]] [[1]] [[?{Difficulté|0}]] [[?{Harmonique|Nuit,@{nuit}|Âme,@{ame}|Nature,@{nature}|Esprit,@{esprit}|Étincelle,@{etincelle}}]] [[[[floor([[1d?{Harmonique}]]/4)]] + [[@{atout_nd6}d6>4]] ]] [[[[floor([[1d20]]/4)]] + [[@{atout_nd6}d6>4]] ]] {{title=@{character_name}}} @{rtype}}} {{carac=?{Quel Harmonique|Nuit|Âme|Nature|Esprit|Étincelle}}} {{max_merv=$[[0]]}} {{un=$[[1]]}} {{difficulte=$[[2]]}} {{max_harm=$[[3]]}} {{jet_brut_harm=$[[4]]}} {{jet_brut_merv=$[[6]]}} {{r_harmonique=$[[10]]}} {{r_merveilleux=$[[11]]}}
