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

## Design your Keyboard

![](static/keyboard%20drawing.jpg)

# Collect your parts

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

![](static/cherry-switch-table.webp){ height=50% }

## Switches

![](static/choc-switch-table.png){ height=50% }

## Switches

![](static/cherry-switch-tree.webp){ height=50% }

## Shield / PCB / Sockets / Hand Wired

![](static/split-pcb.jpg){ height=50% }

## Shield / PCB / Sockets / Hand Wired

![](static/skree-pcbs.webp){ height=50% }

## Shield / PCB / Sockets / Hand Wired

![](static/cherry-switch-pcb.png){ height=50% }

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

::: incremental

- Wired or Wireless
- How many inputs?

:::

## Microcontroller / Firmware

::: incremental

- QMK
  - The default
  - Wide support
  - Lots of offshoot projects (via, vial, etc.)
  - Mostly for wired boards

:::

## Microcontroller / Firmware

::: incremental

- ZMK 
  - The upstart
  - Less board support
  - More difficult to get started
  - Mostly for wireless boards

:::

## Microcontroller / Firmware

![](static/pro-micro.webp){ height=250 }

::: notes

This is the most common format for controllers

There are lots of controllers that share the same pinout, not just clones

:::

## Microcontroller / Firmware

![](static/nice-nano.png){ height=250 }

::: notes

This is a copy of the pro-micro format for wireless builds

:::

## Microcontroller / Firmware

![](static/rp2040.webp){ height=250 }

::: notes

This is a chonky boy if you want lots of inputs

:::

## Case

![](static/3d-printers.webp){ height=250 }

# Building a Keyboard

## Shopping List

::: incremental

 - [x] Keycaps
 - [x] Switches
 - [x] PCB
 - [x] Accessories
 - [x] Microcontroller
 - [x] Case
 
:::

## Assemble your board

![](static/my-diy-board.jpg){ height=250 }

::: notes

Depends on how you're putting it together

Might put switches in first, might do sockets first

:::

## Wire your board

![](static/matrix.png){ height=250 }

::: notes

you'll need num rows + num cols inputs on your board, so minimizing is good

also consider difficulty of wiring

also consider thumb keys if doing an ergo

hot swap vs soldered in

:::

## Wire your board

![](static/hand-wired.jpg){ height=250 }

## Setup your Firmware

## QMK

![](static/qmk-logo.png){ height=250 }

::: notes

most popular

mostly used for wired builds

lots of spinoffs

vial etc.

:::

## QMK

![](static/qmk-configurator.png){ height=250 }

## QMK

![](static/qmk-toolbox.png){ height=250 }

## QMK

```
sudo pacman -S qmk
qmk setup
qmk flash -kb sofle -km default
```

## ZMK

![](static/zmk-logo.jpg){ height=250 }

::: notes

mostly used for wireless builds

less accessory support

community not quite as big

making rapid progress

:::

## ZMK

 1. Create a new Github Repo called `zmk-config`
 2. `bash -c "$(curl -fsSL https://zmk.dev/setup.sh)"`

## ZMK

![](static/github-actions.png){ height=250 }

## ZMK

![](static/github-actions-2.png){ height=250 }

## ZMK

![](static/github-actions-3.png){ height=250 }

## ZMK

```
unzip firmware.zip
cp my-keyboard.u2f /var/run/media/rtward/NICENANO
```

## ZMK

![](static/zmk-configurator.png){ height=250 }

# Contrats!

## Cosmetics

::: notes

case, tenting, etc.

:::

## Proft!

::: notes

You've got a cool ass keyboard now

You can spend the next few months tweaking the keymap to be just what you want

:::

# Links

 - https://skree.us/
 - https://www.littlekeyboards.com/
 - https://www.aliexpress.us/
 - https://ryanis.cool/cosmos/
 - https://config.qmk.fm/
 - https://nickcoutsos.github.io/keymap-editor/
 - https://nickcoutsos.github.io/keymap-layout-tools/
 - https://zmk-physical-layout-converter.streamlit.app/

# Questions?

![](static/but-why-male-models.jpg)

---

Robert Ward <robert@rtward.com>

![](static/qrcode.png)

Talk: [${TALK_URL}](${TALK_URL})

Repo: [${REPO_URL}](${REPO_URL})
