# Wacom CTC-6110WL review (after 1 year of usage)
## Quick tl;dr for the lazy
- $160
- 240Hz polling rate (faster than most consumer tablets)
  + _I can't feel the hardware smoothing. Am I dumb?_
- Default pen feels nice
- Nice pen compatiblity
- Works with Android phones
- No buttons on the tablet
- **Bad pressure input/Inconsistent pen pressure** (very important to note; bad for drawing if you ask me)
- Unreliable USB-C port
- Eat nibs like crazy

## Intro
Wacom CTC-6110WL (as known as Wacom One M, not to be confused with One by Wacom. _Blame Wacom_) is a tablet from 2023. Pretty new, so I expect the driver to works with modern operating systems (be it Windows 11 or macOS... whatever that is), unlike old tablets with no modern driver support (thankfully, we have OpenTabletDriver to cover this issue!).

I bought this tablet so I can draw something on my laptop, because drawing with a trackpad is a pain, and virtual tablet thing on my phone is just too small (along with high latency, even on USB, plus it have ads that covers a portion of the virtual tablet area). Now it's worth noting that I didn't check the tablet buying guide before I bought it, so yeah, a mistake from my end. Can't do anything about it though.

After a whole year (a.k.a letting the warranty expire), I can finally do a review on this pen tablet.

## What's in the box?
Now it's worth noting that they also offer an option to buy these separately on their e-store. However, I bought an entire box with the following things:

- A tablet (Obviously)
- A pen (Can you believe it? We need a pen to draw!)
- A quick start guide and big warranty notice paper that you probably don't bother to read
- **USB-C to USB-C cable** (Important!!!)
  + If your PC doesn't have USB-C port, you need to buy one, OR use Bluetooth (but then how would you charge your tablet?)
  + USB-C to USB-C means you can also plug it into your Android phone! Not sure about iPhone 15 though...
- 2 pack of 5 nibs (10 nibs in total), as well as nib remover (because you need to remove the nib in order to replace it!)

## Pros
### 240Hz polling rate
Being a Wacom consumer tablet, but this bad boy have much higher polling rate than others from what I've seen. Although the polling rate doesn't matter much when we get higher than 120Hz (since tablets are absolute positioning devices), it might be more responsive as we get faster polling rate.

**However**, you might have to use OpenTabletDriver in order to feel the responsiveness, because the official driver add some latency or something.

_I also noticed some people said this tablet have hardware smoothing; I really don't feel it when using OpenTabletDriver, so that might be a hoax. Or it's just that this is my first time using a tablet, oh well..._

_If you plan on getting this for osu!, my suggestion is... you should look for other tablets, unless you really want 240Hz for $120 more than others._

### Nice default pen
Unlike other pen from other manufacturers (whose tip retracts _a lot_ when you press it against the surface), the pen tip have this kind of "hard feel", almost feel like drawing with pencil. If you have used S-pen on Galaxy Note 5 before then well, this pen is exactly like that S-pen. The grip is kinda like my fineliner.

### Nice surface
The surface have a nice friction; it's like drawing on a matte surface with your pen. I wouldn't call it "feel like drawing on paper with pencil", but if you ask me if it is close enough, then I would say yes. That said, if your nib gets sharp, you should replace it to avoid scratching the surface.

Also, **you should wear glove** when drawing with your hand pressed down against the surface. I made a mistake by not wearing a glove while drawing and now the surface is smooth, which makes drawing lines (or anything requires precision) much harder.

### Works with Android phone
I mean, a consumer tablet that was meant to be used by consumers should works with their devices, no? You can use Bluetooth or USB-C cable, though if I recall correctly, the cursor is completely hidden when you connect to your Pixel phone. It does show up as cursor on my phone though.

### It works with S-pen!!! HUH???
A weird quirk I found. The pen is also compatible with my Note10+ as well, so yeah, I guess I only need 1 pen to rule 'em all!

## Cons
### Bad pressure input/Inconsistent pen pressure
Despite having 4096 pressure points, this tablet might actually be more terrible than my friend's CTL-472, which only have 1024 pressure points. The pen pressure is glitchy; it doesn't smoothly interpolate when I draw in Krita (at least with 1000px brush size).

![CTC-6110WL: Stroke that looks like a bunch of blobs](./2024-08-09/stroke.png)

I tried using S-pen on my tablet and Wacom pen on my phone to confirm that this is not the pen issue (they are cross compatible!). Stroke on my phone is smooth and nice, while on my PC, it looks like a bunch of blobs, just like screencap above. I was wondering if this is an issue with my tablet only, or it affect all CTC-x110WL tablets, since the tablet buying guide spreadsheet also states that CTC-4110WL (a smaller variant of my tablet) have glitchy pressure.

The current mitigation for inconsistent pressure now is to use pressure smoothing, which adds a bit of latency. In Krita, you can use "Weighted" smoothing with "Smooth Pressure". For other applications, consider finding something related to pressure smoothing in the manual, or use OpenTabletDriver with pressure smoothing plugin.

**Update (10/08/2024)**: You can (partially) mitigate the inconsistent pressure problem by folloing the guide mentioned in this video: https://www.youtube.com/watch?v=415ngQOHiME. Also it's confirmed that the entire CTC-x110WL line of tablets have the same pressure issue, so I've removed "at least for me" part. I wish one day Wacom will release a firmware update to (at least partially) fix the issue (driver update is not enough; the tablet was designed to work on Android devices as well).

### USB-C port sometimes broke for a few minutes
This had happened to me multiple times before, but it usually related to high power device or something. Basically, there's a period where I can't connect using USB-C cable. Bluetooth still works; it's just the USB that doesn't works. I'm not sure why, it could be my tablet's issue again, or it could be something that also affect all tablets with the same model, because this issue also happened with another one at local Wacom store (the place where I bought this tablet).

### Nib eater
The surface, while feel nice to draw on, is actually a nib eater. I've replaced the nib 4 times since the day I bought this tablet, while my friend don't have to do that often, though I expect this is a small issue, since you need a nice surface to draw on, or it would be much harder to draw linearts (I tried drawing on my phone before; the surface is just too slippery so my linearts are shit).

## What else?
### I don't use "gifts"
It came with 3 months of whatever drawing softwares out there, but I decided to use Krita, because it's free and it feels like it was designed for professionals (I'm not professional though, unfortunately...). If only I can donate some bucks to Krita Development Fund...

### Toggling eraser (without eraser bind)
Assuming you are still using the same pen that came with the box and official Wacom driver. If you hold the 2nd button, then slowly lower the pen, the eraser mode will be toggled. Releasing the button and it will come back to normal mode. I use this multiple times before and it's great that I don't have to bind eraser for 2nd button; I bind panning mode to it instead.

### A version without battery and Bluetooth would be nice!
I plug my tablet to my laptop most of the time, so having a battery makes the tablet heavier, though I could have just bought other tablet for cheap instead.

## Conclusion
OK tablet that's sufficient for drawing simple stuffs, but when pressure stablity is important to you, you might want to find other tablet instead. OK for osu!, but would you pay $120 more for 240Hz, while top player is using 133Hz tablet and still gaming hard? It's just another consumer tablet after all. I can't recommend this tablet to you though, unless Wacom managed to fix the issue with pressure input through firmware update or something.