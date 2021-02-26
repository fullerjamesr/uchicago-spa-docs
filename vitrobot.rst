Grid preparation and freezing (Vitrobot)
========================================

What settings should I try?
---------------------------
There are relatively few variables under your control:

**Humidity and temperature of the chamber:** The chamber is humidified to prevent additional losses from the sample during the blotting process, especially after blotting when the sample is reduced to a thin film of miniscule volume. Most samples do not need to deviate from 100% humidity and at/slightly below room temp (18—22 °C). Regarding temperature: considering that the sample is in (thermal) contact with the tweezers which constantly come in and out of the chamber, and the short time your sample droplet usually spends in the chamber, the chamber air temperature may not have a huge impact on the temperature of your sample droplet. If your sample has a very strong solubility or stability difference between 4 and 22 °C, however, there is certainly no harm in trying to keep things cooler.

**Wait time:** How many seconds after pressing the button before the vitrobot will start blotting. In the general case this can be 0. Wait times are useful under two circumstances: (1) to make the timing of an on-grid reaction (e.g., adding a ligand to the sample droplet immediately before blotting) semi-repeatable; or (2) in cases of a continuous support surface, to give some time for the sample particles to interact with and adhere to the support surface before blotting. Recommend times for the latter are similar to negative stain incubation times, in the range of 15 – 30 seconds.

**Blot force:** A dimensionless value that determines how close together the vitrobot will attempt to bring the blotting pads. In general this can be left constant and should not need to screened extensively. Because the blotting mechanism is in part driven by a spring, over long times of extensive use, it may be necessary for this value to be increased (and tailored to each vitrobot) as the springs loosen. More viscous samples may require slight increases (+1, +2) past this point. Ask around, other users probably have values they use for each vitrobot that have been shown to work well.

.. tip::
   A good way to calibrate this is to run the vitrobot with blot papers but without tweezers loaded and observe how close the blotting papers approach. A good value of blot force will be the *lowest* positive value at which the bottom edge of the papers repeatably-but-just-barely touch in the absence of a grid. That way, when a grid is present, there should be good consistent contact across the grid surface.

**Blot time:** How long the blotting pads will be closed around your sample. This is the primary vitrobot parameter that is screened. However, screening can be fairly coarse – remember that the angled nature of the blot pads tends to generate a range of ice thickness across the grid. For holey surfaces and standard buffers (i.e., sub-CMC detergents and no additives that modify viscosity), good ice is usually observed between 3 and 6 seconds when blot force is set as described above. Often it is best to focus on perfecting the nature of the underlying sample (concentration, upstream purification steps, complex integrity, any ligands or buffer additives) at only one or two blot times (e.g., 3.5 and 5 seconds) before fine-tuning this parameter to maximize the number of squares of optimal ice thickness for final data collection.

**Drain time:** The delay between blotting pad retraction and plunging. Under most conditions, skipping this (set to 0 seconds) is the norm, as it prolongs the time that the sample exists as a thin liquid film with significant air-water interface(s). However, it can sometimes lead to an improvement in the resulting distribution of ice, as it allows more time for the thin film to equilibrate/relax after separating from the blotting papers. For example, gold surfaces are more difficult to fully hydrophilize by glow discharge, and as a result tend to give “puddles” of thicker ice in the middle of grid squares. Adding 1 second of drain time can help alleviate this.

The Vitrobot interface
----------------------
The Vitrobot user interface is divided across two pages. You can toggle between them using the **CONSOLE** and **OPTIONS** tabs at the bottom left. The control buttons along the right edge are always displayed.

Console tab
^^^^^^^^^^^

.. figure:: img/vitrobot_consoletab.*

   Vitrobot interface, console tab

.. topic:: Temperature

   Set the desired chamber temperature. The actual temperature is given in the big red digits.

.. topic:: Humidity

   Set the desired chamber humidity. The OFF/ON/MAN radio button needs to be set to ON or MAN for the humidifier to turn on. ON behaves like a thermostat: the humidifier is turned on only when the humidity deviates from the set point. MAN means the humidifier runs constantly regardless of the measured chamber humidity and setpoint.

.. topic:: Miscellaneous

   Poorly titled, this is a general purpose timer. You can set a time with the arrows and hit start, and it will count down for you. The thing that looks like a clock is just a visual representation of the fraction of the start time left - the arm will move counterclockwise around and back to north/12:00 as time decreases.

.. topic:: Memo

   The Vitrobot will write simple logging and error messages to this text box.

Options tab
^^^^^^^^^^^

.. figure:: img/vitrobot_optionstab.*

   Vitrobot interface, options tab
   
.. topic:: Processes

   The Vitrobot is capable of doing up to 20 cycles of sample application + blotting prior to plunging, each with different settings. By default there is only 1. You can use the buttons to add or delete additional cycles.

.. topic:: Process Parameters

   Set the desired blotting parameters, using the arrow buttons by each field.

.. topic:: Miscellaneous

   These checkboxes enable or disable other Vitrobot functions.

   *Use Footpedal* is self-explanatory.

   *Humidifier off During Process* will force the humidifier off during sample application and the blotting sequence. Recommended!

   *Skip Grid Transfer*: By default, the Vitrobot cycle includes a (extra) step at the end after lowering the grid and freezing reservoir, where it will lower the ethane chamber slightly further to bring the tweezers and grid out of the ethane. This is safe *if* you act fast and are using the optional insulating foam ring to create a large LN2 vapor layer. However, we recommend that you manage transfer out of the ethane manually, and if so you can check this to skip an unnecessary button press. Recommended!

   *Autoraise Ethanelift* will combine the steps of raising the fresh tweezers + grid into the chamber and raising the freezing reservoir up to the chamber, thus saving you a button press. Most users get accustomed to the sequential prompts of attaching tweezers, pressing a button that retracts the tweezers, then mounting the ethane and pressing a button again, in which case this option is not enabled.

----

The following sections of this page are ordered top-to-bottom in the recommended sequence that will make the best use of your time. The exception is the section about ethane tank valve usage, which is consolidated at the bottom.

Setting up the Vitrobot
-----------------------
Getting the Vitrobot set up first ensures that (1) your blot papers will have time to equilibrate in the humidified chamber, and (2) you get right to using your ethane when it’s as fresh as possible.

1. Turn the Vitrobot on. The switch is around the back on the right side, near the base of the machine.
2. Attach and fill the humidifier:

   .. caution::
      Make sure the red rubber O-ring is properly (evenly) seated around the humidifier’s opening.

   a. Attach the humidifier to the blotting chamber. The triangular sticker should face towards you. To maneuver the humidifier, its power cord will feed in and out of a hole in the base of the Vitrobot.
   
   .. caution::
      Guide the cord gently, it is possible to break the enclosed wires or their connection with the plug.
   
   b. Place a paper towel below the humidifier to catch leakage that occurs during filling.
   c. Using a 60 mL syringe, inject approximately 60 mL of distilled water via the tubing inlet at the bottom of the humidifier. Water is prevented from flowing back down this tube by a check valve. To generate a nice seal and prevent leaks, pull back gently on the syringe plunger after filling. There is no need to overfill it, but once water starts flowing into the blotting chamber, it’s definitely full.
   d. Wipe up any overfill water from inside the blotting chamber and any water that leaked out onto the Vitrobot base during filling. Standing water in these locations can cause inconveniences later, especially if it freezes.

3. Attach blotting papers:

   a. Use tweezers (to avoid contamination from hands/gloves as much as possible) to remove two blot papers from the stack provided.
   b. Attach one blotting paper to each of the blotting paddles. The blot papers are held in place by the white plastic clip rings, which insert into the blotting paddles.
   
      .. tip::
         Because the blot papers are made by being punched out of a larger sheet, there can be a slight curl in the outer and inner edges of the papers. This is often more evident on the inner edge, but can also affect the outer edge that will be interacting with your grid. Should this curl face towards  or away from the sample? Opinions vary. **It's probably most important to be consistent.** The Vitrobot manual would have you believe you should point the curl towards the pads/away from sample.
         
      .. tip::
         It is not necessary to use more than a single blot paper each, unless you are trying to exactly mimic blotting conditions given to you from some other source.

   c. (Strongly recommended, but not required) Run through the **Reset BlotPapers** function by pressing that button on the vitrobot interface. The act of attaching the blot papers tends to jostle the blotting paddles out of position slightly, which often causes the first grid you freeze to be significantly different than the rest. The paddles can be reset by running a blank blotting cycle, which is triggered by the *Reset BlotPapers* button.

4. Using the Vitrobot interface, under the Console tab, set your desired humidity and temperature. Most samples do not need to deviate from 100% humidity + at/slightly below room temp (18—22 °C). Make sure the chamber door is closed, and check to see that the humidity in the chamber begins to rise after a few seconds. If minutes pass without the humidity in the chamber moving towards your set point, first check and reseat the seal/O-ring between the humidifier and the chamber (careful, it’s full of water now!); if the problem persists, add a few more mL of distilled water to the humidifier.

Glow discharge your grids
-------------------------
The carbon or gold foil surface of TEM grids are hydrophobic, which prevents aqueous samples from properly dispersing across and into the holey surface. To create a hydrophilic surface, glow discharge generates plasma in the space directly above the grid, which spews ions down onto the grid surface that render it hydrophilic.

The UChicago EM core facility has a Gatan Solarus for glow discharging/plasma cleaning grids.

.. image:: img/solarus.*

1. Place your grids, **foil/sample side up**, on a soft/compressible surface that will let you pick the grids back up again easily. This is often a rubber mat in a petri dish, or a small glass slide wrapped in parafilm, as these surfaces are also slightly sticky, which helps keep the grids in place during transport and vacuum changes.
2. Open the chamber on the top of the Gatan Solarus glow discharge unit.

.. note::
   Our machine tends to accumulate a slight vacuum in the chamber when not in use.
   
   If the chamber won’t open, click the *Vacuum* button as if to initiate pulling a vacuum in the chamber, then immediately click *Abort*, which should trigger a full venting process that, when finished, should allow you to easily open the chamber.

3. Place your grids and carrier surface on the bottom of the round chamber.
4. Close the chamber lid.
5. Adjust the glow discharge time as desired. The longer the time, the more hydrophilic the resulting surface, but prolonged exposure to the plasma will thin (weaken) and possibly damage the foil surface.

.. tip::
   Gold foil surfaces often require longer treatment than carbon to achieve similar liquid spreading properties.
   
   James recommends 45 seconds for carbon surfaces and 1:15 for gold surfaces.

6. Press *Start*, which should go through all the steps of pulling a moderate vacuum in the chamber and creating plasma for the specified time.
7. When the interface indicates the cycle is done, press *Vent* to vent the remaining vacuum in the chamber so you can open it and remove your grids.

.. tip::
   Take a look at your grids. Are they where you left them?
   
   The vacuum venting can occasionally generate enough air movement to flip grids over.

8. Close the chamber lid before walking away!

Prepare the freezing chamber with liquid nitrogen and ethane
------------------------------------------------------------
.. admonition::
   Recall that (at normal atmospheric pressures)

   * Liquid nitrogen exists at about -196 °C
   * Ethane is a waxy solid at liquid nitrogen temperatures, melts at -182.8 °C, and boils at -89 °C

1. Fully assemble the freezing chamber: brass cup for liquid ethane, spider, and grid box platform (and the foam frost shield, if you choose to use it). Get your grid boxes in place in the platform slots.
2. Submerge the freezing chamber in LN2, both in the outer chamber and the brass cup. At this stage you can aggressively fill everything.
3. Keep adding LN2 as needed until the initial Leidenfrost bubbling has calmed, keeping the level in the outer chamber above your grid boxes so they don’t frost up and keeping at least enough in the brass cup to keep the bottom submerged. Then, cover the whole thing with an ice bucket to reduce frost.
4. While the freezing chamber is cooling, prepare the ethane tank for dispensing (see below)
5. Immediately as the last of the LN2 slowly evaporates from the brass cup, begin dispensing ethane gas into the cup. At this point, the brass cup should be at - or just barely above - LN2 temperature, perfect for liquifying ethane gas on contact.

   a. Hold the tip of the ethane gas hose against the corner of the brass cup
   b. Slowly open the Regular Output Valve to begin a gentle flow of gas
   c. While the gas is flowing, slowly move the tip of the hose around the bottom of the brass cup. This ensures that the work to cool the ethane is distributed across the full area of the cold brass.
   d. As liquid accumulates, the sound of the ethane dispensing will change from gaseous hissing to liquid bubbling. You may not be able to see it clearly through a cloud of frosty vapor. At this point, you can begin to use the sides of the brass cup to cool the incoming ethane instead of the bottom. This will also reduce bubbling in the new liquid ethane that can spray it out into the outer nitrogen reservoir.
   e. Fill the brass cup nearly to the top with ethane. You may need to stop and lift the spider up briefly to check the level
   f. Once finished, close the Regulator Output Valve. You can leave the rest of the ethane regulator as-is while you’re freezing, in case you need to stop and refill with more ethane in the middle of your session.

Grid freezing
-------------
The workflow loop for freezing a grid goes something like this:

.. caution::
   The main thing that can go wrong with the Vitrobot during freezing is that the tweezers are not attached properly, or the trapdoor over the aperture in the bottom of the chamber fails to open. In either case, this will ram the tweezers into a solid surface when they try to plunge and ruin them.
   
   Do you hear funny noises coming from the mechanism operating the trapdoor? STOP and go find a facility staff.
   
   Is there condensation or other water/buffer around the trapdoor? It can freeze when the freezing reservoir is raised and ice the trapdoor shut. Wipe it totally dry with paper towels or kimwipes.
 
#. Grasp a fresh grid with the tweezers. The grid should be centered relative to the long axis of the tweezers. The tweezers should touch as little of the grid as possible, but enough so that the grid will not shift or fall out during the process. This usually means the tip of the tweezers will impinge a bit into the mesh area of the grid, but only slightly.

   .. tip::
      **Remember which side of your grid is the foil side!** The clamp on the end of the tweezers that connects them to the vitrobot rod makes this easy: one side has a visible screw head and red threadlocker painted around it, the other is solid metal. Make it a habit to always grab your grids with one of those sides facing up.
      
      .. figure:: img/vitrobot_tweezers_sides.png
      
         The easily distinguished faces of the vitrobot tweezers

#. Lock the tweezers with the black sliding clamp.

   .. caution::
      Do not overtighten. The bottom of the clamp need only come down as far as the first ridge of the tweezer grip.

      .. figure:: img/vitrobot_tweezers_clamped.png
      
         This is clamped enough!

#. If you just started the vitrobot, you will have to click *Place new grid* on the Vitrobot interface to lower the rod out of the chamber. If the rod is already accessible, you either can do it now or after attaching the tweezers.
#. Attach the tweezers to the Vitrobot plunge rod. The tweezers should be centered (front to back) on the rod. Attach the tweezers such that the foil side of the grid faces the direction from which you will apply the sample in the blotting chamber (usually driven by your handedness).

   .. caution::
      Failure to center the tweezers on the rod could result in them missing the trapdoor aperture during plunge and instead ram into the chamber floor causing irreparable damage. Vitrobot tweezers are not cheap!

#. Click *Place new grid* and/or *Continue* to retract the grid, tweezers, and rod into the blotting chamber
#. Remove the spider from the freezing reservoir and store it under LN2. Place the freezing reservoir on the Vitrobot platform. Click *Place ethane chamber* in the Vitrobot interface to raise it flush under the door to the blotting chamber.

   .. caution::
      The spider won't fit when the freezing reservoir is raised. Don't forget to remove it!

#. If you want to change any of the blotting settings from where they already are, now is your last chance. After clicking *Start process*, changes to settings are ignored for this grid.
#. Click *Start process* in the Vitrobot interface to lower the grid slightly. It now lines up with the entrance doors/apertures on either side of the blotting chamber. Open the little sliding door on the appropriate side, and pipette 2.5 to 3.5 uL of your sample onto the foil side of the grid.
#. Immediately click *Continue* on the Vitrobot user interface to being the automated blotting and plunging procedure you have set out in the Vitrobot interface (options tab). The Vitrobot will bring the grid back up in line with the blot papers, pause for *Wait time* seconds, bring the blotting paddles together for *Blot time* seconds, retract the blotting paddles, wait *Drain time* seconds, then plunge the grid through the small trapdoor aperture into the liquid ethane in the freezing reservoir below. The reservoir and the rod/tweezers will then lower in synchrony.
#. Being careful to not collide the grid with the brass cup sides or pull it out of the ethane, detach the tweezers from the plunge rod.
#. Bracing the freed tweezers against the side of the brass cup, and continuing to keep the grid away from the sides and under the ethane, remove the tweezers + freezing reservoir from the Vitrobot to the countertop.
#. Move the grid to the grid box, being careful to not collide the grid with any surfaces along the way.
   
   .. tip::
      Although moving quickly here is advantageous, it is more important to keep the grid from colliding with anything and keep as close to the cold ethane/nitrogen (within the vapor layer) as possible. Unnecessary focus on speed can lead to mistakes!

   .. tip::
      Excess ethane tends to get wicked up between the tweezer arms, then run down and form a solid white frozen layer over your grid when moved to LN2 temperatures. To avoid this, bring the grid up slowly until the tweezer tips (and thus probably about a quarter to half of the grid) are well out of the ethane. Shake gently to encourage excess ethane to drain back into the reservoir. Then keep moving relatively slowly while you totally remove the (rest of the) grid from the ethane so that any ethane meniscus detaches gracefully. Only start moving fast after you're totally out of the ethane.
      
      Finally, know that small bits of ethane residue are fine. They will either detach when manipulating the grid to get it into the microscope or sublimate away in the vacuum of the microscope. Don’t stress too much about it, don't toss your grid out.

   a. If you are using the foam ring insert, you can move the grid directly from just-above the ethane to its destination grid box slot, because the foam insert insulates a generous vapor layer. In this case, you would need to move the black sliding tweezers clamp back up to the top of the tweezers right away while the grid is under the ethane.
   b. If not using the foam insert, it is best to first move the grid to under the outer liquid nitrogen, undo the black sliding tweezer clamp, then move the grid to its destination grid box slot.
#. Grab the spider out of LN2 and place it back into the ethane cup to keep it cool, and cover the whole freezing reservoir again (e.g., with an ice bucket) to minimize frost buildup.
#. Wipe the Vitrobot tweezers thoroughly with a kimwipe, to remove the condensation that will form as they quickly return to room temperature.
#. Repeat this process for each desired grid.

When you're done
----------------
Please put everything away when you're done. **Do not skip this part.**

#. Store your grid boxes for long term storage. Probably in a big dewar in your lab or the core facility.
#. Remove and store the vitrobot tweezers. Please be nice to the Vitrobot tweezers. Cap them! A pipette tip works fine if the the original cap has been lost.
#. Turn the Vitrobot off using the *Exit* button in the Vitrobot interface. Wait, then after the screen turns fully off and the trapdoor closes, turn the Vitrobot off using the switch in the back.
#. The freezing reservoir can be placed in the fume hood to burn off.
#. Disconnect the humidifier (only after the Vitrobot is shut down!) carefully and tip the remaining water into a vessel you can bring to the sink to dump out. There's quite a bit of water in the interior liner in the humidifier that bleeds into the middle reservoir via a hole about halfway up the side, so you'll have to shake and rotate it quite a bit to get it all out.
   
   .. caution::
      Please take the time to do this completely, otherwise the leftover warm water starts growing various micro-organisms. Which will then get spewed into the chamber alongside the water vapor the next time someone uses the humidifier.

#. Remove and dispose of your blotting papers, and leave the ring clips in the chamber.
#. Excess LN2 in any containers/dewars can be dumped into the dewar for the Talos cold trap. Facility handheld dewars should then be air dried (where you found it).
#. Purge the ethane tank regulator when you're done, unless someone else is still freezing on the other Vitrobot.
#. Sign the log!

Ethane
------
The regulator on an ethane tank will have 3 valves/knobs and 2 gauges, as shown below. This regulator is used to step down from the pressure in the tank to the point where you can dispense it by hand.

.. image:: img/regulator.*

In both cases, the idea is to either close or open the valves starting at the tank and moving outwards.

.. caution::
   You won't be dealing with enough ethane to be flammable (assuming you don't just throw all the valves open and walk away). But, liquid ethane is much more capable of causing burns than liquid nitrogen (Leidenfrost won't save you). Be wary of splashes!

Preparing for dispense
^^^^^^^^^^^^^^^^^^^^^^

#. Check the status of the valves and gauges. There should be no pressure on either gauge and all the valves should be closed. A previous user may have forgotten to close valve(s), or forgotten to purge the regulator. On the other hand, if someone else is freezing at the same time, everything may already be set for you to dispense, and you can just start dispensing.
   
   If no other users are present and the regulator has been left registering pressure on one or both gauges, then a previous user has messed up. In this case, **Purge the regulator before continuing** to the next step. You don't want that ethane that's been sitting in the regulator valves, anyway.
#. Open the *cylinder valve (1)*. You will see pressure registering at the gauge closer to the tank. For our purposes, this valve is essentially “all or nothing,” so there is no need to open further once pressure registers. It’s usually in the range of hundreds of PSI, depending on how full the tank is.
#. Gently turn the *regulator hand knob (2)* in the labeled “Increase” direction until pressure registers on the distal second gauge. For the purpose of gently dispensing into the Vitrobot brass cup, anything between 15-50 PSI will suffice. More than about 50 PSI and you’ll just spray ethane all over the place.
#. Ethane can now be dispensed using the *regulator outlet valve (3)*.

Purging when you're done
^^^^^^^^^^^^^^^^^^^^^^^^

#. Close the *cylinder valve (1)*.
#. Carefully open the *regulator outlet valve (3)* and direct the gas output away from you to clear the regulator of remaining pressurized ethane.
#. Close the *regulator hand knob (2)* (turn in the labeled “Decrease” direction). The *regulator hand knob (2)* is “closed” when you feel it become loose as you turn it in the “Decrease” direction.
#. Close the *regulator outlet valve (3)*.
