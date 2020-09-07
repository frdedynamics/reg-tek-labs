********************************************************
Lab 4, Pole placement control of helicopter model
********************************************************

Time and place
==============================================
- HVL Robotics Lab, Øyrane_ 12, 6800 Førde, 2. floor (under Reodorklubben).
- Time: TBD.

.. warning::
    - Don't put your fingers in the propellers. Don't!
    - Make sure the helicopter has room to move around

Equipment
==============================================
- Helicopter model from Quanser with two propellers in "helicopter" configuration (not "duo copter")
- Lab PC, specific for the helicopter. This has Matlab, Simulink, all necessary licenses and other software.
- The folder "Lab 4 RegTek" on the lab pc desktop.



Description
==============================================
In this lab you will do PID and Pole Placement (PP) control on a helicopter model. Let`s decouple!

Your controller will be given a score, less is better.
Take a screen dump of your score and controller gains (PID or PP), send it to me, and receive a thumbs up for
completing the lab.


The helicopter model can be a fun, practical challenge for three reasons

    #. Yaw and pitch are coupled
    #. The trigonometric functions in the system model shows its non-linearity
    #. It's like a helicopter, but it doesn't fly away


The overall workflow for you to do is

    #. Turn on stuff
    #. Open Matlab, run a init script, then a Simulink model. Get familiar.
    #. Tune the PID manually
    #. Tune some PP gains/poles
    #. Get a score
    #. Win

Steps
==============================================

 #. Open the desktop folder Lab 4 Reg Tek.
 #. Open Oppgave_1_pid.m (Matlab R2015b should open)

    #. Run it

 #. Open Oppgave_1_pid_simulink.slx

    #. Hit the Build button, blue dotted top right in simulink
    #. Wait for build to finish
    #. Find the Connect button, close to the play button, click it.
    #. Press play
    #. Helicopter should do some motions for 55 seconds and you get a score
    #. Click Connect button again to disconnect if not already disconnected

 #. Change your gains in the .m file and repeat the steps above (run, build, connect, play) until you`re happy

If all is well, repeat for Oppgave_2_polplassering.m and Oppgave_2_polplassering_simulink.slx, else:

    #. Disconnect power to the helicopter
    #. Restart PC
    #. Reconnect power to the helicopter

P.S: There`s no user restrictions on the lab pc so it`s surely possible to f*** things up for everyone.
Please don`t use the lab pc for anything else than lab 4 and specifically - only change your gains/poles in the
assigned .m files.

Reg tek rulez!

.. _Øyrane: https://www.google.com/maps/place/HVL+Robotics+Lab/@61.4590375,5.8326453,17z/data=!3m1!4b1!4m5!3m4!1s0x4616333d5f3d88b5:0x2025abbba16257dd!8m2!3d61.459035!4d5.8348393
