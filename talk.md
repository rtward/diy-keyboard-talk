% DIY Keyboards
% Robert Ward <robert@rtward.com>
%![](static/qrcode.png)<br/>Talk: [${TALK_URL}](${TALK_URL})<br/>Repo: [${REPO_URL}](${REPO_URL})

# DIY Keyboards

## Or

## How I learned to stop worrying and love the blinky lights

![](static/hackers-keyboard.png)

# Why?

![](static/but-why.jpg)

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

![](static/layers.png)

::: notes

Change your whole layout with one key

:::

## It's Cool

![](static/hackerman.webp)

::: notes

Lets be honest

:::

# Okay I'm Convinced

# How do I do it?

## Design your Keyboard

![](static/cosmos-screenshot.png)

## Design your Keyboard

![](static/keyboard%20drawing.jpg)

# Collect your parts

## Keycaps

![](static/keycaps.webp)

::: notes

Starting with the most important part, obviously.

So many options

:::

## Keycaps

![](static/custom-keycap-1.webp)

## Keycaps

![](static/custom-keycap-2.webp)

## Keycaps

![](static/custom-keycap-3.jpg)

## Switches

![](static/mx-switch.webp)

::: notes

Two basic options, MX or Choc

:::

## Switches

![](static/choc-switch.jpg)

::: notes

Choc are low-profile if you're trying to build a smaller board

:::

## Switches

![](static/cherry-switch-table.webp)

## Switches

![](static/choc-switch-table.png)

## Switches

![](static/cherry-switch-tree.webp)

## Shield / PCB / Sockets / Hand Wired

![](static/split-pcb.jpg)

## Shield / PCB / Sockets / Hand Wired

![](static/skree-pcbs.webp)

## Shield / PCB / Sockets / Hand Wired

![](static/cherry-switch-pcb.png)

## Shield / PCB / Sockets / Hand Wired

![](static/hand-wired.jpg)

## Accessories

![](static/encoder.webp)

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

![](static/pro-micro.webp)

::: notes

This is the most common format for controllers

There are lots of controllers that share the same pinout, not just clones

:::

## Microcontroller / Firmware

![](static/nice-nano.png)

::: notes

This is a copy of the pro-micro format for wireless builds

:::

## Microcontroller / Firmware

![](static/rp2040.webp)

::: notes

This is a chonky boy if you want lots of inputs

:::

## Case

![](static/3d-printers.webp)

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

![](static/my-diy-board.jpg)

::: notes

Depends on how you're putting it together

Might put switches in first, might do sockets first

:::

## Wire your board

![](static/matrix.png)

::: notes

you'll need num rows + num cols inputs on your board, so minimizing is good

also consider difficulty of wiring

also consider thumb keys if doing an ergo

hot swap vs soldered in

:::

## Wire your board

![](static/hand-wired.jpg)

## Setup your Firmware

## QMK

![](static/qmk-logo.png)

::: notes

most popular

mostly used for wired builds

lots of spinoffs

vial etc.

:::

## QMK

![](static/qmk-configurator.png)

## QMK

![](static/qmk-toolbox.png)

## QMK

```
sudo pacman -S qmk
qmk setup
qmk flash -kb sofle -km default
```

## ZMK

![](static/zmk-logo.jpg)

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

![](static/github-actions.png)

## ZMK

![](static/github-actions-2.png)

## ZMK

![](static/github-actions-3.png)

## ZMK

```
unzip firmware.zip
cp my-keyboard.u2f /var/run/media/rtward/NICENANO
```

## ZMK

![](static/zmk-configurator.png)

## ZMK

Demo Time

## ZMK

::: incremental 

 1. Find a keyboard that's close
 2. Copy the board over
 3. Edit the physical layout (.dtsi)
 3. Edit the sides if split
 3. Edit the board for accessories
 3. Update your build.yaml
 3. Push to GitHub

:::

# Congrats!

## Congrats!

![](static/cowboy-bebop.webp)

::: notes

You've got a cool ass keyboard now

You can spend the next few months tweaking the keymap to be just what you want

:::

# Advice

## Macro Pad

![](static/macro-pad.jpg)

::: notes

Build a macro pad first.

It's basically all the same work, but much easier.

:::

## Experiment

![](static/experiment.jpg)

::: notes

Play around with designs and keymaps, find what works for you.

:::

## Commit

![](static/handcuffs.jpg)

::: notes

Stay committed to using your new board and trying new layouts.

You'll be surprised how quickly you can adapt.

:::

# Questions?

![](static/but-why-male-models.jpg)

---

Robert Ward <robert@rtward.com>

![](static/qrcode.png)

Talk: [${TALK_URL}](${TALK_URL})

Repo: [${REPO_URL}](${REPO_URL})
