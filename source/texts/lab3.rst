********************************************************
Lab 3, PID control, with feed forward, of pendulum
********************************************************

Time and place
==============================================
- Room Hammer at TBD

Equipment
==============================================
- Matlab and Simulink
- Handout model in .slx file



Description
==============================================
In this lab you will tune a PID to control the position of a simulated pendulum. Software is done, you will do the
tuning.



The pendulum model can be a fun challenge for three reasons

    #. It`s non-linear, the torque from gravity is dependant on the pendulum position.
    #. It`s in every single control theory book - it is fundamental in understanding reg tek concepts.


The overall workflow for you to do is

    #. Open the Simulink model (.slx)
    #. Run it
    #. Have fun
    #. Tune the PID manually
    #. Write a feed forward term to compensate for gravity
    #. Analyse work done by FF and PID
    #. Learn

Steps
==============================================

WIP!

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
       valve disturbance is handled ok.

 #. Open the manual valve fully, run the test, get a score.

     #. Happy? Done. Else, keep tuning, ask questions, take the opportunity to understand control theory.

Reg tek rulez!