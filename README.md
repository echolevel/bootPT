# bootPT
Bootable Amiga floppy disk image with Syphus' custom Protracker build

![bootPT screenshot](screenshot.png)

## Changelog

* v0.07 - merged 8bitbubsy's fixes to a raw sample loading bug I discovered
* v0.06 - new Protracker build based on 8bitbubsy's latest source (February 2020), and changed config references from DF0: to PTBOOT2.3F:, and finally updated About screen to reflect the 'F'
* v0.05 - new Protracker build based on 8bitbubsy's latest source (October 2019), and added mod2smp.cli
* v0.04 - new Protracker build based on 8bitbubsy's latest source (September 2019), and added some tiny intro code that displays an ASCII logo
* v0.03 - realised add36k was causing problems, replaced it with add44k
* v0.02 - fixed samples assign in PT-Config.00
* v0.01 - initial commit

## Usage

Boot the Amiga with this image - tested on A1200 and A500, and should work on almost all others. If you're dropped back to an AmigaDOS screen after getting a 'disk not found' message while swapping floppy disks/images ( to save/load modules or samples), don't worry - Protracker probably hasn't crashed, just lost focus. Hit Left-Amiga + M on the keyboard to switch back to Protracker. Enjoy!

## Documentation

See the About section (below) for some more info about this ADF, but for general Protracker documentation I've done a quick [Markdown reformat of the original PT2.3d helpfile](2019_PT_HELPFILE.md). It's built into Protracker, but it's sometimes difficult to navigate (and impossible to search through). I've added and annotated where appropriate, in reference to 2.3e and 2.3f changes, but it's an ongoing work in progress. Ultimately I'd like this to be a canonical repository of everything that's known about PT2.3d+ so please contribute if you think anything's missing!

## About

This is just a bootable ADF file which can be used with an emulator such as WinUAE (Windows) or FS-UAE (MacOS), or with a GOTEK USB floppy emulator on real Amiga hardware. It's intended for maximum compatibility with OCS/ECS machines (A500, A500+, A600), but should also work fine on AGA machines.

The startup-sequence first runs add44k, a tiny program that increases your available RAM by removing one entire bitplane and shrinking the other to 50 pixels (written in 1992 by Alexander Rawass). Protracker can only address samples in chip memory since it uses the DMA to play back sampledata with almost no cost to the CPU. The disadvantage is that it's unable to store or read any samples using fast ram you might have installed (RAM expansions, basically), limiting you to 512kb on a stock A500 or 2MB on a stock A1200, but lots of amazing tunes have been written within these limitations so don't get disheartened :D Protracker will, however, try to put as much non-sample data (graphics, patterndata, etc) as possible in fast mem in order to free up chip mem, so having some fast mem definitely helps. Here's some info about how you could expand your desktop 'wedge' style Amiga (I'm less familiar with the big box models, but the general principles are the same):


| Amiga model | Stock Chip Mem | Chip Mem Limit | Fast Mem Options |
| ------------ | ------------- | ----------|------------ |
| A500 | 0.5MB (512KB) | 1MB with trapdoor expansion, 2MB possible with Gary mod | Various accelerator and edge connector options, new and old |
| A500+ | 1MB | 2MB with trapdoor expansion | Various accelerator and edge connector options, new and old |
| A600 | 1MB | 2MB with trapdoor expansion | 4MB and 8MB fast mem expansions; more available with accelerators |
| A1200 | 2MB | 2MB is all you're getting! | Trapdoor ram expansions (some include FPU), various accelerators |

Note: much of the current market for new old stock and newly manufactured accelerators and ram expansions is based on people's enthusiasm for WHDLoad, a program that allows Amiga games to be installed to - and played directly from - hard disk. The overhead involved means that games which in the early 90s ran happily on a stock A1200, for example, now need a bit more RAM to run WHDLoad. A little bit of extra CPU helps too, but also people always want as much speed as possible :) If your main vibe is wanting to use Protracker on a real Amiga, however, you can have an absolute blast on just a stock A1200, A600 or A500+! Also a stock A500, but I'd say the extra 512KB to bring you up to 1MB chip mem would be very much worth the ~£20 it would cost you. Some of Protracker's VU meters might struggle slightly on an A500/A500+, but the audio will never glitch - that's rock solid Paula/68k stuff and Paula doesn't care how fast your CPU is. So what I'm saying is: please don't go and blow loads of money on a load of fancy expansions until you're sure you need them!


After add44k has squeezed a bit more free memory out of the system for us, Protracker 2.3F runs automatically. A few notes about the default config I've included:

* AUTOEXIT is Off (so Disk Op stays open after you've loaded something, good if you're not sure which sample you want)
* MOD. ONLY is Off (so you'll see all files when loading modules, not just those with the mod.prefix. File extensions are pretty free and easy on Amiga; programs can implement them if they want, but there are no canonical associations. Protracker modules traditionally have mod. as a prefix, not '.mod' as a suffix - but this is just so you know what type of files they are. Protracker doesn't care either way! If you try to load a non-mod file as a module, it'll let you...you'll probably want to do CLEAR->ALL on the main screen to empty out all the garbage that'll appear)
* CUTTOBUFF is On (if you're on a stock A500, or have very limited chipmem for some other reason, you might want to disable this - it'll mean that any 'cut' operation while editing samples is destructive and final, but it might save you running out of memory)
* AUTODIR is Off (this should stop PT from reading directories until you've typed Return in the path field, but it doesn't seem to be working...maybe a bug?)
* The others you can look up in the 2019_PT_HELPFILE :)


This is my custom build of PT2.3F, which in turn is [8bitbubsy's](https://16-bits.org) fantastic overhaul of the previously definitive Protracker version: 2.3D. While 2.3D was the best, and more stable than most of its successors, it had a load of bugs that hung around for almost 20 years until 8bitbubsy redid the code from the ground up. Thanks to his tidying and helpful ASM comments, and thanks to some tips from StingRay^Scarab, I've been able to add some usability tweaks that I always wanted in Protracker plus - of course - my own custom graphics. Partly vanity, partly for fun, but also partly because I always used to be intrigued by demogroups' internal-only custom builds of popular demotools in the early 90s: typically they looked awesome but were actually kind of crappy and unstable, created (or modified to suit from available source) as OMG TOP SECRET GROUP-ONLY prods that eventually leaked out into the public domain.

Anyway, last night (19th October 2019) I decided to mess with the graphics assets in DeluxePaint IV to get a sort of decaying, decrepit feel for the GUI which seems appropriately Halloweeny for the time of year. It's based on 8bitbubsy's final source code for v2.3F and is probably as stable as Protracker is ever gonna get.

I've also added the CLI version of mod2smp by Tomasz Muszynski (Hali/Union) which allows you to 'bounce' down sections of a module to flat sampledata, which you can then load right back into Protracker. This is great for using multiple Protracker tracks to create some complex pad chord, sting or polyphonic drum pattern, then converting it all to a single mono sample that only uses one track in your module. Like everything, it's a tradeoff between filesize, flexibility and quality. Type mod2smp.cli without any arguments to see its built-in help, which gives you instructions and examples.

The only other thing to mention is that I added a folder of small chipsamples to the root of the disk, and set that folder as the default samples directory in Protracker's config. So it might be a fun way to get started with chiptracking on Amiga: just boot this image, maybe find some Protracker tutorials, and away you go!

Cheers,

Syphus / Up Rough
