# Android Homescreen [Ricing](https://wiki.installgentoo.com/wiki/Android_ricing) 📱🍙 [MIRAI-未来]

a small collection of KWGT Widgets I did for my Huawei Mate 20 Pro `LYA-29`

## Screenshots

<img src="./res/Screenshot_1.jpg" width="420" alt="Mirai Android Wallpaper">


Music_Player.kwgt, Neofetch.kwgt           |  Sushi_Clock.kwgt, Weather.kwgt
:-------------------------:|:-------------------------:
![Media Player and Neofetch Widgets](/res/Screenshot_2.jpg)  |  ![Sushi_Clock and Weather Widgets](/res/Screenshot_3.jpg)

## How to use it?

you can import the `.kwgt` files with the [Kustom KWGT App](https://play.google.com/store/apps/details?id=org.kustom.widget)\.

---

## add coin price and update

![sushi_price](res/Screenshot_4.jpg)

create a global variable with a [coingecko API](https://www.coingecko.com/en/api/documentation) call as text

current Sushi price (EUR) -> gv
`https://api.coingecko.com/api/v3/simple/price?ids=sushi&vs_currencies=EUR`

create a text Element with `wg()` and JSON parser

`$wg(gv(YOUR_GLOBAL_VARIABLE_NAME), json, .sushi.eur)$€` 

I use the sushi logo with a "Kustom Action" to force "RSS/TEXT/XML-Updates" on tap which refreshes the call/price.

### todo

- [ ] fetch termux output from bash\.
- [x] add current $SUSHI price\.
- [ ] toggle light/dark mode\.
