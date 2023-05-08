Uses Marlin 2.1.1  
Projektbeschreibung: https://kanuracer.eu/index.php/3d-druck/ender-5-pro-sprite-extruder-umbau/  
You need to make some changes to your printer. For instructions: https://kanuracer.eu/index.php/3d-druck/ender-5-pro-sprite-extruder-umbau/  

Changes:
  - //#define ENDER5_USE_BLTOUCH -> #define ENDER5_USE_BLTOUCH  
	- #define CUSTOM_MACHINE_NAME "Ender-5 Pro 4.2.2" -> #define CUSTOM_MACHINE_NAME "Ender-5 Pro Sprite & BLTouch"  
	- #define TEMP_SENSOR_0 1 -> #define TEMP_SENSOR_0 11  
	- #define HEATER_0_MAXTEMP 275 -> #define HEATER_0_MAXTEMP 310  
	- #define HEATER_1_MAXTEMP 275 -> #define HEATER_0_MAXTEMP 310  
	- #define HEATER_2_MAXTEMP 275 -> #define HEATER_0_MAXTEMP 310  
	- #define HEATER_3_MAXTEMP 275 -> #define HEATER_0_MAXTEMP 310  
	- #define HEATER_4_MAXTEMP 275 -> #define HEATER_0_MAXTEMP 310  
	- #define HEATER_5_MAXTEMP 275 -> #define HEATER_0_MAXTEMP 310  
	- #define HEATER_6_MAXTEMP 275 -> #define HEATER_0_MAXTEMP 310  
	- #define HEATER_7_MAXTEMP 275 -> #define HEATER_0_MAXTEMP 310  
	- #define DEFAULT_Kp  21.73 -> #define DEFAULT_Kp  14.06  
	- #define DEFAULT_Ki   1.54 -> #define DEFAULT_Ki   1.19  
	- #define DEFAULT_Kd  76.55 -> #define DEFAULT_Kd  41.61  
	- #define DEFAULT_AXIS_STEPS_PER_UNIT { 80, 80, 800, 93 } -> #define DEFAULT_AXIS_STEPS_PER_UNIT { 80, 80, 800, 424.9 }  
	- #define Z_MIN_PROBE_USES_Z_MIN_ENDSTOP_PIN -> //#define Z_MIN_PROBE_USES_Z_MIN_ENDSTOP_PIN  
	- #define NOZZLE_TO_PROBE_OFFSET { -40, -13, -1.45 } -> #define NOZZLE_TO_PROBE_OFFSET { -31.94, -40.66, -2.92 }  
	- #define GRID_MAX_POINTS_X 3 -> #define GRID_MAX_POINTS_X 5  
	- #define Z_SAFE_HOMING_X_POINT X_CENTER  -> //#define Z_SAFE_HOMING_X_POINT X_CENTER  
	- #define Z_SAFE_HOMING_Y_POINT Y_CENTER  -> //define Z_SAFE_HOMING_Y_POINT Y_CENTER  
		○ #define Z_SAFE_HOMING_X_POINT ((X_BED_SIZE + 19.6) / 2)    // X point for Z homing  
		○ #define Z_SAFE_HOMING_Y_POINT ((Y_BED_SIZE + 36) / 2)    // Y point for Z homing  
