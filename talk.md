% DIY Keyboards
% Robert Ward <robert@rtward.com>
%![](static/qrcode.png)<br/>Talk: [${TALK_URL}](${TALK_URL})<br/>Repo: [${REPO_URL}](${REPO_URL})

# DIY Keyboards

## Or

## How I learned to stop worrying and love the blinky lights

![](static/hackers-keyboard.png){ width=100% }

# Why?

![](static/but-why.jpg){ height=100% }

## Cheaper?

. . .

no

## More Reliable?

. . .

no

## Better?

. . .

maybe?

## Because

## RSI

![](static/hand-cramp.webp){ width=100% }

::: notes

More an argument for ergo

My story

:::

## Custom Layouts

::: notes

Want to try out DVORAK or Colemak or Workman?

:::

## Macros

<div align="center">
```
(•_•) ( •_•)>⌐■-■ (⌐■_■)
```
</div>

::: notes

Your keybaord can do more than 1 press = 1 letter

:::

## Layers

![](static/layers.png){ width=100% }

::: notes

Change your whole layout with one key

:::

## It's Cool

![](static/hackerman.webp){ height=100% }

::: notes

Lets be honest

:::

# Okay I'm Convinced

# How do I do it?

## Design your Keyboard

![](static/cosmos-screenshot.png){ height=100% }

Cosmos - https://ryanis.cool/cosmos/

## Design your Keyboard

![](static/keyboard%20drawing.jpg)

# Collect your parts

 - https://skree.us/
 - https://www.littlekeyboards.com/
 - https://www.aliexpress.us/

## Keycaps

![](static/keycaps.webp){ height=100% }

::: notes

Starting with the most important part, obviously.

So many options

:::

## Keycaps

![](static/custom-keycap-1.webp){ height=100% }

## Keycaps

![](static/custom-keycap-2.webp){ height=100% }

## Keycaps

![](static/custom-keycap-3.jpg){ height=100% }

## Switches

![](static/mx-switch.webp){ height=100% }

::: notes

Two basic options, MX or Choc

:::

## Switches

![](static/choc-switch.jpg){ height=100% }

::: notes

Choc are low-profile if you're trying to build a smaller board

:::

## Switches

![](static/cherry-switch-table.webp){ height=100% }

## Switches

![](static/choc-switch-table.png){ height=100% }

## Switches

![](static/cherry-switch-tree.webp){ height=100% }

## Shield / PCB / Sockets / Hand Wired

![](static/split-pcb.jpg)

## Shield / PCB / Sockets / Hand Wired

![](static/skree-pcbs.webp)

## Shield / PCB / Sockets / Hand Wired

![](static/cherry-switch-pcb.png)

## Shield / PCB / Sockets / Hand Wired

![](static/hand-wired.jpg)

## Accessories

![](static/encocder.webp)

## Accessories

![](static/trackball.webp)

## Accessories

![](static/oled.webp)

## Accessories

![](static/rgb.jpg)

## Accessories

![](static/kitchen-sink.jpg)

## Microcontroller / Firmware

- Wired or Wireless
- How many inputs?

- Pro Micro is the most common format
- Nice!Nano for Wireless

- Wired or Wireless
- ZMK for Wireless
- QMK for Wired
- Lots of offshoots of QMK

## Case

![](static/hand-wired.jpg){ height=100% }

# Shopping List

::: incremental

 - [x] Keycaps
 - [x] Switches
 - [x] PCB
 - [x] Accessories
 - [x] Microcontroller
 - [x] Case
 
 :::

# Building a Keyboard

## Plan your wiring

::: notes

you'll need num rows + num cols inputs on your board, so minimizing is good

also consider difficulty of wiring

also consider thumb keys if doing an ergo

hot swap vs soldered in

:::

## Plan your accessories

::: notes

make sure you know how many inputs you need

check out com protocols like i2c or spi, which can be shared in some cases

:::

## Plan your controller

::: notes

wired or wireless is the big question

also look at firmware compatibility

also look at number and types of IO ports

:::

## PCB / Shield vs Hand Wiring

::: notes

shield = easier

hand wiring = more customization

:::

## Setup your Firmware

## QMK

::: notes

most popular

mostly used for wired builds

lots of spinoffs

vial etc.

:::

## ZMK

::: notes

mostly used for wireless builds

less accessory support

community not quite as big

making rapid progress

:::

## Cosmetics

::: notes

case, tenting, etc.

:::

## Proft!

::: notes

You've got a cool ass keyboard now

You can spend the next few months tweaking the keymap to be just what you want

:::

# Questions?

![](static/but-why-male-models.jpg)

---

Robert Ward <robert@rtward.com>

![](static/qrcode.png)

Talk: [${TALK_URL}](${TALK_URL})

Repo: [${REPO_URL}](${REPO_URL})
