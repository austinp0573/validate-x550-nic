# Validating an Intel X550 NIC (Dell Part # C4D5P)

## Overview

I have in the past had issues when purchasing Network Interface Cards (I will, going forward, refer to a Network Interface Card as a NIC). At time I have received goods that were of dubious origin, some of these have performed well enough, and some have not.

If you intend to use a NIC on a system that requires uptime, it's a good idea to briefly investigate it and at least ensure that it's a genuine part that passes some basic tests.

## Initial Inspection

Determining a counterfeit PCB by visual inspection can be very easy, or almost impossible, a thorough treatise on that topic is beyond the pervue of this repo, but briefly:

1. **Look for Intel markings & stickers**

   * On the **green PCB** itself, you should see a **printed white Intel logo** as part of the board silkscreen, not just on a sticker.
   * Look for a **hologram/Yottamark/BradyID style sticker** near the bracket or on the heatsink/PCB. Genuine retail/OEM cards often have one; missing or obviously fake holograms can be a red flag. (my card, an OEM Dell model, did not come with a holograpic sticker, investigating the matter, I found that the OEM cards often do not, an actual Intel card definitely would)
   * Check for a **printed part number** like `X550-T2`, `X550T2BLK`, or an OEM FRU (Dell/Lenovo/HP part codes) on the main label.

2. **Check build quality**
   
   * This is, in my limited experience, the most obvious sign of trouble, prior to installing the card. 
   * Solder joints should look clean and uniform; no obviously hand-soldered wires, bodge wires, or random stickers covering chips.
   * The heatsink should be firmly mounted with proper screws, not glued or wobbly.
   * The RJ45 ports should be firmly aligned with the bracket and not crooked.

3. Optional but helpful: **take a clear photo** of the front of the card (label & heatsink side). If anything looks off, you can describe it or compare to product photos from Intel/major resellers later.

### Sources

[How to distinguish 10-Gigabit network card Intel X520-DA2](https://hwp24.com/articles/how_to_distinguish_10_gigabit_network_card_intel_x520_da2_from_chinese_fakes/)

---

## Hardware Installation

For this I will be placing the NIC in an HP EliteDesk 800 G2 SFF PC.

The process is very straightforward:
- Remove the side of the case.
- Remove the PCIe slot retention arm.
- Remove the PCIe slot place holder.
- Insert the card.
- Return the retention arm to it's original position.
- Close the case.
TODO: Add photo
## Hardware Identification
## Firmware & Driver Verification
## EEPROM Integrity Check
## Link & Diagnostic Testing
## Loopback & Throughput Testing (iperf3)
## Thermal Considerations