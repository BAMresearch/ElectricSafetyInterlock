# ElectricSafetyInterlock (ESI)
Schematics, pictures, parts list and documents for an electric safety interlock (ESI). 

## Disclaimer
While this particular safety interlock design and execution has been approved by our local electronics department, rules and regulations in your area might differ. The functionality and reliability is also dependent on the build quality. The original designers hold no responsibility or liability for (modified) copies built elsewhere. Use at your own risk.

## General aim
This interlock is designed to prevent electrical shock from high voltage (>60V) equipment. 

While the general safety interlock can be generically applied, this particular example employs an external vacuum-activated switch. It is for safeguarding human operations inside a vacuum sample chamber while the chamber doors are open. The circuit is closed (output is active) when a sufficient level of vacuum is reached, i.e. when all accessible openings are necessarily closed. 

The initial application is to interrupt power to a 220V, 250W heating cartridge (itself mounted inside a small sample holder with potentially exposed contacts) when the sample chamber is open. 

The external circuit can be modified to use different interlock mechanisms as needed. Note that the external interlock circuit is only a single circuit (with two signal lines) and thus is not protected against external shorts. 

To accomodate a range of safety interlocks, the 4-pin M12 connector is wired as follows: 
Pin 1 (Brown): +24V for power supply, max current 0.6A
Pin 2 (White): Safety interlock system signal 1 (0 or 24V)
Pin 3 (Blue) : Safety interlock system signal 2 (0 or 24V)
Pin 4 (Black): 0V for power supply

The safety is interlocked (output active) when both signal pins are set high (24V), with sufficient current to activate the two relays. Pin 1 and 4 can be used to power safety hardware (such as light curtains or proximity detectors) with 24VDC up to a current of 0.6A. A larger power supply can be installed when higher currents are needed, while staying within the current limits imposed by the wiring cross-section. 

## Lights and indicators during operation
The green signal lamp indicates that the ESI is operational. 

The orange signal lamp indicates that the output is active (safety circuit closed, relays on, 230V supplied).

An extra warning light (red) is connected in such a way that, if the relays are in an unequal state, and if 230V is supplied on the interlocked circuit, the RED signal lamp lights up. This can happen when the signal cable is incorrectly wired or broken, or when one of the relays is welded closed and needs replacing. 

The power switch (red) at the back of the device indicates that power is supplied to the 24V side of the circuit. 
