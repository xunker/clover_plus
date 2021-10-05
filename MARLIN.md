CloverPlus Marlin Config
==================================

After 5 years of trial and error, here is the Marlin config I use. I am using a really old version, 1.1.0 RC5, but it should work on any newer version of Marlin (except for the jerk settings which I've read has changed).

Configuration.h
---------------

Values as of Oct, 2021. If not listed here, leave it as default

```c
#ifndef MOTHERBOARD
  #define MOTHERBOARD BOARD_RAMPS_14_EFF
#endif

#define CUSTOM_MACHINE_NAME "CloverPlus"

#define EXTRUDERS 1

// :{1:'ATX',2:'X-Box 360'}
#define POWER_SUPPLY 2

#define PS_DEFAULT_ON

#define TEMP_SENSOR_0 1

#define TEMP_SENSOR_BED 0

// Enable DELTA kinematics and most of the default configuration for Deltas
#define DELTA

#define DELTA_SEGMENTS_PER_SECOND 80

#define DELTA_DIAGONAL_ROD 217.0-3.5 // This may be too much subtraction

#define DELTA_SMOOTH_ROD_OFFSET 100.429

#define DELTA_EFFECTOR_OFFSET 20.0

#define DELTA_CARRIAGE_OFFSET 18.7 // from comment on Thingiverse

#define DELTA_RADIUS (DELTA_SMOOTH_ROD_OFFSET-DELTA_EFFECTOR_OFFSET-DELTA_CARRIAGE_OFFSET)

// Print surface diameter/2 minus unreachable space (avoid collisions with vertical towers).
#define DELTA_PRINTABLE_RADIUS 60.0 // 120mm round bed

#define ENDSTOPPULLUPS
const bool X_MIN_ENDSTOP_INVERTING = true;
const bool Y_MIN_ENDSTOP_INVERTING = true;
const bool Z_MIN_ENDSTOP_INVERTING = false;
const bool X_MAX_ENDSTOP_INVERTING = true;
const bool Y_MAX_ENDSTOP_INVERTING = true;
const bool Z_MAX_ENDSTOP_INVERTING = true;
const bool Z_MIN_PROBE_ENDSTOP_INVERTING = true;

#define X_ENABLE_ON 0
#define Y_ENABLE_ON 0
#define Z_ENABLE_ON 0
#define E_ENABLE_ON 0 // For all extruders

#define X_HOME_DIR 1  // deltas always home to max
#define Y_HOME_DIR 1
#define Z_HOME_DIR 1

#define MANUAL_HOME_POSITIONS

#if ENABLED(MANUAL_HOME_POSITIONS)
  #define MANUAL_X_HOME_POS 0
  #define MANUAL_Y_HOME_POS 0
  #define MANUAL_Z_HOME_POS 117.25
#endif

#define HOMING_FEEDRATE_XYZ 2500
#define HOMING_FEEDRATE_E 0
#define HOMING_FEEDRATE { HOMING_FEEDRATE_XYZ, HOMING_FEEDRATE_XYZ, HOMING_FEEDRATE_XYZ, HOMING_FEEDRATE_E }

// 16t GT2 pulleys
#define DEFAULT_AXIS_STEPS_PER_UNIT   {50, 50, 50, 32}


#define DEFAULT_MAX_FEEDRATE          {500, 500, 500, 80}

#define DEFAULT_MAX_ACCELERATION      {3000,3000,3000,12000}

#define DEFAULT_ACCELERATION          1500
#define DEFAULT_RETRACT_ACCELERATION  1500
#define DEFAULT_TRAVEL_ACCELERATION   6000

// Suggested Delta Defaults
#define DEFAULT_XYJERK                10.0    // (mm/sec)
#define DEFAULT_ZJERK                 10.0    // (mm/sec) Must be same as XY for delta
#define DEFAULT_EJERK                 10.0     // (mm/sec)

// these values copied from Kossel config
// #define DEFAULT_XYJERK                5.0    // (mm/sec)
// #define DEFAULT_ZJERK                 5.0    // (mm/sec) Must be same as XY for delta
//  #define DEFAULT_EJERK                 10.0     // (mm/sec)

#define REPRAP_DISCOUNT_FULL_GRAPHIC_SMART_CONTROLLER
```
