# 7/10/2026 - It Works!

_Time Spent: 6hr_

Final stretch before the deadline and got ready to cut! First I had to fix a lot of sag issues with the Z axis and used spring washers to fix it. I am pretty impressed with how far it's come with 3D Printed PLA but the limits are starting show up with the flex on skinner parts (X mounting brackets for example). Ideally these should get recut in aluminum but that's for later.

Went and did some research on how to get this setup and bought a 1/4" bit for the spindle/router and a 2x4ft slab of 1/4" MDF. Used a circular saw to cut it to a size that would fit in the machine. While I intend to use more aluminum extrusions to mount the a better 1/2" baseplate, for now I'm just clamping and drilling the piece onto the frame of the machine. 

![](photos/IMG_3550.png)

Wrote some basic G-Code and cut it! (video sped up 2x)

There are some immediate issues (corners are bad because the two Y rails are out of sync and lag behide due to PLA flexing) but I'm so happy with this project and am amazed I even got this far. This was such a fun project and taught me so much about CAD, CNC machines, wood/metal working, and so much more!

# 7/10/2026 - Software Configuration

Messed with motor parameters for speed and power and whatnot. Motors were getting pretty hot and I started investigating. I then noticed the Y axis was spinning *extremely* slowly compared to the other axes. After some research it turns out there is a grblHAL bug for my board. I also wanted to enable some extra features (current limiting for example) that the web builder didn't give me. I cloned the repo, patched it a bit and then rebuilt the firmware. Flashed it and it works! Dialed in motor values and its working great! (Sorry no image, look at next post)

# 7/9/2026 - More mounting and Cabling

_Time Spent: 4hr_

With almost all the issues fixed, I assembled the full machine more or less. It's not perfect (electronics aren't mounted, lot's of parts are sagging) but will be good enough for getting the machine running. Honestly not much to say, just lots of assembly.

![](photos/IMG_3547.png)

# 7/8/2026 - Motherboard + Electronics

_Time Spent: 2hr_

I assembled the motherboard/RPi case. I started out by realizing my USB slots weren't big enough for the thick USB cables I was using. Just sanded them and it fits now. Then I put a couple M3 inserts in and mounted the motherboard and fan. Unfortunatly, I realized to late that the RPi Zero does not use M3 screw. My solution? Drill through the RPi

![](photos/IMG_4927.png)
![](photos/IMG_4929.png)
![](photos/IMG_4928.png)

If it works it works I guess. Also installed CNC.js on the RPi and started learning how to use it.

# 6/30/2026 - X Axis Reprint

_Time Spent: 1hr_

I noticed this earlier but theres a design mistake on the X axis where the linear rail collides with a 3D print and the stepper mount also blocks the stepper itself. After a reprint it's fixed. (Sorry no picture)

# 6/28/2026 - Ball Screws

_Time Spent: Way too long_

Not exactly a journal entry but a prolonged painful experience I had from June 19-July 8. I went to mount the ball screw for the X axis only to discover the ball screw was extremely hard to turn and made a grinding noise when I tried. I tried lubricating it and a bunch of other things with no succcess. I quickly reached out to customer support and was told to wait 48 hours. In the meantime I read online that VEVOR (the company I for the ball screw from) has *horrendous* customer support. After 48 hours, I got no response and sent a follow up. Another 24 hours later I tried to send a follow up but it didn't let me. I opened a new ticket referencing the old one and mentioned that I'd file a chargeback with HCB if I didn't get a response. 

I almost immediately (2hrs) got a response on the original ticket after that. They suggested adjusting the tension screw on the ball screw. Wow, that's actually helpful and I'm pretty stupid for not doing that originally. Guess what? There is no tension screw. It's nowhere on the part and no manual online says anything about one. I replied with the same info and didn't get a response for a while. I decided to just reach out to HCB for a chargeback where they suggested asking the Stasis team. The Stasis team (Meghana) was super helpful and topped up my grant to get a new ballscrew. Moral of the story: never buy from VEVOR.

# 6/28/2026 - Z Axis Mounting

_Time Spent: 1.5hr_

Mounted linear rails for X axis and got the Z axis mounted. Made a design mistake where the X axis didn't leave enough counterbore for the screws but fixed with a reprint.

![](photos/IMG_4923.png)
![](photos/IMG_4924.png)

# 6/28/2026 - Frame Assembly

_Time Spent: 3.5h_

Reprinted parts (in blue this time!) and got enough to assembly the base frame of the Y axis. Also had to buy some longer screws from Home Depot which was unfortunate since they were $4 each. 

![](photos/IMG_4842.png)
![](photos/IMG_4843.png)

Also started work on the X gantry

![](photos/IMG_4845.png)


# 6/28/2026 - Power Supply

_Time spent: 1h_

Got the PSU case printed and disassembled the Ender 3 stock case. Assembled it and tested, works great.

![](photos/IMG_4839.png)

# 6/25/2026 - Spray Painting

_Time spent: 1h_

Had to take a break from assembly to wait for prints to finish and parts to arrive. I wanted a black and blue look for the machine, but it's currently silver and rainbow...

Thought I could at least get the black part and bought some spray paint. After sanding and putting several coats I ended up with an extremly shabby paint job which I'll fix Soon™. 

![](https://cdn.hackclub.com/019f4ff5-ec86-76c7-932a-4e00093f5433/IMG_2548.jpeg)

![](https://cdn.hackclub.com/019f4ff7-8381-77c7-b8c2-7eb18428c544/IMG_4783.jpeg)

# 6/24/2026 - Cutting Z Axis

_Time spent: 3.5h_

Continued working on Z axis. The linear rails are 600mm but the Z axis needs a shorter 8in one. I went out and bought an angle grinder blade for stainless steel and started cutting (lots of sparks, yikes)

![](https://cdn.hackclub.com/019f4fee-d357-74d5-9d0d-a69bb16660a4/IMG_3471.jpeg)

After that, I assembled the rest of the Z axis with the stepper and it works amazingly.

![](https://user-cdn.hackclub-assets.com/019f4ff2-558e-7bca-9765-0941d6e73df3/IMG_4770.jpeg)

# 6/24/2026 - Parts and Mismeasurement

_Time spent: 1.5h_

More parts arrived, mainly the aluminum extrusions and all Amazon parts. One thing weird was Amazon somehow messed up and shipped a random item for someone else instead of the heated inserts. We sorted it out with Amazon and the inserts are on the way.

With the extrusions, I can start assembling most of the build (except I can't mount the linear rails until the AliExpress order comes).

![](https://cdn.hackclub.com/019f4fea-be2b-77d0-88e3-9b9e0e9099ce/IMG_4762.jpeg)

But then I noticed a pretty big issue. The CAD model I used for the ball screws claimed a length of 600mm. I made a huge mistake by not measuring it in CAD because it is actually 650mm. The actual part is 600mm as it should be, but with that mistake the screws don't reach. I've modifed the design to account for this and am fixing a couple other issues and reprinting.

# 6/18/2026 - Buying Parts and 3D Printing

_Time spent: 3.5h_

A few things changed since I made the BOM. First off, AliExpress had a few deals I was relying on expire. This bumped the price a lot, so I got some alternatives of a similar price. More importantly, Harbor Freight's compact router went out of stock online. Luckily, it was in stock at their store in Fremont, CA. I live in the Bay Area and it wasn't too far. So I went and bought it in person and it's working great.

I'm also starting to 3D print the parts for the machine. I'm not super happy with it, but the only filament I have a full spool of right now is a multi-color pastel one. It doesn't look right on a industrial looking CNC but I'll go with it for now. 


![](https://stasis.hackclub-assets.com/images/1781812386761-7mt9mo.jpeg)

Everything should be arriving pretty quickly (except for the AliExpress items which are obviously shipping from China) so I'll get building very soon.

Also started on the Z axis

![](https://cdn.hackclub.com/019f4fe9-0f97-7812-af87-daf3991e4c45/IMG_4756.jpeg)


# 6/18/2026 - grblHAL Setup

_Time spent: 1.75h_

I started disassembling my Ender 3 and got the motherboard, PSU, and related cables. Then I used https://svn.io-engineering.com:8443/ to get an image of grblHAL that I could flash onto the motherboard. Surprisingly, the exact motherboard I was using was a preset option so it looks like someone else has had this idea too.

After flashing, I connected a USB and was able to communicate with grblHAL over serial. I started learning basic commands and got a motor moving. I was super surprised how easy the whole process was.

![](https://stasis.hackclub-assets.com/images/1781811955329-urxflm.jpeg)

