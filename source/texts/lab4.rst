********************************************************
Lab 4, Pole placement control of helicopter model
********************************************************

Time and place
==============================================
- HVL Robotics lab at TBD

.. warning::
    - Don't put your fingers in the propellers. Don't!
    - Make sure the helicopter has room to move around

Equipment
==============================================
- Helicopter model from Quanser with two propellers in "helicopter" configuration (not "duo copter")
- Lab PC, specific for the helicopter. This has Matlab, Simulink, all necessary licenses and other software.



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
    #. Calculate PP gains
    #. Get a score
    #. Win

Steps
==============================================

 #. Turn on the helicopter first, then the lab PC. Don't ask why.. I don't know why.
 #. Open Matlab, run some_init_script.m. If all is well, go to the next step, else:

    #. Check that the helicopter is connected to the lab pc via usb.
    #. Check power supply for helicopter, lab pc and screen.
    #. Check screen, keyboard and mouse connections.
    #. Wait for green lights. Else, call for help.

 #. Open some_simulink_mdl.slx

    #. Play around with the pitch and yaw power sliders

 #. Open some some_simulink_mdl_with_pid.slx

    #. Play around with pitch and yaw reference sliders

 #. Calculate PP gains with help from HALP!

 #. Open some some_simulink_mdl_with_pp.slx

    #. Play around with pitch and yaw reference sliders

 #. Try your PID and PP controller, get a score

    #. Open some_prepared_simulink_test.slx
    #. Use the selector to select PID or PP
    #. Check your gains
    #. Run model, take note of the score and gains.
    #. Happy? Done. Else, keep tuning, ask questions, take the opportunity to understand control theory.

Reg tek rulez!