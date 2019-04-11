---
title: Augmentus - WH40K Augmented Reality Tool
navtext: Augmentus
description: A tool designed to assist in active tabletop games, saving you time and keeping you focused on gameplay.
hero: "/assets/images/tau-water-caste-envoy.jpg"
heroalt: "Tau Empire water caste members"
---

# Augmentus

*A tool designed to assist in active tabletop games, saving you time and keeping you focused on gameplay.*

## Purpose

The purpose of this application is to enhance our tabletop playing experience, never to replace the parts that are most enjoyable to us all. 

There was an augmented reality (AR) project floating around that was trying to replace tabletop models with virtual ones on the tabletop.

**This is not that.**

Tabletop gaming is about more than just the game - the lore, the art, the craftsmanship and so much more all play into the immersion and enjoyment of this hobby. The bane of the tabletop is the time spent checking distances, trying to figure out rule interactions, and (mis)calculating wounds and armor saves.

## Project overview

There are two main phases planned for this application. The first will focus on the tracking of unit positions on the board, the second will manage unit interactions.  

### Phase 1: Position tracking and measuring

This phase's goal is to be able to recognize and track the positions of all units on the board at once. 

Once the positions are tracked, your device can then display an overlay on the battlefield in true augmented reality fashion to show movement and shooting ranges (or a combination of both) for any unit on the field at any time. 

We have been researching the use of Image recognition, RFID, QR codes, and BlueTooth technologies for this task.

**Image recognition**

Training each individual unit type to be recognizable would be tiresome, and it appears that the devices we use everyday would have a difficult time distinguishing between individual models. Unless someone has any brilliant ideas, image recognition probably will not be sufficient for this application in the near future. 

**QR codes**

QR codes (the little black-and-white square barcodes) are unsightly, have to be visible to your device camera, and have limited range for the sizes we are considering. We did consider a QR-type code system that would fit around the vertical edge of a model base - that had an effective range of about 12" in optimal conditions. We simple could not find a way to make these practical. 

**RFID**

The equipment needed seems impractical for this application. Still doing some research into existing technologies here. 

**BlueTooth Low Energy**

BlueTooth Low Energy (BLE) beacons have a battery lifespan ranging from a few years to nearly a decade. However, the starting price appears to be around $10/each and goes up quickly. 

We are currently running with the BLE option, and attempting to source much cheaper beacons ($1/$2 each). These beacons need only operate for 2-3 meters and broadcast a simple identifier. Those would then be picked up by receivers at the corners of the battlefield, which allows for easy positioning. 

Even at $10/each, there are certain times where this could still be viable (such as at tournaments) but it does not allow this tool to be a mainstream solution. 

## Phase II - Interaction

*What was the strength on that weapon again? What's the toughness on the target unit? My AP? Your armor save? Did you have an invuln? Wait, didn't that guy have a feel-no-pain? Arg, I forgot my mortal wounds.*

No more frustrating rule lawyering and book turning (and FAQ printouts) to confirm wording of a rule. Pick your unit, pick an enemy unit, and pick an interaction (shoot, charge, etc.) to instantly see all of the necessary roles and rules. Not a calculator, mind you - you still need to roll your dice. We do **not** want to take away the tactile feel of the game. 

You will, however, know instantly what you need to roll to hit, wound, the enemy's armor/invuln/FNP saves, and any special abilities associated with those two units interacting. How many more games can you get in if you spend all of your time on strategy, moves, and rolls instead of calculations and page flipping?

Augmentus is not a game system itself - it is simply a battlefield management tool. It does not replace the tabletop experience, it **enhances it** - say it again - *it does not replace the tabletop experience, it enhances it*. That is the key to a successful tabletop technology and we firmly believe the future of the hobby.

For legal purposes, this will simply be the *generic rules engine* for tabletop games, and you will still need to manually enter your lists and the actual rules sort of like you have to do with another popular application that narrowly skirts IP issues (\*cough\* Battlescribe \*cough\*). That is, unless someone with a big company that owns the IP wants to get in on this project and gain a major edge in the market. 

Straight looking at you, Games Workshop. We would love to talk with you! 

(Like everything else on this site, Games Workshop does not officially endorse and is in no way associated with the Ar'sho Enclave or the Augmentus project.)

## Current status: research

We are researching different location-tracking solutions and actively searching for pricing/asking for bids on BLE beacons that might meet our needs and target price point, which we are trying to keep under $100 per army. That price will fluctuate depending on the size of your army. 

We are also open to being contacted by [Games Workshop](https://www.games-workshop.com/){: target="blank"} (are you listening, Geedubs?) if they want to make this an official product. 

If you'd like to keep up with our progress, follow our [Facebook](https://www.facebook.com/ArshoEnclave/){: target="_blank"} or [Twitter](https://twitter.com/ArshoEnclave){: target="_blank"} pages or even hop on our [Patreon](https://www.patreon.com/arshoenclave){: target="_blank"} where we publicly post updates. 

**If you want to be involved** we *probably* won't turn down help. Contact us through any of our channels or [email us](mailto:arshoenclaves@gmail.com) directly.
