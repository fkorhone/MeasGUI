Copyright (c) 2018 Frans Korhonen, Institute for Atmospheric and Earth System Research / Physics, Faculty of Science, University of Helsinki, Finland
This file is part of MeasGUI.

This Source Code Form is subject to the terms of the Mozilla Public
License, v. 2.0. If a copy of the MPL was not distributed with this
 file, You can obtain one at http://mozilla.org/MPL/2.0/. 

Meas GUI - Measurement Graphics user Interface for RMCIOS (channel system)
Compiled originally with LabVIEW 2015

Labview sources:
meas_gui_nomatlab.lvproj
Project file for building MeasGUI executable without matlab linkage. (does not start matlab)
(project -> propertios -> conditional disable symbols: NO_MATLAB=1)
Project also build hardware_configurator.exe and measurement_configurator.exe

meas_gui.lvproj
Project file for building MeasGUI with all features.

command_channel.vi
VI block for communicatig with RMCIOS systems (channel_system) in a various ways.

draw_to_matlab.vi
Vi block for drawing, plotting and scatter directly to matlab.  

application_path.vi
Utility VI for determining location of running LabVIEW program. 
(works when run from both: VI or compiled exe)

draw_to_matlab.vi
Vi block for drawing, plotting and scatter directly to matlab.  

form_3D_data.vi
Creates 2d intensity Matrix and axes data, from sparse 3 vecor data. Intended for creating 3d plots.

front_panel_ctl_save.vi
Utility function for saving the sate of named front panel controls.

hardware_configurator.vi
Template tool for creating RMCIOS (channel_system) hardware related configurations graphically.

log_controls.vi
Vi tool for logging state of named front panel controls.

log_key_variant.vi
Vi block for saving different kind of data to a bytestream

meas_gui.vi
Measurement graphics user interface main program.

measurement_configurator.vi
Template tool for creating RMCIOS (channel_system) measurement related configurations graphically.

multidimensional_ramp.vi
Vi block for creating multidimensional scan ramps/step sequences to a 2-Dimensional array.

ramp.vi
Vi block for creating linear ramps/step step sequences to a 1 -dimensional array.

run_program.vi
Vi block for calling another program using RMCIOS run_program.dll utility program. 
stdin/stdout get redirected for the program and can be controlled and read from labview.

windows_file.vi
Vi for calling windows file api directly. Used for using special windows file handles eg. pipes.
