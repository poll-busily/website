+++
title = "Minolta X500/X700 Capacitor Repair"
date = 2017-11-01

[taxonomies]
tags = ["photography", "repair"]
+++

Here are some instructions for replacing the primary electrolytic capacitor found in several Minolta film SLR bodies.

<!-- more -->
Over time, electrolytic capacitors are prone to failure and these Minolta bodies start to show strange behaviour like not actuating the shutter all the time. 

If you’re handy with a soldering iron then it’s actually relatively simple to replace the old cap with a new one and revive a capable camera that would otherwise end up in landfill. I came across a few examples of this operation in the far corners of the internet but those had small, low-quality photos and I wanted to provide something that’s hopefully more detailed and easier to follow. 

This guide applies primarily to the X-500 (or X-570 as it was marketed in the USA) but should also apply to the X-300/X-370 models as well. All photos shown here are of the X-500/X-570 model. 

The X-700 has, as I understand it, an additional capacitor at the top of the camera and the replacement of that isn’t covered here. Replacing just the bottom capacitor is sometimes enough to get the camera working again and sometimes not. 

{{ img(path="./image.jpg", alt="") }}

## Background

These types of capacitor contain a liquid electrolyte and, with the passage of time, this can leak or dry out, leaving the capacitor with a reduced charge capacity. As the capacitor weakens, sudden loads (such as the shutter firing) are increasingly drawn directly from the battery. This causes the voltage to drop or “sag” momentarily before returning to its previous level. Once the voltage sag becomes too high the camera will shut down during shutter firing, as the voltage is no longer sufficient to drive the other camera circuitry. Replacing the capacitor restores the buffer of charge required to drive the shutter and, in many cases, that’s all that’s required to get the camera working again. 

The camera used in this guide was received in a working state but as the original capacitor was still in place I opted to replace it preemptively. Photos shown in the gallery below are with the new capacitor in place. 

To determine if the capacitor is original, take a look at the voltage listed on the capacitor can. You may need to gently lift the capacitor up and out of the camera body by half a centimetre or so in order to see all of the text. If the voltage rating is 4V then it is likely to be original, as caps with this voltage are less widely available nowadays. Other possible signs to look for are differences in the solder joint (colour, shininess, quality) relative to other nearby joints, and whether the capacitor appears to be a tight fit in the space where it lives, again indicating that it might not be the originally-specified part.

## Required Tools

An extensive toolkit isn’t needed for this job. As long as you have a half-decent soldering iron and the skills to wield it then you’ll just need a standard screwdriver to access the circuitry beneath the base plate. 

- A small JIS (or Philips-head) screwdriver
- A soldering iron suitable for PCB work
- Solder
- Solder wick (optional, for cleanup)
- Small, long-nosed pliers or tweezers (optional, helps removal)

## Capacitor Choices

The original capacitor from the X-500 and X-300 will be either a 200uF or 220uF, 4 volt, electrolytic cap and most likely of the reputable Nichicon brand. Suitable replacements are easy to get, although capacitors with a 6.3V rating are likely to be much more widely available – you can freely go to a higher voltage rating but be aware that the physical size of the cap often increases as you do so. 

**Note:** Apparently, the X-500/X-300 service manual calls for a 150uF, 3.15v cap so if you have trouble finding a 200uF or 220uF that will fit, you may well be able to use a smaller 150uF instead. Thanks to Roland for leaving a comment on a previous version of this article with the info. 
My Original Choice

I used a [Nichicon USR0J221MDD 6.3V, 220uF](https://uk.rs-online.com/web/p/aluminium-capacitors/4758719) cap, available at RS Electronics with part number 475-8719. I like RS because they don’t have a minimum order quantity, which makes small, one-off orders like this more reasonable, but this is not an affiliate link :-). 

The capacitor I chose is from the SR series and is 6.3mm in diameter and 7mm in length. This provides a good fit with plenty of room to spare. Other caps with the same rating will work. You could get away with a longer cap but I wouldn’t use one with a diameter much above 7mm as it might be a tight fit near the base. 

### Newer Options (2024-)

As of 2024, the above cap that I used has gone end of life. Here are some alternatives to consider. These should meet all the same specs but I haven't tested them myself.

- [Panasonic ECE-A0JKA221](https://mou.sr/3Towbej)
- [RS PRO 220μF](https://uk.rs-online.com/web/p/aluminium-capacitors/7060589)

## Process
**The usual disclaimer before you go ahead: it’s always possible that you could damage the camera (or yourself!) by attempting the repair. If you’re not comfortable with a soldering iron and basic electronics then you should consider sending the camera off to a repair shop instead (maybe point them to this article!).**

First, make sure that any film and batteries have been removed from the camera. I like to be certain that I’m not going to cause any issues if I accidentally short out any contacts with the soldering iron or solder wick.

1. Remove the four screws holding the base plate to the internal frame. Note that there are two shorter screws and two longer screws – keep these together and take note of their location. Lift the plate up and away as there’s nothing attached to it underneath.

2. Now we can see the capacitor nestled away at the right hand edge (with the camera upside-down and the mount facing away from you). The two solder joints at the base of its legs are where we will need to heat to remove it. Unlike on a rigid, through-hole PCB the component legs don’t protrude down through the circuit board – they’re just soldered to pads on top – and this simplifies the process since nothing needs to be moved or removed for access to the reverse side.

3. Heat each leg in turn, lifting it gently up and away from the pad with a pair of tweezers as you do so. An alternative, if that’s not working so well, is to hold the capacitor can with the tweezers instead and to rotate the whole body. The PCB is semi-flexible so it might also lift a little bit during the process and that’s okay.

4. Optionally, use some solder wick (braid) and a dab of flux to quickly remove any old solder from the pads and then add a little fresh solder to each pad.

5. Trim the legs of your replacement capacitor to an appropriate length. This is easier if you removed the old capacitor without snipping its legs as you have a reference but you can always use a little trial and error, coupled with a Mk.I Eyeball, to find the right length as well.

6. Orient the replacement capacitor correctly with the negative side facing the camera body and the positive side facing the battery chamber. In the previous step we made both legs the same length (required for the cap to fit properly) but that removed one of the ways by which we can identify the proper orientation. The gallery images here show the correct orientation of the capacitor with the negative side (indicated by the stripe on the can) facing outwards and the positive side facing towards the inside of the camera.

7. Hold the replacement capacitor in place using tweezers and solder the first leg using the solder that is already on the pad, plus a small amount of solder loaded on the iron tip, to avoid the need to feed in additional solder from a spool. We only need small amounts here. Repeat for the second leg, for which the cap should sit in place on its own.

That’s all there is to it. Once the camera is reassembled with batteries installed, take a few test shots without film to see whether the proper shutter operation has been restored. 

## Tips

- Try to keep the soldering iron temperature relatively low if your iron is adjustable; this reduces the risk of melting or scorching the flexible PCB. I used a temperature of approximately 380C, a small tip, and leaded solder for this job.

- Double check your capacitor orientation before soldering as installing the electrolytic cap with the leads back-to-front will damage it.