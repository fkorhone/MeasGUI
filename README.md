# MeasGUI
MeasGUI - Measurement Graphics User Interface

## Depencies
MeasGUI depend on RMCIOS. Copy RMCIOS implementation to the root folder of the application.

## Connection between MeasGUI and RMCIOS 
Connection can be esbalished between two ways:
1. Local (LOCAL) connection using stdin/stdout rediection. Redirection is implemented in run\_program.dll and labview program call functions from this library to invoke stdin and out operations to the measurement program.

2. Windows pipe. (PIPE)
RMCIOS create named pipe. 

## Copying and credits

MeasGUI - Measurement Graphics User Interface
Copyright (c) 2018 Frans Korhonen

MeasGUI was originally developed at Institute for Atmospheric 
and Earth System Research / Physics, Faculty of Science, 
University of Helsinki, Finland

Assistance, experience and feedback from following persons have been 
critical in development of MeasGUI: Michel Attoui, Juha Kangasluoma, 
Lauri Ahonen, Ella Häkkinen, Markku Kulmala and Tuukka Petäjä.

This file is part of MeasGUI. This notice was encoded using utf-8

This Source Code Form is subject to the terms of the Mozilla Public
License, v. 2.0. If a copy of the MPL was not distributed with this
file, You can obtain one at http://mozilla.org/MPL/2.0/. 

## Source Files

###meas\_gui.lvproj
Project file for building MeasGUI with all features.

###command\_channel.vi
VI block for communicatig with RMCIOS systems in a various ways.

###draw\_to\_matlab.vi
Vi block for drawing, plotting and scatter directly to matlab.  

###application\_path.vi
Utility VI for determining location of running LabVIEW program. 
(works when run from both: VI or compiled exe)

###draw\_to\_matlab.vi
Vi block for drawing, plotting and scatter directly to matlab.  

###form\_3D\_data.vi
Creates 2d intensity Matrix and axes data, from sparse 3 vecor data. Intended for creating 3d plots.

###front\_panel\_ctl\_save.vi
Utility function for saving the sate of named front panel controls.

###hardware\_configurator.vi
Template tool for creating RMCIOS hardware related configurations graphically.

###log\_controls.vi
Vi tool for logging state of named front panel controls.

##log\_key\_variant.vi
Vi block for saving different kind of data to a bytestream

##meas\_gui.vi
Measurement graphics user interface main program.

##measurement\_configurator.vi
Template tool for creating RMCIOS measurement related configurations graphically.

##multidimensional\_ramp.vi
Vi block for creating multidimensional scan ramps/step sequences to a 2-Dimensional array.

##ramp.vi
Vi block for creating linear ramps/step step sequences to a 1 -dimensional array.

##run\_program.vi
Vi block for calling another program using RMCIOS run\_program.dll utility program. 
stdin/stdout get redirected for the program and can be controlled and read from labview.

##windows\_file.vi
Vi for calling windows file api directly. Used for using special windows file handles eg. pipes.

