********************************************************
Lab 1, PID control of water tank named LM900
********************************************************

Time and place
==============================================
- Room Hammer at TBD

Equipment
==============================================
- LM900, the red model at Hammer with two water tanks, a manual valve between the tanks and some sensors.
- Beckhoff CX and IO`s
- Some device with a browser, connected to lab WiFi
- If you need to debug, or you`re just interested, take a look thru the IO list and System Control Diagram
  on `GitHub <https://github.com/MOJOliciousFTW/HVLlab/tree/master/LM900/>`_



Description
==============================================
In this lab you will tune a PID to control the water level in a tank. Software is done, you will do the tuning.

Your PID will be given a score, less is better.
Take a screen dump of your score and PID gains, send it to me, and receive a thumbs up for completing the lab.

The LM900 model can be a fun, practical challenge for three reasons
    #. The manual valve is an un-measured disturbance (but you can estimate it)
    #. The outflow of tank 1 is dependant of the square root of its water level (non-linear, can be compensated for)
    #. The pump should not run dry, and tank 1 should not overflow (interlocks are in place to prevent this)

The overall workflow for you to do is
    #. Turn on stuff
    #. Get to the user interface thru a browser
    #. Have fun
    #. Tune the PID manually (feel free to use the auto tuner, but do some additional tuning)
    #. Get a score
    #. Win

Steps
==============================================

#. Connect to the local lab WiFi with your device (PC, smartphone, tablet) and go to address_of_ui. If all is well,
    go to the next step, else:

    #. Check that the LM900 IO is connected to Beckhoff IO modules, see io_list

    #. Check that IO`s are connected to Beckhoff CX.

    #. Check power supply to LM900, IO, CX, router. Turn these on.

    #. Wait for green lights. Else, call for help.

#. The LIC01 (level indicator and control) CA is a NORSOK I-005 (IEC PAS 63131) template for control of analogue
    signals (PID). Select manual, internal mode, play around with the manual output.

    #. Open the manual valve completely
    #. Set your manual output to something that gives a steady water level (maybe 50%).
    #. What is the resulting level? What is the ratio between manual output and resulting water level?

#. Set your internal mode gains. This PID is in standard form, so I and D are in units of seconds. Maybe try Kp,Ti,Td as
    1,10,0.
#. Try your PID
    #. Set a desired level YR as 50%
    #. Switch to auto (still internal)
    #. Observe your PID.
        #. Move the YR around
        #. Move the manual valve around
    #. Adjust tuning until you get a smooth running pump, the level reaches it`s reference smoothly and the manual
        vale disturbance is handled ok.

#. Open the manual valve fully, run the test, get a score.
    #. Happy? Done. Else, keep tuning, ask questions, take the opportunity to understand control theory.

Reg tek rulez!