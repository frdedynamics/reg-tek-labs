********************************************************
Lab 2, PID control of motor and auto tuning
********************************************************

Time and place
==============================================
- HVL Robotics Lab, Øyrane_ 12, 6800 Førde, 2. floor (under Reodorklubben).
- Fridays 12-14.

Equipment
==============================================
- Motor, the red model at Hammer with a motor and variable load.
- Beckhoff CX and IO`s
- Some device with a browser, connected to lab WiFi
- If you need to debug, or you`re just interested, take a look thru the IO list
  on `GitHub <https://github.com/MOJOliciousFTW/HVLlab/tree/master/PWM/04_IOlist/>`_



Description
==============================================
In this lab you will auto tune a PID to control the speed of a motor. Software is done, you will do the tuning.

Your PID will be given a score, less is better.
Take a screen dump of your score and PID gains, send it to me, and receive a thumbs up for completing the lab.


The motor model can be a fun, practical challenge for three reasons

    #. The varying load is an un-measured disturbance (but you can estimate it)
    #. Deadband/sticktion, the motor doesn't turn before it gets a bit of throttle
    #. It`s comparable to cruise control subject to varying uphills.

Not to mention it`s old and worn, varying in behaviour from day to day.


The overall workflow for you to do is

    #. Turn on stuff
    #. Get to the user interface thru a browser
    #. Have fun
    #. Use the auto tuner, maybe improve tuning manually.
    #. Get a score
    #. Win

Steps
==============================================

 #. Connect to the local lab WiFi with your device (PC, smartphone, tablet) and go to http://172.31.1.97/Tc3PlcHmiWeb/Port_851/Visu/webvisu.htm.. If all is well,
    go to the next step, else:

    #. Check that the motor IO is connected to Beckhoff IO modules, see io_list
    #. Check that IO`s are connected to Beckhoff CX.
    #. Check power supply to motor, IO, CX, router. Turn these on.
    #. Wait for green lights. Else, call for help.

 #. Click PWM to get to the right screen.

 #. The SC01 (speed control) CA is a NORSOK I-005 (IEC PAS 63131) template for control of analogue
    signals (PID). Select manual, internal mode, play around with the manual output.

    #. Switch all resistors down (off).
    #. Set your manual output to something that gives a steady speed (maybe 50%).
    #. What is the resulting speed? What is the ratio between manual output and resulting speed?

 #. Set your internal mode gains. This PID is in standard form, so I and D are in units of seconds. Maybe try Kp,Ti,Td
    as 1,5,2.


 #. Try your PID

    #. Set a desired level YR as 50%
    #. Switch to auto (still internal)
    #. Observe your PID.

            #. Move the YR around
            #. Move the manual switches to vary the load
    #. Adjust tuning until you get a smooth speed control, the desired speed is reached smoothly and the switchable
       loads is handled ok.

 #. Turn off all switchable loads, run the test, get a score.

     #. Happy? Done. Else, keep tuning, ask questions, take the opportunity to understand control theory.

Reg tek rulez!

.. _Øyrane: https://www.google.com/maps/place/HVL+Robotics+Lab/@61.4590375,5.8326453,17z/data=!3m1!4b1!4m5!3m4!1s0x4616333d5f3d88b5:0x2025abbba16257dd!8m2!3d61.459035!4d5.8348393

