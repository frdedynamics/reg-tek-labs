********************************************************
Lab 3, PID control, with feed forward, of pendulum
********************************************************

Time and place
==============================================
- HVL Robotics Lab, Øyrane_ 12, 6800 Førde, 2. floor (under Reodorklubben).
- Fridays 12-14.

Equipment
==============================================
- Matlab and Simulink
- single_pendulum.slx Simulink file from `GitHub <https://github.com/frdedynamics/reg-tek-labs/tree/master/code/>`_



Description
==============================================
In this lab you will add a feed forward term to a PID and tune a PID to control the position of a simulated pendulum.

Your PID will be given a score, less is better.
Take a screen dump of your score and PID gains, send it to me, and receive a thumbs up for completing the lab.

The pendulum model can be a fun challenge for three reasons

    #. It`s non-linear, the torque from gravity is dependant on the pendulum position
    #. It`s in every single control theory book
    #. The pendulum is simple, easy to get our head around, but still an advanced control problem


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


 #. Open the .slx file on your laptop

    #. Add feed-forward
    #. Tune PID

 #. Run the test, get a score.

     #. Happy? Done. Else, keep tuning, ask questions, take the opportunity to understand control theory.

Reg tek rulez!

.. _Øyrane: https://www.google.com/maps/place/HVL+Robotics+Lab/@61.4590375,5.8326453,17z/data=!3m1!4b1!4m5!3m4!1s0x4616333d5f3d88b5:0x2025abbba16257dd!8m2!3d61.459035!4d5.8348393
