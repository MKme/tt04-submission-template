![](../../workflows/gds/badge.svg) ![](../../workflows/docs/badge.svg) ![](../../workflows/wokwi_test/badge.svg)


<p align="center">


<br>
<br>
🐦 <a href="https://twitter.com/mkmeorg">Twitter</a>
| 📺 <a href="https://www.youtube.com/mkmeorg">YouTube</a>
| 🌍 <a href="http://www.mkme.org">mkme.org</a><br>
Support this project and become a patron on <a href="http://mkme.org/patreon">Eric's Patreon</a>.<br>
Website, Forum and store are at http://mkme.org <br>
Chat with Me: <a href="https://discord.gg/j9S4Fgv">Discord</a></b>
</p>


#  8 Bit Digital Zipher
Simple cipher using 8 bit IO 

## The Idea
8 bit input. One combination opens the lock and powers the output. 255 combinations do not. 

Imagine this project has been done to death but this will be my first ASIC. 

## The reason

I want to support the tinytapeout initiative and also spread the knowledge on how to make fun projects and learn new skills. Having made ones' own IC is quite cool. 

## How it works
Can be used as a simple puzzle demo or as a safety chain/interlock on equipment.
Being hardware interlocks without microcontroller logic it should be acceptable in
some industry certifications. The high or low input can be tied to the sensors and
switches in the safety chain. Only when all are in the desired state will the output be
OKAY/HIGH. NO and NC switches/sensors can be tied to the appropriate pins.

## How to test
Provide below inputs on the required pins to activate output
## IO

# Input Output Bidirectional
0 HIGH HIGH none
1 LOW NA none
2 HIGH NA none
3 HIGH NA none
4 LOW NA none
# Input Output Bidirectional
5 HIGH NA none
6 LOW NA none
7 HIGH NA none

# What is Tiny Tapeout?

TinyTapeout is an educational project that aims to make it easier and cheaper than ever to get your digital designs manufactured on a real chip!

Go to https://tinytapeout.com for instructions!

## How to change the Wokwi project

Edit the [info.yaml](info.yaml) and change the wokwi_id to match your project.

## How to enable the GitHub actions to build the ASIC files

Please see the instructions for:

- [Enabling GitHub Actions](https://tinytapeout.com/faq/#when-i-commit-my-change-the-gds-action-isnt-running)
- [Enabling GitHub Pages](https://tinytapeout.com/faq/#my-github-action-is-failing-on-the-pages-part)

## How does it work?

When you edit the info.yaml to choose a different ID, the [GitHub Action](.github/workflows/gds.yaml) will fetch the digital netlist of your design from Wokwi.

After that, the action uses the open source ASIC tool called [OpenLane](https://www.zerotoasiccourse.com/terminology/openlane/) to build the files needed to fabricate an ASIC.

## Resources

- [FAQ](https://tinytapeout.com/faq/)
- [Digital design lessons](https://tinytapeout.com/digital_design/)
- [Learn how semiconductors work](https://tinytapeout.com/siliwiz/)
- [Join the community](https://discord.gg/rPK2nSjxy8)

## What next?

- Submit your design to the next shuttle [on the website](https://tinytapeout.com/#submit-your-design), the closing date is 8th September.
- Share your GDS on Twitter, tag it [#tinytapeout](https://twitter.com/hashtag/tinytapeout?src=hashtag_click) and [link me](https://twitter.com/matthewvenn)!
