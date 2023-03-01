# ElectricSafetyInterlock (ESI)
Schematics, pictures, parts list and documents for an electric safety interlock (ESI). 

## disclaimer
While this particular safety interlock design and execution has been approved by our local electronics department, rules and regulations in your area might differ. The functionality and reliability is also dependent on the build quality. The original designers hold no responsibility or liability for (modified) copies built elsewhere. Use at your own risk.

## General aim
This interlock is designed to prevent electrical shock from high voltage (>60V) equipment. 

While the general safety interlock can be generically applied, this particular example employs an external vacuum-activated switch. It is for safeguarding human operations inside a vacuum sample chamber while the chamber doors are open. The circuit is closed (output is active) when a sufficient level of vacuum is reached, i.e. when all accessible openings are necessarily closed. 

The initial application is to interrupt power to a 220V, 250W heating cartridge (itself mounted inside a small sample holder with potentially exposed contacts) when the sample chamber is open. 

The external circuit can be modified to use different interlock mechanisms as needed. Note that the external interlock circuit is only a single circuit and thus is not protected against external shorts. 

## lights and indicators
The green signal lamp indicates that the ESI is operational. 

The orange signal lamp indicates that the output is active (safety circuit closed, relays on, 230V supplied).

An extra warning light (red) is connected in such a way that, if one of the relays is welded closed and thus the relays are in an unequal state, the RED signal lamp lights up. When this happens, the relays need to be replaced. 

The power switch (red) at the back of the device indicates that power is supplied to the 24V side of the circuit. 
