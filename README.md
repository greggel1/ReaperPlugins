# CV Clock

## Information

This plugin provides a pulse wave generator or a steady Voltage output to synchronize VCV Rack with Reaper.
It might work also with modular gear, but I don't have any to test with.

## Installation

### Windows

Put it under AppData\\Roaming\\REAPER\\Effects\\utility in your user's directory.

### Linux

tbd

## Usage

 -  Insert a new track
 -  Uncheck "Master send" in its routes, this is very IMPORTANT
 -  Select eg. "ReaRoute 1" as its "Hardware Output"
 -  Add the plugin to the FX Section. Search for "CV Clock Generator"
 -  In VCV set the "audio-8" out module to use the ASIO driver and "ReaRoute ASIO (x64) (1-8 in, 1-8 out)" as the audio device
 -  In VCV add a Clocked/Clckd module and connect the corresponding ReaRoute "From Device" jack to "Clocked" BPM input jack
 -  Set Clocked/Clcked to p24 mode

### Options

#### Mode

  - Pulse: The plugin generates a pulse wave
  - CV: The plugin generates a steady control voltage

#### BPM By

  - Reaper: The plugin takes Reaper's BPM as tempo source
  - Plugin: The plugin takes the BPM slider as tempo source

#### BPM
  - The plugin's tempo source (30-300 BPM)

#### Divider
  - Clock division when option "Mode" is set to "Pulse".

#### Pulse Width
  - Pulse Width of the pulse wave when option "Mode" is set to "Pulse"
