# Extras I did not include in the main parts of Guinea-Softx

------------

 ## Custom Theme colors 
Based on the KDE Plasma theme [Vivid-Dark](https://github.com/L4ki/Vivid-Plasma-Themes)   
Preview of the [Custom colors](https://github.com/user-attachments/assets/7e623567-cc9d-45e1-af7c-d0cfaeb0b928)

`Left: #36446E`   
`Middle: #222C41`   
`Right: #6077AA`

It should look kinda like this.   
<img width="299" height="69" alt="image" src="https://github.com/user-attachments/assets/4d6ffc5a-2714-425d-880b-060b5bf01dfa" />

_Also all the colors should have Color intensity of 60% and gradiant direction 0°_


---

# CSS Tweaks
To add any of below CSS changes just copy and paste them into the vencord custom Css. Or if not useing vencord Append them to the end of the CSS file of the theme

## Hide some Buttons in settins
If there is a setting button you don't want to remove from this list just delate its accosiated line.   
(tho things will break if you remove `Offical Discord social account buttons`line or `display: none;` lines of this)
```
/*Top & middle section*/
.side_aa8da2 > div:nth-child(7)  /* famliy center */,
.side_aa8da2 > div:nth-child(11) /* Clips */,
.side_aa8da2 > div:nth-child(27) /* Language and time */,
.side_aa8da2 > div:nth-child(26) /* keybinds */ /* still can use ctl+/ to open it */,
/* activity privicy */
.side_aa8da2 > div:nth-child(39) /* activity privicy Divider */ ,
.side_aa8da2 > div:nth-child(40) /* activity privicy header */,
.side_aa8da2 > div:nth-child(41) /* activity privicy button */,
/* Bottom section */
.side_aa8da2 > div:nth-child(42) /* What's new divider */,
.side_aa8da2 > div:nth-child(43) /* what's new button */,
.side_aa8da2 > div:nth-child(44) /* Merch */,
.side_aa8da2 > div:nth-child(45) /* Bottom divider */,
.side_aa8da2 > div:nth-child(48) /* Offical Discord social account buttons */ {
  display: none;
}
```
### Vencord options (seperted since these will break things if you are not useing vencord)
```
/* Vencord */
.side_aa8da2 > div:nth-child(35) /* Updater */,
.side_aa8da2 > div:nth-child(36) /* cloud */,
.side_aa8da2 > div:nth-child(37) /* Backup and restore */ {
  display: none;
}
```
### Nitro options (seperted for pepole who use nitro)
```
/* Nitro */
.side_aa8da2 > div:nth-child(12) /* Billing divider */,
.side_aa8da2 > div:nth-child(13) /* Billing settings header */,
.side_aa8da2 > div:nth-child(14) /* Nitro */,
.side_aa8da2 > div:nth-child(15) /* server Boost */,
.side_aa8da2 > div:nth-child(16) /* Subscriptions */,
.side_aa8da2 > div:nth-child(17) /* Gift Inventory */,
.side_aa8da2 > div:nth-child(18) /* Billing */
 {display: none;}
```

## Remove Quest Button Above DMS

` div.scroller__99e7c.thin_d125d2.scrollerBase_d125d2.fade_d125d2 > ul > div.wrapper__553bf {display: none;} `

## Remove Nitro Button Above DMS

`div.scroller__99e7c.thin_d125d2.scrollerBase_d125d2.fade_d125d2 > ul > div:nth-child(3) {display: none;}`

## Remove Activities Button to the right of the emoji button

`.buttonContainer_e6e74f.app-launcher-entrypoint {display: none;}`

