# Peak Computing

Friends often ask what ThinkPads I recommend and why, and I figure that 
rather than going on a really autistic rant for the next hour, it might make sense 
to just have a page I link them to.

## ThinkPad X230 - Patrician's Choice

A lot of people online are still on the ThinkPad X220 train, and this is 
somewhat understandable for a satisfying out-of-the-box experience, however 
the X230 has far more potential than most realize. Firstly, it is an easy 
matter to replace Lenovo's new (cringe) keyboard with the [older (based) X220 keyboard](https://www.thinkwiki.org/wiki/Install_Classic_Keyboard_on_xx30_Series_ThinkPads)
and with a quick flash of [modified embedded controller firmware](https://github.com/hamishcoleman/thinkpad-ec), you've both 
replicated all X220 keyboard functionality (save for the Caps Lock light) and removed 
the battery whitelist which normally prevents the use of aftermarket (and even 
X220) batteries. Already after doing this, you effectively have an X220 with a 
vastly superior iGPU and a slightly better, more efficient processor that can run 
DDR3 memory at higher speeds (1866MHz vs 1333MHz). Additionally, while _only_ the i7 X220 
model supports USB 3.0, all X230 models do.  

Let's say you want to go further. Maybe you wanted this to feel more like a 
tangible hardware upgrade. There are a number of [X230 motherboard 
options](https://www.aliexpress.com/item/1005001368272558.html) on webites like 
AliExpress which have undergone BGA rework to accomodate quad-core hyperthreaded 
processors. In terms of the display, while there are kits that work for both the 
X220 and X230 to bring them to [1080p](https://nitrocaster.me/store/x220-x230-fhd-mod-kit.html), you will 
need an X230 if you wish to upgrade to [1440p (or even 1600p)](https://www.xyte.ch/shop/)! Even if such a kit were to support the X220, you will likely 
notice the weaker iGPU far more frequently. 

A lot of people wish to coreboot their machines and do whatever they can to 
inhibit Intel's Management Engine spyware. Due to the BIOS and Management Engine 
being stored on two chips (both conveniently located under the palmrest) rather than one, as was the case on the X220, it is far easier to do this on the X230. The hardware changes with the X230 allow for prebuilt images like those provided by projects like [skulls](https://github.com/merge/skulls) to be used when corebooting. 
This project in particular also has a convenient flag that can be used to run [me\_cleaner](https://github.com/corna/me_cleaner) during this process. On 
the X220 by contrast, coreboot images have to be configured and built manually on 
a per-device basis, and me\_cleaner must be run separately. Skulls also provides [patches](https://github.com/jyvet/skulls/commit/8cc80fa439198753920ac04bd010cee994c09908) for the aforementioned 1080p screen mod, which is something you will inevitably run into more annoyance with on the X220. Assuming you also 
replace the Intel wifi card (coreboot removes the wifi card whitelist), you can 
now reliably make use a deblobbed kernel like Debian's or linux-libre, or install 
an OS like OpenBSD without worrying about having to install additional nonfree 
firmware. 

## Corebooted ThinkPad T420

Once corebooted, the T420 not only supports the higher memory speeds of 
the T430, but hilariously, you can also install Ivy Bridge processors that you'd 
otherwise need a T430 to make use of. 

## ThinkPad T430

If you're down to replace the keyboard with a T420 keyboard, care a lot about USB 
3.0, or don't wish to coreboot your machine for whatever reason, then fine, fuck it, 
why not, the T430 also works. 

## Librebooted ThinkPad T400/X200

For RMS-type people who are left unsatisfied due to the the 90kB of remaining 
neutered Management Engine running briefly at boot which is left over after 
running me\_cleaner on xx20/xx30-series models. This is effectively the best 
hardware you can acquire in a ThinkPad with these contraints. If you do not intend 
to run them with Libreboot, don't even bother with these machines unless you get a good deal.

## ThinkPad W700ds/W701ds

Gee Bill! How come your mom lets you have _two_ screens?

## Honorary Mentions

The X60, T60, X61, T61, X201, X220, and T410 and their variants have varying 
degrees of merit depending on what you intend to do with them and what price you acquire them for. 
