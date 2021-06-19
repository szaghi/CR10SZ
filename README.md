### CR10SZ, a modified CR10S 3D printer (aka cariola 2.0)

Creality CR10S is a decent 3D printer with large volume, but to obtain good quality the printing speed must be kept very low. Moreover, its usage is not straightforward, in particular for newbies (my CR10S is going to be a present for a friend of mine without any 3D printing experience). As a consequence, I modify my CR10S in order to improve speed printing (maintaining good quality) and easyness of usage.

The modifications involve both mechanics and electronics.

#### Mechanics mods

The (brief) list of mechanics mods is:

+ adopt linear rails (MGN12H) for both X and Y axis (more precise at high speed than stock wheels carriages);
+ move the 2 Z steppers to the top from the bottom in order to allow T8 screws (that are not of good quality) to work *in traction* and not *in compression*;
+ add Z frame braces to increase frame rigidity;
+ change extruder configuration from bowden to direct: a BMG (clone) extruder has been configured in direct mode over a microswiss (original) hotend; the X carriage has been designed from scratch and it allows the usage of a 5015 blower with a good-flow, short, fan duct within a very accurate inductive Z-probe for automatic bed leveling a Z-tilt-adjust.

#### Electronics mods

The (brief) list of electronics mods is:

+ use SKR 1.4 turbo mainboard with TMC 2209 drivers: in particular 2 independent drivers are used for the 2 Z axis thus, coupling the usage of Z-probe, to perform Z-tilt-adjust;
+ use BTT TFT35-E3-V3.0 display to control the printer;
+ use raspberry Pi 3 b+ to control the board by means of Klipper firmware;
+ use Wantai 42BYGHM810 Nema 17 steppers for X and Y axis, while use Stepperonline 17HS19-2004S1 Nema 17 for the 2 Z axis; the direct extruder is moved by Stepperonline 17HS08-1004S3 Nema 17 panckage stepper.

#### Overview of the final result

Combining all mods, the new CR10S (CR10SZ aka cariola 2.0) results as a standalone (no more separated control box with flying cables) 3D printer with a *Klipperized* heart that provides great quality even at high speed for this kind of kinematics and building volume and also allowing an easy web control by means of Fluidd interface.

#### Files

Many mods are taken from thingiverse and their STL are included here only for the sake of simplicity, but all rights and merits must go to their authors. Others mods as been designed from scratch: a Blender file is provided including all mods, use the blend file instead of STL if in doubt.

+ `blend/CR10SZ.blend` contains all mods, refer to it also for the assembly;
+ mods taken from thingiverse:
   + SKR mount https://www.thingiverse.com/thing:4047923
