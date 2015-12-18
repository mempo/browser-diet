---
order: 21
title: Zkuste async
---

Abychom vysvětlili, jak je tento atribut užitečný pro lepší výkon, je dobré pochopit, co se děje, když jej nepoužijeme.

<div class="img-left">
  <img id="geek-20" class="icos-geek" src="https://browserdiet.com/en/assets/img/20.png" alt="Geek #20" width="118" height="275" />
</div>

``` html
<script src="example.js"></script>
```

V tomto případě musí stránka čekat, dokud není skript celý stažený, naparsovaný a spuštěný, před tím, než může být zpracováno a vykresleno další HTML. To může značně prodloužit čas načítání vaší stránky. Občas je takové chování požadováno, obecně však ne.

``` html
<script async src="example.js"></script>
```

Skript je stažen asynchronně, zatímco pokračuje parsování zbytku stránky. Je garantováno, že se skript spustí hned, jak bude stažen. Mějte na mysli, že v případě více asynchronních skriptů není nijak zaručeno, v jakém pořadí budou spuštěny.

*> [Reference](https://github.com/zenorocha/browser-diet/wiki/References#try-out-async)*
