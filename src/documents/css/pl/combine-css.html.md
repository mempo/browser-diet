---
order: 23
title: Łączenie wielu plików CSS
---

Kolejna dobra praktyka dla organizacji i obsługi stylów to dzielenie ich na mniejsze moduły.

```html
<link rel="stylesheet" href="structure.css" media="all">
<link rel="stylesheet" href="banner.css" media="all">
<link rel="stylesheet" href="layout.css" media="all">
<link rel="stylesheet" href="component.css" media="all">
<link rel="stylesheet" href="plugin.css" media="all">
```

Jednak każdy z tych plików wymaga osobnego żądania HTTP (dobrze wiemy, że przeglądarki pobierają równolegle ograniczoną liczbę zasobów).

```html
<link rel="stylesheet" href="main.css" media="all">
```

Połącz swoje pliki CSS. Mniejsza liczba plików, daje w rezultacie mniejszą liczbę żądań i szybsze ładowanie strony.

Chcesz najlepszych wyników? Automatyzacja tego procesu poprzez narzędzia budowania.

*> Przydatne narzędzia: [Grunt](http://gruntjs.com/).*
