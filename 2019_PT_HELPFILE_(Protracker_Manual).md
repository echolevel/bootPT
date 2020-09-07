Updated on 2019-10-29 by Brendan "Syphus"
Ratliff (@echolevel).
This is a work in progress -
I'll incorporate details of any significant
changes by 8bitbubsy for his 2.3e and 2.3f
versions of Protracker, and tweak
the formatting a bit for readability.

========================================

ProTracker V2.3d   Oct. '94
===========================

**(C) 1992 Mushroom Studios
This program is Public Domain**


**Written by: Peter "CRAYON" Hanning**

Hi there music lovers!

Here comes PT2.3d, a new version of
ProTracker, the best tracker around!

There has been several new changes this
time to enhance ProTracker even more!
Read more about it in the Readme! file.
Don't hesitate to contact us if you
can't get it working, if there's some-
thing you can't figure out or if you
find any bugs.


Some technical info:

Sourcecode: 440k / 25000 lines
Main Program: 200k
GFX data: 80k (packed)

Something you'd like in the next
version of ProTracker? Have you
found any bugs? Anyway, write to:

     Mushroom Studios/Noxious
     Vinterstigen 12
     14440 Ronninge
     Sweden

(No games, please!)

Mushroom Studios are:

* Peter "CRAYON" Hanning (Code,Music)
* Anders "DOLPHIN" Ramsay(Music,Organize)
* Daniel "KNOTIS" Sindahl(Code)

Greetings to:
* All members of Noxious
* Tritoon/Alpha Flight - Matrix/LSD
* Devistator/EOC1999 - T.G.L./Aliens
 * Spirou/Visual Design - Alex Kunz
* Sun/Dreamdealers - Deltabar Dilonardo
* Markus Jentsch - Tal/Majic12
* Sebastien Rose - Toni Maenpaa

*This space is for rent*


MAINSCREEN
==========

#### PLAY ####
Will play the song from the current
position in the song. The pointer
turns yellow, just to show you what's
going on.

#### PATTERN ####
Will play the current pattern which
is shown at the bottom of the screen.
The pointer turns yellow here as well.
Holding down the right button while
pressing play,pattern or record will
play from the current patternposition.

#### EDIT ####
Will put you in edit mode. The pointer
turns blue, and you can enter notes
and numbers from the keyboard. Use
the arrowkeys to move up/down and
left/right in the pattern. Entering
a note or a number will cause the
pattern to jump one or more slots
down.

#### RECORD ####
Will put you in edit mode, but also
play the current pattern or song. You
can select this in the Edit Options
menu. While the pattern or song is
playing, you can type in notes and
numbers from the keyboard, and they
will appear in the pattern as it
scrolls. The notes and numbers will
also be quantized to the nearest slot,
so that keeping a steady rhythm is no
problem. The pointer will turn blue
here as well as in the the normal edit
mode.

#### STOP ####
Will stop playing of songs and patt-
erns, recording, and will turn edit
mode off.

#### CLEAR ####
Will first ask you what you want to
clear. You can clear either all, song
or samples.Patternnames are cleared
together with the song.

#### EDIT OP. ####
Will exchange the Spectrum Analyzer
with the Edit Menu(s). Pressing more
than one time will browse through the
edit op. screens.

#### DISK OP. ####
Will go to the File Requester.

#### PLST ####
Will go to the PLST screen.

#### PSET-ED ####
Will go to the preset editor.

#### SETUP ####
Will go to the Setup Screen.

#### SAMPLER ####
Will go to the Sampler screen.

#### 1, 2, 3 and 4 ####
Represent the audiochannels of your
amiga. When lit, that channel is on.
When not lit, the channel is muted and
the notes in that track will not be
played.Holding the right mousebutton
will solo the desired channel.

#### TEMPO ####
The tempo gadget on the status bar is
for setting the CIA speed, if CIA
timing is used. The gadget will be
updated every time you set the speed
using the F command (if CIA that is).

#### I(NSERT) ####
Insert a position into your song.

#### D(ELETE) ####
Delete a position from your song.

#### POS ####
Defines your position in the songtable.
Pressing POS wil put you in the
Position-Editor.

#### PATTERN ####
Defines which pattern will be played at
a specific position.

#### LENGTH ## (SONG)
Defines the length of the song.

#### FINETUNE ####
Tune your untuned samples to match the
others.

    0 436.4 hz    -1 432.1 hz
    1 439.0 hz    -2 429.6 hz
    2 441.6 hz    -3 426.3 hz
    3 445.1 hz    -4 423.1 hz
    4 447.8 hz    -5 419.9 hz
    5 451.5 hz    -6 416.7 hz
    6 455.2 hz    -7 414.4 hz
    7 457.0 hz    -8 412.0 hz

#### SAMPLE ####
Choose sample. You can use up to 31, or
hex $1F samples in a song. Pressing
both mousebuttons at the same time will
set the samplenumber to zero. You can
then record the pattern with sample 0
to prevent ProTracker from setting the
volume each time you play a new note.

#### LENGTH ## (SAMPLE)
The Length gadgets are simply used for
setting the length of the sample. A
sample can be up to 64k, or $fffe long.
You can add workspace behind the sample
by increasing the length and letting go
of the button. PT will ask if you are
sure, and if you are, allocate more
memory for the sample.

#### VOLUME ####
Use this to set the volume the current
sample will be played with.

#### REPEAT ####
Here you set the start of the sample-
loop.

#### REPLEN ####
Here you set the length of the sample-
loop.

#### PATTERNNUMBER GADGET ####
To the middle left of the screen is a
box with a number in it. The number is
the current pattern number. Click on it
to type in a new number.

When in type-
in mode, use return, ESC or right mouse-
button to exit. This should also work
on most other such gadgets.

#### A(BOUT) ####
This one you'll have to experience for
yourself.

#### LOAD ## (sample)
Will simply try to load the current
samplename. Use this when you've fucked
up in the sample editor, and have
destroyed a sample.

Pressing both the left and right button
on the arrow-gadgets will speed them up
a bit. All numbergadgets except Fine-
tune&Sample allows you to click in the
gadget and type in the desired value.
Holding the right mousebutton while
pressing them will zero the value.

The main screen has some indicators on
the left side of the song- and sample-
name textgadgets.The indicators are as
follows:

    M S M 0-9 (Metronome ON, Split ON, Multi ON, Editskip)
    I 0-9     (AutoInsert ON, AutoInsertMacro)

DISK OP 1
========
#### PATH ####
The paths for songs, modules, samples,
tracks and patterns can now be changed,
and they can be up to 31 characters
long. To change path, click on load
song/module/sample/track/pattern or the
arrow indicating what path you're at.

#### FREE (DISKSPACE) ####
Free diskspace can be shown in hex or
decimal. Select this on the setup
screen. Click on "free" to get free
diskspace without re-reading the dir.
#### FORMAT DISK ####
Will format a disk in df0:

#### RENAME FILE ####
Will dir the current directory. Select
a filename, and you will be able to
edit the name.

#### DELETE FILE ####
Will dir the current directory. Select
a file, and it will be deleted from the
disk.

#### PACK ####
When on, ProTracker will pack songs
before saving. Modules will be Power-
Packed and .pp will be added to the
filename.

#### LOAD SONG ####
Will dir the songs path. Select a song,
and it will be loaded and decrunched if
crunched.

#### SAVE SONG ####
Will pack the song if pack is on, then
save it to the current songs path.
Remember to enter a name for your song,
otherwise PT will not save!

#### LOAD MODULE ####
Will dir the modules path. Select a
module, and it will be loaded. Power-
packed modules will be decrunched.

#### SAVE MODULE ####
Will crunch(Powerpacker) the module if
pack is on,then save it to the current
modules path. Holding the right mouse-
button will save as an executable file
in the current directory.

#### LOAD SAMPLE ####
Will dir the sample path. Select a
sample, and it will be loaded to the
current sample. IFF headers will be
chopped off and loops loaded, if any.
Powerpacked samples will be loaded and
decrunched.

#### SAVE SAMPLE ####
Will save the current sample as RAW,
IFF or PAK(Powerpacked). Select this
in the "Save" gadget to the right of
"Load Sample". IFF loops will be saved
too(Not with PAK in this version).

#### DIR-BROWSE BUTTON ####
By pressing this button you can browse
through various preset paths, so that
you won't have to enter them over and
over again.Holding right mousebutton
will show all paths in the filewindow.

#### PATH INDICATOR ####
Click to change paths without reading
dir.

#### T(OP) ####
Will put you at the top of the file-
list.Holding the right mousebutton will
put you at the previous character in
the file-list.Try it out!

#### B(OTTOM) ####
Will put you at the bottom of the file-
list.Holding the right mousebutton will
put you at the next character in the
file-list.

Holding shift while pressing a key will
put you in the list at the chosen
position. This works in the PLST and
Preset-Ed screens as well.



Disk Op 2
=========

Disk op.2 has alot in common with disk
op.1 but with a few additional features

#### LOAD TRACK ####
Will dir the track path.Select a track,
and it will be loaded to the cursor
position or to the trackbuffer,
depending on the MODE choice.

#### SAVE TRACK ####
Will save the track from the cursor
position or from the trackbuffer.

#### LOAD PATTERN ####
Will dir the pattern path. Select a
pattern, and it will be loaded to the
cursor position or to the patternbuffer

#### SAVE PATTERN ####
Will save the pattern from the cursor
position or from the patternbuffer.

#### MODE ####
Determines if the track/pattern will
load/save to/from the buffer or the
cursor position.


**AutoDir** - If you set the autodir toggle
on the setup screen to on, ProTracker
will automatically dir the current path
when you enter the disk op. screen and
after you've saved/renamed/deleted
something.

**AutoExit** - When this toggle is on Pro-
Tracker will exit from disk op. when
loading a song/module/track or pattern.

PLST
====

The PLST is fairly simple to use.
Listed here are all the samples in your
Presetlist and their lengths.Just click
on a name, and ProTracker will ask for
a disk called ST-01 through to ST-FF.
Insert it, and the chosen sample will
be loaded to the current sample dis-
played at the left of the screen. Use
the up/down arrow keys to move up and
down in the PresetList. If you press
shift or the right mousebutton,the PLST
will move 10 presets at a time.

At the top the PLST shows the total
number of samples from the selected
sounddisks.There are some PLST gadgets:

#### CLEAR ####
Will clear all the sounddisk names you
have entered, and display the whole
PresetList.

#### MOUNTL(IST) ####
Will search your drives for disks
called ST-\*\*, and put the names into
the ST-__ gadgets. ST-00 will not be
mounted.

#### ST-__ ####
There are three ST-__ gadgets where you
can enter the numbers of the sounddisks
you want to display in the PLST. Only
the presets from the selected sound-
disks will be shown. If you clear all
gadgets (by pressing return or right
mousebutton), or press "Clear",the PLST
will revert to show all presets.

#### T(OP) ####
Will put you at the top of the preset-
list.Holding the right mousebutton will
put you at the previous character in
the preset-list.
#### B(OTTOM) ####
Will put you at the bottom of the
preset-list.Holding the right mouse-
button will put you at the next
character in the preset-list.

#### EXIT ####
There are 2 exitgadgets in this version
I didn't know what to change the other
exitgadget to.

Holding shift while pressing a key will
put you in the list at the chosen
position. This works in the DiskOp and
Preset-Ed screens as well.

PRESET ED
==========

The preset editor is used for sorting
and catalogueing your samples. All
samples for use with ProTracker should
be on disks called "ST-01" to "ST-FF".
When adding a disk to the presetlist,
only these disks are recognized.

Harddisk owners may want to add a
directory. e.g. You've got a directory
called "Supersamples", and you want to
use the samples on PT... Simple. Assign
"Supersamples" to ST-13 or whatever. In
the box with "Disk:" and ST-__ in it,
enter ST-13.Now type "DHX:supersamples"
in the path box and press "add path".

The path will be added as ST-13 in your
presetlist, so everytime you need a
sample from ST-13, it will be loaded
from "Supersamples" instead. Simple?

**Editing**

To edit a preset, simply click on it.
Use the arrowkeys to move left/right.
When moving up and down in the preset-
list, use shift or the right mouse-
button to speed it up a bit.
#### ADD PATH ####
Will add the current path to the
presetlist.Infofiles will not be added.
Samplenames can only be 15 chars long.

#### INSERT PRESET ####
Will create a new preset.Enter the data
for the sample, and it will be added to
the presetlist.

#### DELETE PRESET ####
Will delete the wanted preset from the
presetlist.


#### DELETE DISK ####
Will delete the disknumber set in the
"Disk:" box.

#### PATH ####
This is where you enter the path to be
added from. It can be up to 31
characters long.

#### DISK ####
This is the disk (or HD-dir) that's
being added from (or deleted).

#### PRESETS ####
This is the current number of presets
in the presetlist.

#### CLEAR PLST ####
Will clear all the presets.

#### LOAD PLST ####
Will load the presetlist from a file
called "PLST". This file should be
placed in the PTdir (See setup2).

#### SAVE PLST #####
Will save the presetlist as a file
called "PLST" to the current PTdir.


#### PRINT PLST ####
Will print the presetlist to the
current print path, shown on the
setup-screen.

#### PLST ####
Will go to the PLST-screen!

#### T(OP) ####
Will put you at the top of the preset-
list.Holding the right mousebutton will
put you at the previous character in
the preset-list.


#### B(OTTOM) ####
Will put you at the bottom of the
preset-list.Holding the right mouse-
button will put you at the next
character in the preset-list.

Holding shift while pressing a key will
put you in the list at the chosen
position. This works in the PLST and
DiskOp screens as well.





SAMPLER
=======

#### Editing ####

When editing a sample, use the mouse to
set the cursorline and to mark ranges.

#### WAVEFORM ####
Will play the full sample with loops.

#### DISPLAY ####
Will play the part of the sample being
shown on screen.


#### RANGE ####
Will play the marked range.

#### STOP ####
Will stop all playing of samples.

#### SHOW RANGE ####
Will magnify the current range and
display it.

#### SHOW ALL ####
Will display the whole sample.

#### BEG ####
Will put the cursorline at the begin-
ning of the sample.

#### END ####
Will put the cursorline at the end of
the sample.

#### SWAP BUFF(ER) ####
The swap the current sample with the
copy-buffer.

#### ZOOM OUT ####
Will show double the range you are dis-
playing.


#### RANGE ALL ####
Will range the part of the sample being
displayed on screen.

#### CUT ####
Will cut away the part of the sample
that's marked.

#### COPY ####
Will copy the marked range to the copy-
buffer.

#### PASTE ####
Will paste the copy-buffer into the
current sample.

#### The volume box ####

Set the "FROM" and "TO" volume
percentages by using the sliders, or
just type in any number you please
(from 0 to 200) in the percentage boxes
to the right.

#### NORMALIZE ####
Will find the highest volume settings
possible (without clipping).

#### CANCEL�####
Will exit the volume box.

#### \ ####
Will set the percentages 100%-0%

#### / ####
Will set the percentages 0%-100%

#### - ####
Will set the percentages 100%-100%

#### RAMP ####
Will ramp (calculate) the volume!

#### TUNETONE ####
Will create a sinus sound, which you
can tune your samples after. See
setup 2 help for details.

#### SAMPLE ####
Will first enter the monitor screen.
Now click right button to sample, left
to exit.The pointer will be green when
waiting for diskactivity to stop.

#### NOTE ####
This is the note to sample on. Range is
C-1 to B-3.

#### RESAMPLE ####
Here's a step-by-step explanation:
1. Turn on the tuning tone.
2. Use the keyboard to find what note
  it is. Use finetune if needed.
3. Enter the note in the "Note:" box to
  the right.
4. Press resample!

#### NOTE ####
This is what note to resample to.

#### DISP(LAY) ####
This is the length of the part of the
sample being shown on screen.

#### LOOP ON/OFF ####
This is for turning loops on/off
without having to fiddle with the
repeat and replen gadgets.

#### EXIT ####
Exits the sampler screen.










SETUP 1
=======
The setup screens were provided so that
PT users could set up their own
personal environment. We hope we have
satisfied most of you. You've got 8
on/off toggles,a split keyboard editor,
a color palette and lots more. Choose
what you want, and use "Save Config" to
save your environment. On the next
screen is a list of what will be saved
in the config file.



**This will be saved in the config file:**

* Songs/Modules/Samples/Tracks/Patterns and Print paths & savemode
* Colors
* Keyrepeat
* The 24 On/Off toggles
* Split
* Keyboard data
* Keyrepeat
* Accidental
* The eight external dos commands
* Max PLST entries
* Multikey channeltable
* Effectmacros
* CIA/VB timing
* Tempo & Speed
* DMA wait
* Tunetone+Volume

You can have up to 256 different config
files. They will be saved as
"PT.config-00", "PT.config-01" and so
on. Set the confignumber in the
"cnfig" box.

#### LOAD CONFIG ####
Will load the selected config file.

#### SAVE CONFIG ####
Will save the selected config file.

#### RESET ALL ####
Will set the original PT defaults and
colors.

#### MULTI ####
This table is used with the multi
keyboard option.The four numbers repre-
sent what channel each channel will
jump to next. 1-2, 2-3, 3-4 and so on.

#### THE DOT ####
The gadget with a dot and a textline
can be used to execute dos commands.
Each of the 8 commands can be up to 31
letters long. Pressing the dot will
browse through the commands. Holding
the right button and pressing it will
execute the command. Note that PT needs
the command "run" to execute the other
commands.This is because of commodore's
stupid programming of the dos library
function "execute". Type "endcli" to go
back to ProTracker.


#### THE COLOR PALETTE ####
The color palette is simple to use.
Just select a color, and use the R,
G and B sliders to set the color.

#### UNDO ####
Will put back the latest change.

#### CANCEL ####
Will set the config colors.

#### DEF(AULT) ####
Will set the original ST colors.


#### SPLIT ####
You can set 4 splits on the keyboard,
each with it's own sample, splitpoint
and transpose. Just type in a sample
number and select the key to split at
by pressing the appropriate one. The
transpose note for each split is the
first note in that split-range. Notes
below the first split will be played
with the current sample. Split is great
for recording drums, or for playing
untuned samples in tune (use together
with finetune).


#### CLEAR ####
Will clear the splits.

#### KEYREP(EAT) ####
The first number is the keyrepeat delay
and the second is the speed.

#### ACCIDENTAL ####
Simple enough, accidental allows you to
select sharp (#) or flat (�) notes.
This will not be saved with the song!

#### PRINT SONG ####
Will print the song to the path shown
below the "Print Song" gadget.The print
path can be 31 chars long.

#### SPLIT ON/OFF ####
Toggles between normal and split key-
board.

#### FILTER ON/OFF ####
Toggles the audiofilter / PowerLED.
(Not available on all Amigas)

#### TRANS(POSE)DEL(ETE) ON/OFF ####
When on, notes transposed out of range
will be deleted.


#### SHOWDEC(IMAL) ####
When on, Freemem, Tunemem, and file-
lengths will be shown in decimal.

#### AUTODIR ON/OFF ####
When on, ProTracker dirs the current
directory path automatically.

#### AUTOEXIT ON/OFF ####
When on, ProTracker will automatically
exit from the file requester when
loading a song,module,track or pattern.

#### MOD. ONLY ON/OFF ####
When on, ProTracker will only show
modules beginning with "mod.".

#### MIDI ON/OFF ####
Enables midi input (see midi help).

#### 2 ####
Will enter SETUP 2.


SETUP 2
=======

#### TIMING ####
We included this so that American users
also could enjoy ProTracker, and
wouldn't have to use sonix or any other
terrible music program...

You can choose between CIA or Vblank
timing. Vblank is the timing-method
soundtrackers have been using since the
dawn of time, while CIA is a much
better and accurate timing with the
tempo measured in beats per minute.
Using Vblank on NTSC amigas will cause
the song to play 20% faster. With CIA,
there's no difference.

#### TEMPO ####
This is where you set your default CIA
timing tempo. Range: 32-255.

#### SPEED ####
This is where you set your default
Vblank timing speed. Range: 01-FF.

#### COPPER EDITOR ####
The copper editor is for altering the
colors of the VU-meters and the
spectrum analyzer to your own liking.
Select a color by clicking somewhere
within the coppered stripe. Now use the
R, G and B sliders to alter the color.

#### SPREAD ####
Will create an even gradient between
the current color and the one you click
on next.

#### ARROWS ####
Will rotate the whole copper stripe in
the Y-axis (up/down).

#### UNDO, CANCEL and DEF(AULT) ####
Will work just like in the palette in
SETUP 1.

#### MODS ####
This is where you set your default
modules path.

#### SONGS ####
This is where you set your default
songs path.

#### SAMPL(ES) ####
This is where you set your default
sample path.


#### PTDIR ####
This is the path for the helpfile, the
PLST and the PT configfile(s).

#### MAX PLST ####
This is the maximum number of presets
in your presetlist.

#### DMA WAIT ####
Use this on fast amigas to slow down
the DMA enough to not miss any notes.
If you set a too low value, you will
miss some of the low notes! If you set
a too high value, everything will be
slowed down. 300 or a little less is ok
on a normal A500 7.09 MHz (PAL). 900
(approx.) is ok on an A3000 running at
25Mhz.

#### TUNING TONE ####
The tuning tone is for use with the
sample editor. The note is what note
to play the tuning tone at, and the
number is the volume.

#### COUNT IN ####
Doesn't work..YET..sorry...

#### <- DEFAULT ####
Will put back the default for every-
thing in the middle column.

#### OVERRIDE ####
When on, PT will ignore any paths or
disknames when loading a song or
module. All the samples will be loaded
from the current sample path.

#### NOSAMPLES ####
When on, PT won't load the samples when
loading a song or module.

#### BLANKZERO ####
When on, PT won't show the first zero
in the samplenumber.

#### SHOW DIRS ####
When on, directories will be shown in
Disk Op.

#### SHOW PUBL(IC) ####
When on, PT will show all free memory,
not just chip-mem.

#### CUT TO BUFF(ER) ####
When on, all samples cut in the sample
editor will to put in the copy-buffer.

#### LOAD LOOP ####
When on, PT will load loops from IFF-
samples.

#### SYS(TEM) REQ(UESTS) ####
allows you to turn the requests on/off

#### 1 ####
Will enter SETUP 1.

#### SALVAGE ####
doesn't work yet.

#### 100 PATTERNS ####
with this on, you will be able to have
100 patterns.

#### SAVE ICONS ####
When on, PT will save an icon together
with the module.

#### LOAD (PATTERN)NAMES ####
When on, PT will try to load the
patternnames with the module.

#### SAVE (PATTERN)NAMES ####
When on, PT will save patternnames
with the module.

#### LOAD PLST ####
When on, PT loads PLST when starting.

#### SCREEN ADJUST ####
When on, PT will scroll the screen 16
pixels to the left.

#### SAMPLEPAK ####
allows you to pack samples as IFF or
RAW.

You can now have modules with 100
patterns. If you save a module with
more than 64 patterns then M.K. in
the moduleheader will be changed to
M!K!


MIDI
====

Midi routines in ProTracker 2.3d are
still very limited. Midi in should work
ok, though. To activate midi, you'll
have to turn it on on the setup1
screen. Use the three upper octaves on
your synthesizer to play notes. Some
keys in the lowest octave can be used
to play/stop/record etc.

We might fix better midi support in
later versions of ProTracker, but so
far, this is uncertain... Read the
PT.ReadMe! file for more info.


POSITION-EDITOR
===============

Press 'POS' on the mainscreen to get to
the Position-Editor. All the gadgets
should be well known, pressing the big
gadget at the top will stop the song.
Keyboard input works too,Left Alt,Left
Amiga,space and the cursor up/down
arrows.You can use the Position,pattern
and length gadgets on the main screen,
or click in the list to alter the
current pattern or to enter a name to
each pattern if you'd like to. The
Patternnames will be loaded/saved if
you have the corresponding toggles ON
(load names,save names). The files will
have the mod. exchanged to mod! just to
distuingish them from the real modules.
The patternnames will be cleared if you
choose clear song or clear all.Another
way is to click on each name you'd like
to clear and then press the right mouse
button. Patternplay works a little
different from in the mainscreen.The
pattern shown on the edit-row(the
current position) will be played
instead of the pattern currently shown
in the notedatawindow.

HEY! The patternnames has no effect on
the module, they are just to remind
the musician of the contents of the
patterns, eg. you can name the first
three patterns to INTRO just to remind
yourself that those three patterns are
the intro to your tune!


EDIT OP.
========

The edit op. screens were just a handy
way for us to implement all the new
functions we had thought of. There are
three screens, and you can browse
through them by pressing the edit op.
gadget more than once, or select one by
clicking on the numbers 1-3.

To exit edit op., click on the gadget
labeled "E" or press ESC.

###Edit op. Screen 1:###

#### TRANSPOSING ####

What is transposing ?

Transposing lets you shift the pitch of
the notes up or down. E.g. Change a C-3
to a C#3.

In comparison to other trackers,
ProTracker lets you transpose in just
about every way you can imagine.You can
transpose either the current sample or
all the samples in a track or pattern.
To the right of the title bar is a
small box with the letter "S" or "A".

    S - Only the current sample will be
       transposed.
    A - All the samples from $00-$1F will
       be transposed.

To toggle between the two, click on the
edit op. title bar.

If the setup toggle "TransDel" is on,
all the notes transposed out of range
(C-1 to B-3) will be deleted. If not,
they will not be transposed.
Edit op. screen 2: (Record)

#### RECORD ####


    PATT - Record current pattern only.
    SONG - When recording, PT will move through the patterns in the song, just like normal play.

#### QUANTIZE ####
Will move the notes you record to every
n'th slot. Entering 00 will turn off
the quantizing, and the notes you play
will always be inserted at the pattern-
position you are at. Entering 01 will
quantize the notes the the nearest slot
according to the speed. i.e. if you
play a note after the first half has
been played, it will be quantized to
the slot below. Entering a value like
8 will quantize to every 8th note, and
so on. Got that?

#### METRO(NOME) ####
The first number is the speed of the
metronome,and the second is the channel
to play it on. The Sample used for
metronomes is always sample $1F. Load
your own favourite metronome sample.The
metronome will always be played at C-3,
but you can still change the volume and
loop values. To turn off the metronome,
just set the speed or channel to 00.
V2.3d: The metronome has got a master
toggle ALT+M.

#### KEYS ####
When MULTI, PT will jump to another
channel after you play a note on the
keyboard. This makes it possible to
play two or more notes at the same time
(very useful with midi). On the setup
screen you can choose what channel to
jump to after playing a note.


### Edit Op. screen 2: (Samples) ###

To the right of the title bar is a
small box with the letter "T", "P" or
"S".

    T - Copy & Exchange apply to current track only.
    P - Copy & Exchange will affect the whole pattern.
    S - Copy & Exchange will apply to the real samples in memory.

To toggle between the two, click on the
edit op. title bar.

#### DELETE ####
Will delete all notes with the current
sample in current track or whole
pattern.

#### KILL ####
Will kill the current sample. That is,
remove it from memory and reset all
sample settings. It will not be deleted
from the track or pattern. You can also
use the period (.) key on the numeric
keyboard to invoke this function.

#### EXCHGE (EXCHANGE) ####
Will exchange the samplenumber shown in
the "FROM" gadget with the samplenumber
in the "TO" gadget and vice versa. "T"
or "P" selects track or pattern. "S"
exchanges the samples.

#### MOVE ####
Will move the samplenumber shown in the
"FROM" gadget to the samplenumber in
the "TO" gadget.


Edit Op. screen 3: (Sample Editor)

To the right of the title bar is a
small box with the letter "H" or "C".

    H - Will halve the volume when mixing and echoing to avoid clipping.
    C - Will not halve the volume. The sample may be clipped.

To toggle between the two, click on the
edit op. title bar.

#### MIX ####
Will mix one sample with another. PT
asks you which two samples to be mixed,
and where to put the result.

Holding the right button and pressing
mix will mix the current sample with
itself. You can offset the sample by
setting a position in the "pos" gadget.
If you set "mod" to a non-zero value,
the sample will also be modulated.

#### ECHO ####
Will create a echo effect on the
current sample. Use "pos" to set the
delay time of the echo.If you want more
room to echo in, just turn up the
length of the sample.

#### BOOST ####
Will turn up the treble of the sample.
Use this on hi-hats and snares!
#### FILTER ####
Will Delta-filter the sample. Use this
on noisy basses.

#### X-FADE ####
Will crossfade the sample (mix with
itself, backwards). Handy for looping
samples that are hard to loop.

#### BACKWD (Backwards) ####
Will turn the sample backwards!

#### UPSAMPLE ####
Will remove every second byte of the
sample, halving the length and shifting
the pitch one octave up.

#### DOWNSAMPLE ####
Will double every byte of the sample,
doubling the length, and shifting the
pitch one octave down.If you downsample
samples longer than $7FFE, you will lose
the end of them.

#### POS ####
This is just an offset in the sample,
used for a lot of things.This one has a
numbergadget as well.Holding the right
mousebutton while pressing the number-
gadget will zero the value.

#### MOD ####
This is used for modulation.Press "MOD"
to modulate the current sample. Holding
the right button while pressing the
numbergadget will zero the value.

#### CUTBEG(INNING) ####
Will chop the number of bytes set in
the "POS" gadget off the beginning of
the sample.

#### FU (Fade Up) ####
Will fade the volume from 0 to 100%.Use
"POS" to select where in the sample to
fade up to.
#### FD (Fade Down) ####
Will fade the volume from 100 to 0%.Use
"POS" to select where in the sample to
fade down from.

#### VOL ####
With this you can change the "real"
volume of the sample. Just set a
percentage and press "VOL".VOL has a
numbergadget. Holding the right button
while pressing it will set the value to
100%.

#### CHORD ####
Will put you in the Chord-maker.
Edit Op.3 is now intended to be used
with the new sample-editor. If a range
is marked, some of the functions apply
to the range only. If there's no range
marked, the functions will affect the
whole sample. You may also set "POS" by
clicking on the sample and setting the
cursor-line.


Chord-maker
===========

#### Chord ####
Will make the chord, using the current
sample and the notes chosen, and the
chord will be put in the current
sample or a free sample,depending on
your choice (see below)

#### Reset ####
will reset the notes and the length

#### Undo ####
will undo the last change.
(apart from multiple arrow up/down)
#### Length ####
will set the length to the maximum
value, depending on the length of the
original sample and the notes you
choose.This will ofcourse set the ':'
after the 4 lengthdigits (see below)
Holding the right mousebutton will set
the length to the minimum depending on
the notes chosen. '.' will be shown
after the 4 digits. Mixing with the
minimum length will make the sample as
long as the shortest sample of the 4
resampled notes.


#### Major ####
will set a major chord, depending on
the basenote.

#### Minor ####
will set a minor chord, depending on
the basenote.

#### Sus-4 ####
will set a sus-4 chord, depending on
the basenote

#### Length string gadget ####
will wait for you to enter a new
length (not greater than the maxlength
If you want a longer sample then add
more space after the mix has been done.)
The ':' after the 4 digits shows that
the samplelength is set to its maximum!

#### Major7 ####
will set a major7 chord, depending on
the basenote.

#### Minor7 ####
will set a minor7 chord, depending on
the basenote.

#### Major6 ####
will set a major6 chord, depending on
the basenote.

#### Minor6 ####
will set a minor6 chord, depending on
the basenote.

#### 4 notegadgets ####
The upper one is the basenote.If you
press a gadget,PT will wait for you to
press a note.Holding the right mouse-
button will reset the note.

#### 4 Up/Down gadgets ####
will add/sub 1 halfnote from the
current note.Holding right button will
add/sub 1 octave.You can reset the
note by adding past B-3.

#### The 4 rightmost gadgets ####
works just like the edit op gadgets.
1,2,3 takes you to the corresponding
edit option, and E exits

#### The statusline ####
pressing the upper line will toggle
between New or Old sample: If N, then
PT will search for an free sample to
put the result. If O, then PT will put
the result on the current sample,
overwriting the original sample.

**Note1!**

This version of PT resets repeat and
replen. PT also puts a '!' last in the
samplename to show you that this is a
chord sample.The '!' is for you to see
where the destination-sample has gone,
it has nothing to do with the program.
You can take the '!' away and rename
the sample to ...-major, ...-minor etc
for instance.

**Note2!**

The chosen option on the statusline in
edit op. 3 ,H(alve) or C(lip) will
affect the chord resampling and mixing



EFFECT COMMANDS
---------------

Effect commands on ProTracker should
be compatible with all other trackers.

|Command | Result |
|---------|---------|
| 0 | None/Arpeggio |     
| 1 | Portamento Up   |    
| 2 | Portamento Down   |  
| 3 | TonePortamento      |
| 4 | Vibrato             |
| 5 | ToneP + VolSlide    |
| 6 | Vibra + VolSlide    |
| 7 | Tremolo        |
| 8 | * NOT USED * |
| 9 | SampleOffset |
| A | VolumeSlide |
| B | PositionJump |
| C | Set Volume |
| D | PatternBreak |
| E | Misc. Cmds |
| F | Set Speed    |  

E - COMMANDS
------------

The E command has been altered to
contain more commands than one.

| Command | Result |
|------------|----|
| E0 | Filter On/Off |      
| E1 | Fineslide Up    |    
| E2 | Fineslide Down    |  
| E3 | Glissando Control   |
| E4 | Vibrato Control     |
| E5 | Set Finetune        |
| E6 | Patternloop         |
| E7 | Tremolo Control     |
| E8 | * NOT USED * |
| E9 | Retrig Note |
| EA | FineVol Up |
| EB | FineVol Down |
| EC | NoteCut |
| ED | NoteDelay |
| EE | PatternDelay |
| EF | Invert Loop |

Cmd 0. Arpeggio [Range:$0-$F/$0-$F]
-----------------------------------
Usage: $0 + 1st halfnote add
         + 2nd halfnote add

Arpeggio is used to simulate chords.
This is done by rapidly changing the
pitch between 3(or 2) different notes.
It sounds very noisy and grainy on
most samples, but ok on monotone ones.

Example:

      C-300047  C-major chord: (C+E+G  or C+4+7 halfnotes)
      C-300037  C-minor chord: (C+D#+G or C+3+7 halfnotes)

Cmd 1. Portamento up [Speed:$00-$FF]
------------------------------------
Usage: $1 + portamento speed
Portamento up will simply slide the
sample pitch up. You can NOT slide
higher than B-3! (Period 113)

Example:

    C-300103  1 is the command, 3 is the portamentospeed.

NOTE: The portamento will be called as
many times as the speed of the song.
This means that you'll sometimes have
trouble sliding accuratly. If you
change the speed without changing the
sliderates, it will sound bad...

Cmd 2. Portamento down [Speed:$00-FF]
-------------------------------------
Usage: $2 + portamento speed

Just like command 1, except that this
one slides the pitch down instead.
(Adds to the period).

You can NOT slide lower than C-1!
(Period 856)

Example:

    C-300203  2 is the command, 3 is the portamentospeed.


Cmd 3. Tone-portamento [Speed:$00-$FF]
--------------------------------------
Usage: Dest-note + $3 + slidespeed

This command will automatically slide
from the old note to the new.
You don't have to worry about which
direction to slide, you need only set
the slide speed. To keep on sliding,
just select the command $3 + 00.

Example:

    A-200000  First play a note.
    C-300305  C-3 is the note to slide to, 3 the command, and 5 the speed.

Cmd 4. Vibrato [Rate:$0-$F,Dpth:$0-$F]
--------------------------------------
Usage: $4 + vibratorate + vibratodepth

Example:

    C-300481  4 is the command, 8 is the speed of the vibrato, and 1 is the depth of the vibrato.

To keep on vibrating, just select
the command $4 + 00. To change the
vibrato, you can alter the rate,
depth or both. Use command E4- to
change the vibrato-waveform.


Cmd 5. ToneP + Volsl [Spd:$0-$F/$0-$F]
--------------------------------------
Usage: $5 + upspeed + downspeed

This command will continue the current
toneportamento and slide the volume
at the same time.Compatible with NT2.0.

Example:

    C-300503  3 is the speed to turn the volume down.
    C-300540  4 is the speed to slide it up.


Cmd 6. Vibra + Volsl [Spd:$0-$F/$0-$F]
--------------------------------------
Usage: $6 + upspeed + downspeed

This command will continue the current
vibrato and slide the volume at the
same time. Compatible with NT 2.0.

Example:

    C-300605  5 is the speed to turn the volume down.
    C-300640  4 is the speed to slide it up.


Cmd 7. Tremolo [Rate:$0-$F,Dpth:$0-$F]
--------------------------------------
Usage: $7 + tremolorate + tremolodepth

Tremolo vibrates the volume.

Example:
    C-300794  7 is the command, 9 is the speed of the tremolo, and 4 is the depth of the tremolo.

To keep on tremoling, just select
the command $7 + 00. To change the
tremolo, you can alter the rate,
depth or both. Use command E7- to
change the tremolo-waveform.

Cmd 9. Set SampleOffset [Offs:$00-$FF]
--------------------------------------
Usage: $9 + Sampleoffset

This command will play from a chosen
position in the sample, and not from
the beginning. The two numbers equal
the two first numbers in the length
of the sample. Handy for speech-
samples.

Example:
    C-300923  Play sample from offset $2300.


Cmd A. Volumeslide [Speed:$0-$F/$0-$F]
--------------------------------------
Usage: $A + upspeed + downspeed

Example:
    C-300A05  5 is the speed to turn the volume down.
    C-300A40  4 is the speed to slide it up.

NOTE: The slide will be called as
many times as the speed of the song.
The slower the song, the more the
volume will be changed on each note.

Cmd B. Position-jump [Pos:$00-$7F]
----------------------------------
Usage: $B + position to continue at

Example:

    C-300B01  B is the command, 1 is the position to restart the song at.

This command will also perform a
pattern-break (see 2 pages below).

You can use this command instead of
restart as on Noisetracker, but you
must enter the position in hex!


Cmd C. Set volume [Volume:$00-$40]
----------------------------------
Usage: $C + new volume

Well, this old familiar command will
set the current volume to your own
selected. The highest volume is $40.
All volumes are represented in hex.
(Programmers do it in hex, you know!)

Example:

    C-300C10  C is the command, 10 is the volume (16 decimal).



Cmd D. Pattern-break
[Pattern-pos:00-63, decimal]
-----------------------------
Usage: $D + pattern-position

This command just jumps to the next
song-position, and continues play
from the patternposition you specify.

Example:

    C-300D00  Jump to the next song-position and continue play from patternposition 00.
    Or:
    C-300D32  Jump to the next song-position and continue play from patternposition 32 instead.


Cmd E0. Set filter [Range:$0-$1]
--------------------------------
Usage: $E0 + filter-status

This command jerks around with the
sound-filter on some A500 + A2000.
All other Amiga-users should keep out
of playing around with it.

Example:

    C-300E01  disconnects filter (turns power LED off)
    C-300E00  connects filter (turns power LED on)


Cmd E1. Fineslide up [Range:$0-$F]
----------------------------------
Usage: $E1 + value

This command works just like the
normal portamento up, except that
it only slides up once. It does not
continue sliding during the length of
the note.

Example:

    C-300E11  Slide up 1 at the beginning of the note.

(Great for creating chorus effects)


Cmd E2. Fineslide down [Range:$0-$F]
------------------------------------
Usage: $E2 + value

This command works just like the
normal portamento down, except that
it only slides down once. It does not
continue sliding during the length of
the note.

Example:

    C-300E26  Slide up 6 at the beginning of the note.



Cmd E3. Glissando Ctrl [Range:$0-$1]
------------------------------------
Usage: $E3 + Glissando-Status

Glissando must be used with the tone-
portamento command. When glissando is
activated, toneportamento will slide
a halfnote at a time, instead of a
straight slide.

Example:

    C-300E31  Turn Glissando on.
    C-300E30  Turn Glissando off.


Cmd E4. Set vibrato waveform
[Range:$0-$3]
----------------------------
Usage: $E4 + vibrato-waveform

Example:

    C-300E40  Set sine(default)
         E44  Don't retrig WF
    C-300E41  Set Ramp Down
         E45  Don't retrig WF
    C-300E42  Set Squarewave
         E46  Don't retrig WF
    C-300E43  Set Random
         E47  Don't retrig WF


Cmd E5. Set finetune [Range:$0-$F]
----------------------------------
Usage: $E5 + finetune-value

Example:

    C-300E51  Set finetune to 1.

Use these tables to figure out the
finetune-value.

    Finetune: +7 +6 +5 +4 +3 +2 +1  0 -1 -2 -3 -4 -5 -6 -7 -8
    Value:     7  6  5  4  3  2  1  0  F  E  D  C  B  A  9  8

Cmd E6. PatternLoop [Loops:$0-$F]
----------------------------------
Usage: $E6 + number of loops

This command will loop a part of a
pattern.

Example: C-300E60  Set loopstart.

    C-300E63  Jump to loop 3 times before playing on.




Cmd E7. Set tremolo waveform
[Range:$0-$3]
-----------------------------
Usage: $E7 + tremolo-waveform

Example:

    C-300E70  Set sine(default)
         E74  Don't retrig WF
    C-300E71  Set Ramp Down
         E75  Don't retrig WF
    C-300E72  Set Squarewave
         E76  Don't retrig WF
    C-300E73  Set Random
         E77  Don't retrig WF


Cmd E9. Retrig note [Value:$0-$F]
---------------------------------
Usage: $E9 + Tick to Retrig note at.

This command will retrig the same note
before playing the next. Where to
retrig depends on the speed of the
song. If you retrig with 1 in speed 6
that note will be trigged 6 times in
one note slot. Retrig on hi-hats!

Example:

    C-300F06  Set speed to 6.
    C-300E93  Retrig at tick 3 out of 6.

Cmd EA. FineVolsl up [Range:$0-$F]
----------------------------------
Usage: $EA + value

This command works just like the
normal volumeslide up, except that
it only slides up once. It does not
continue sliding during the length
of the note.

Example:

    C-300EA3  Slide volume up 1 at the beginning of the note.



Cmd EB. FineVolsl down [Range:$0-$F]
------------------------------------
Usage: $EB + value

This command works just like the
normal volumeslide down, except that
it only slides down once. It does not
continue sliding during the length of
the note.

Example:

    C-300EB6  Slide volume down 6 at the beginning of the note.


Cmd EC. Cut note [Value:$0-$F]
------------------------------
Usage: $EC + Tick to cut note at.

This command will cut the note
at the selected tick, creating
extremely short notes.

Example:

    C-300F06  Set speed to 6.
    C-300EC3  Cut at tick 3 out of 6.

Note that the note is not really cut,
the volume is just turned down.


Cmd ED. NoteDelay [Value:$0-$F]
-------------------------------
Usage: $ED + ticks to delay note.

This command will delay the note
to the selected tick.

Example:

    C-300F06  Set speed to 6.

    C-300ED3  Play note at tick 3 out of 6.

If you use ED0, the note will be
delayed a little anyway. You can play
the same note on two channels, delay
one, and get a nice flanging effect.

Cmd EE. PatternDelay [Notes:$0-$F]
----------------------------------
Usage: $EE + notes to delay pattern.

This command will delay the pattern
the selected numbers of notes.

Example:

    C-300EE8

Delay pattern 8
         notes before playing on.

All other effects are still active
when the pattern is being delayed.



Cmd EF. Invert Loop [Speed:$0-$F]
---------------------------------
Usage: $EF + Invertspeed

This command will need a short loop
($10,20,40,80 etc. bytes) to work.
It will invert the loop byte by byte.
Sounds better than funkrepeat...

Example:

    C-300EF8

Set invspeed to 8.

To turn off the inverting, set
invspeed to 0, or press ctrl + Z.


Cmd F. Set speed [Speed:$00-$FF]
--------------------------------
Usage: $F + speed

This command will set the speed of the
song.

| Parameter | Result |
|-------|--------|
|Vblank: Range 01-FF | Normal timing |
| CIA: Range 01-1F | Set vblank speeds with CIA timing.|
|CIA: Range 20-FF | Set BPM speeds, range 32-255. |
| Both: Range 00 | STOP song.|

KEYBOARD
========
The keymap on ProTracker is a standard
US keymap. The font has been enhanced
and redrawn a little, so you now have
a lot more special characters than
before. Remember to always use the
left shift and alt, as the right ones
are used for other things.

High notekeys:

          2 3   5 6 7   9 0   =
        Q W E R T Y U I O P [ ]

Low notekeys:

        S D   G H J   L ;
      Z X C V B N M , . /

| Shortcut | Function |
|--------|-----------------------|   
| F1 | Choose lo octave(From C-1 to G-3) |
| F2 | Choose hi octave(From C-2 to B-3) |
| F3 | Cut   (sample) |
| F4 | Copy  (sample) |
| F5 | Paste (sample) |
| shft+F3 | Cut track to buffer |
| shft+F4 | Copy track to buffer |
| shft+F5 | Paste track-buffer to track |
| alt+F3 | Cut whole pattern to buffer |
| alt+F4 | Copy whole pattern to buffer |
| alt+F5 | Paste patt-buffer to pattern |
| ctrl+F3 | Cut commands to buffer |
| ctrl+F4 | Copy commands to buffer |
| ctrl+F5 | Paste cmd-buffer to track |
| F6 | Go to patternposition 0 |
| F7 | Go to patternposition 16 |
| F8 | Go to patternposition 32 |
| F9 | Go to patternposition 48 |
| F10- Go to patternposition 63 |
| shft+F6-F10 | Store current patternposition on selected F-key |
| alt+F6-F10 | Play pattern from the stored patternposition |
| ctrl+F6-F10 | Record from stored patpos |
| Esc | Exit DiskOp/EditOp/PLST/PsetEd/Setup/Help etc... |
| shft+Return  | Insert blank note at cursorposition and move the others down. Notes beyond patternposition 63 will | be lost! |
| shft+Bckspce | Delete note above cursorposition and move the others up. You can NOT do this if you're at patternposition 0! |
| alt+Return    | As above, but with all 4 tracks |
| alt+Backspace | As above, but with all 4 tracks |
| ctrl+Return    | Push cmds one down |
| ctrl+Backspace | Drag cmds one up |
| ctrl+0-9 | Select how many slots PT will jump down each time you insert a note (this is only in Edit-mode) |
| Tab | Move cursor to next track |
| Shft+Tab | Move cursor to prev track |
| alt+cursor right | patternnumber up |
| alt+cursor left  | patternnumber down |
| shft+cursor right | song-position up |
| shft+cursor left  | song-position down |
| ctrl+cursor left  | samplenumber up |
| ctrl+cursor right | samplenumber down |
| BackwardsSingleQuote (The key over TAB, you know?) | Go to CLI |
| Help | Go to help or plst screen |
| shft+Help | Toggle between Help or PLST on Help key |
| Space | Toggle between Stop/Edit-mode |
| < (beside Z) | Kill DMA & Volumes to 0 |
| right Amiga | Play Pattern |
| right Alt | Play Song |
| right Shift | Record |
| Caps Lock | Toggle Keyrepeat on/off |
| Del | Delete note under cursor |
| alt+Del | Delete command only |
| shft+Del | Delete note and command |
| shft+0-9 | Store current command on selected key |
| alt+0-9 | Insert command in current track
| ctrl+A | Toggle channel on/off |
| ctrl+B | Mark block |
| ctrl+C | Copy block to buffer |
| ctrl+D | Delete block, drag notes up |
| ctrl+E | expand track |
| ctrl+F | toggle filter on/off |
| ctrl+G | Boost all samples |
| ctrl+H | Transpose block up |
| ctrl+I | Insert block, push notes down |
| ctrl+J | Join-paste block |
| ctrl+K | Kill to end of track |
| ctrl+L | Transpose block down |
| ctrl+M | Toggle multikeyboard on/off |
| ctrl+N | Re-mark last block |
| ctrl+O | Contract track |
| ctrl+P | Paste block |
| ctrl+Q | Unmute all channels |
| ctrl+R | Restore F6-F10 positions |
| ctrl+S | Toggle split keyboard on/off |
| ctrl+T | swap tracks |
| ctrl+U | undo last change |
| ctrl+V | Filter all samples |
| ctrl+W | Polyphonize block |
| ctrl+X | Cut block to buffer |
| ctrl+Y | Backwards block |
| ctrl+Z | Restore Effects |
' | Autoinsertmacro down |
|  # | Autoinsertmacro up (The key beside return) |
| alt+A | Monitor/Start sampling |
| alt+B | Boost sample |
| alt+C | Toggle channel 3 |
| alt+D | Go to Disk Op. |
| alt+E | Go to Edit Op. |
| alt+F | Filter sample |
| alt+I | Toggle AutoinsertEffect on/off |
| alt+K | Delete current sample/track |
| alt+M | Toggle metronome on/off |
| alt+Q | Quit ProTracker |
| alt+R | Resample |
| alt+S | Go to Sampler screen |
| alt+T | Tuning Tone |
| alt+V | Toggle channel 4 |
| alt+X | Toggle channel 2 |
| alt+Y | Save all samples |
| alt+Z | Toggle channel 1 |
| alt+shift+M | Set metrochannel to current channel |
| alt+"\" | Copy command above cursor to current patternposition |
| alt+"=" | Copy command above cursor to current patternposition and add one to the value. |
| alt+"-" | Copy command above cursor to current patternposition and subract one from the value. |
  |  \ | Toggle keypad mode (dots!) |    
| Return | Step one note forward |
| Backspc | Step 0 note backward |
| Amiga+Backspc | Step 1 note backward |
| Alt+any key on keypad | tune drumpad |

On Numeric pad
---------------

|Shortcut | Function |
|----------|-----------|
| 0 | Select Sample $0 |
| 1st row | Select Sample $1-$4 |
| 2nd row | Select Sample $5-$8 |
| 3rd row | Select Sample $9-$c |
| 4th row | Select Sample $d-$f |
| Just Enter | Select Sample $10 |
| Hold Enter + the other keys | select sample $11-$1F |
| Period (.) | Kill current sample |


Transposing
-----------

|Sample/Track | Sample/Pattern | Function |
|------|-------|------|
| L-Amiga + 1 | L-Amiga + 2 | Note Up
| L-Amiga + Q | L-Amiga + W | Note Down
| L-Amiga + A | L-Amiga + S | Octave Up
| L-Amiga + Z | L-Amiga + X | Octave Down

|All/Track | All/Pattern | Function |
|------|-------|------|
| L-Amiga + 3 | L-Amiga + 4 | Note Up
| L-Amiga + E | L-Amiga + R | Note Down
| L-Amiga + D | L-Amiga + F | Octave Up
| L-Amiga + C | L-Amiga + V | Octave Down



GENERAL INFO
============

Making Music
------------
Any piece of music written with Pro-
Tracker is built up from patterns.
Each pattern is built up from four
tracks, one for each of the amiga's
audiochannels.

A pattern is 64 lines long. The magni-
fied line is always the one you edit.
If you need shorter patterns, use the
patternbreak effect command.

A track is built up like this:

        32  C-3 01 C  20
       /    \_/ | / \_/
      /     /   |     \    
    Pos Note Sample Effect cmd.

The C-3 is the note being played at
patternposition 32. 01 is the sample-
number, and the three last digits are
the effect command, in this case, set
volume to $20 (C-Command, 20-Value).

ProTracker holds a table with info
about the sequence in which the patt-
erns will be played. With the "Pos"
gadget you determine your position in
the table. With "Pattern" you define
what pattern to play at that position.
"Length" defines the total size of the
table. The full sequence of Patterns
is the Song. A song is built up from
up to 64 different patterns, each
being played at up to 128 different
positions.

The small gadgets labeled "I" and "D"
are Insert and Delete. With them you
can Insert or Delete a position from
your song. The length of your song
will be adjusted automatically.
Remember that the length of your song
always must be one more than the last
position, since the first position
is 0.

The "Are you sure ?" requester
------------------------------
In addition to the gadgets, you can
use "Y" or Return for Yes,
and "N" or ESC for No.

The Clear requester
-------------------
In addition to the gadgets you can use
"A" for All, "O" for Song, "S" for
samples and "C" or ESC for Cancel.

The text-input routine
----------------------
Now this is really simple. Clicking on
a textline will enable you to edit it.
Some text lines are longer than they
seem, so use the arrowkeys to scroll
back and forth in the text. The text-
input mode is just like an ordinary
text editor. You can use backspace,
delete, space and such. In text-input
mode you can also use the numeric pad
for entering numbers. Pressing the
right mousebutton will clear the text-
line and exit the editing. Use ESC or
return to just exit.

The numbergadgets
-----------------
Click on them and type in the value
(Hex or Dec).ESC or return aborts.

Passing arguments from Workbench/CLI
------------------------------------
When starting from CLI, you can type a
modulename with a pathname(optional)
as an argument. The modulename will be
added to the modulepath stored in the
current config-file.

E.g. If the modulepath is ST-00:modules
and you pass crap/mod.fake as an
argument, then the module
ST-00:modules/crap/mod.fake will be
loaded.

When starting from Workbench,
you can click on a project icon twice
and the selected module will be loaded
(presuming that the icon's default tool
is PT2.3d. The module will be loaded
from the modulepath in the current
config-file regardless of in which
directory the moduleicon is located.

That is, you can have all modules in a
directory and the icons in another
directory to prevent PT from loading
all .info files into the file-list when
you select LOAD MODULE.

Pressing the moduleicon once, and
holding shift while double-clicking on
the PT2.3d icon also works as above.

Tips 'n tricks
--------------
When inserting, pasting or join-pasting
hold down shift to keep the cursor from
jumping to the end of the block.
e.g. shft+ctrl+P


Holding shift while pressing ctrl+K
(kill to end of track) will kill to
start of track instead.
Holding shift while pressing ctrl+
shift-a will solo the current channel.

Use Esc or right mousebutton to exit
from a lot of things.

Effect tips
-----------
You can set the volume without playing
a note. e.g.

    ---01000

This will set the volume for sample 1
without trigging the note.
Or try trigging the sample and sliding
the volume down. e.g.

    C-301A08
    ---01A08
    ---01A08

This will create a strange arpeggiato
effect, like on "Cream of the earth"
by Romeo Knight / RSI.


Undocumented Features in PT 2.1A (op to 2.3D)
---------------------------------------------
* Type 'lock' on the keyboard to lock Protracker. It asks for a password of up to 8 characters (press ENTER for a password of less than 8 characters), then Protracker is locked until you type the password again. This locks mouse/keyboard input. Handy when being AFK at demo parties!
* Press both left and right mouse buttons on the little dot next to the Disk Op. path gadget. This will list all available disk drives and let you select one of them.
* Press CTRL+ALT+SHIFT+LEFT-AMIGA+DEL - prepares a pattern for the infamous 'backwards play' trick by inverting data.
* Press the empty key next to the <> key (or between L-SHIFT and Z on some keymaps) - kills all playing voices!

Pointer Colors
--------------

* Gray      - Nothin's happening.
* Yellow    - Playing song / pattern.
* Green     - Disk action.
* Blue      - Edit / record.
* Magenta   - Waiting for something (text, number etc.).
* Cyan      - Select entry or delete.
* Red       - Something went wrong.



Drumpad
-------

Use backspace '\' to toggle modes.
One or more dots will appear to
the right of the freemem display.

No dots: Normal keypad.
 1 dot: Drumpad.
2 dots: Drumpad - Edit/Rec possible.

Use Alt + keypad key to set note.
