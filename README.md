# Ender_Extender_400XL
Working Marlin config 

Update these values if not using Ender Extender kit or Titan style Extruder


Marlin folder contents- working Ender 3 Pro with these upgrades
Ender Extender 400XL kit  [ Bedsize 400x400 & 500 Z ]
BLTouch
BTT SKR Mini 1.3 board 
Titan style Extruder

If you are using standard bedsize, you'll need to change these 3 values in Configuration.H file
#define X_BED_SIZE 400  	//Ender 3 Pro 235
#define Y_BED_SIZE 400         //Ender 3 Pro 235
#define Z_MAX_POS 500       //Ender 3 Pro 250

Also will need to change Y Acceleration back to default
*                                      X, Y, Z, E0 [, E1[, E2...]]
#define DEFAULT_MAX_ACCELERATION      { 500, 300, 100, 5000 }   //Customized JP  Default Y = 500 -- large bed = 300


If not using Titan style Extruder, you'll need to change this value to TRUE
#define INVERT_E0_DIR false    [ True = default  FALSE = Titan style extruder ]
