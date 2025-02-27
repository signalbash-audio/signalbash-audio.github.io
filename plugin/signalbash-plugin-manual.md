---
title: The Signalbash Plugin
layout: home
nav_order: 3
---


# Signalbash Plugin Manual

The Signalbash Plugin is a free and open source audio plugin that you
can use in your DAW to track how long you've been actively working
on creating music, podcasts, or other types of audio content.

## Downloading & Installing The Plugin

The Signalbash Plugin can be downloaded from
[https://signalbash.com/plugin-download](https://signalbash.com/plugin-download).

The download page on signalbash.com will prompt you to download the installer compatible with your computer.

## Plugin Types

The installer will give you the option to install the following plugin types:

- VST3 ( macOS \| Windows \| Linux )
- CLAP ( macOS \| Windows \| Linux )
- AAX ( macOS \| Windows )
- AU (macOS only)


VST2 is not available.


### If Signalbash doesn't appear after installation

If you're using a DAW or on an OS that doesn't support CLAP or AU, you might
not see the Signalbash plugin appear immediately. For example, if you're
using Ableton Live 11 or earlier on a Windows computer.

This is likely because some DAWs don't enable VST3 plugins by default, and will
initially only display installed VST plugins from your VST2 folder. 

If you don't see the plugin listed in your DAW's plugins list, ensure
that your DAW has the VST3 folder enabled. This process is slightly different
for each DAW, but generally involves toggling a checkbox in the DAW's
settings/preferences.

Once you've verified that you've enabled VST3 in your DAW, click rescan
plugins, and Signalbash should appear.


## System Requirements

Signalbash is very lightweight & performant.
If your machine can effectively run DAW/NLE
software, you won't have an issue adding the Signalbash plugin to a session.

In order to run the plugin, your Host software must be capable of loading
one of the plugin formats shown the Plugin Types section above.

Signalbash also requires an internet connection in order to properly save
activity.

Signalbash is only available for 64 bit machines.

Signalbash is available for macOS, Windows, & Linux machines.

### macOS

Signalbash can be installed & run on macOS version 10.11 or greater. Both Intel
& ARM architectures are supported.

### Windows

Signalbash can be run on machines running the Windows operating system
with Windows 7 or greater.

Signalbash is not currently available natively on Windows machines with
ARM processors.

### Linux

Signalbash can be installed & run on x64 (amd64/x86_64) and ARM64/aarch64
Linux Operating Systems.


## Installation Locations

The Installer will install each plugin type at the following locations on your
computer:

### macOS

- Signalbash.vst3: `/Library/Audio/Plug-Ins/VST3`
- Signalbash.clap: `/Library/Audio/Plug-Ins/CLAP`
- Signalbash.component: `/Library/Audio/Plug-Ins/Components`
- Signalbash.aaxplugin: `/Library/Application Support/Avid/Audio/Plug-Ins`

### Windows

- Signalbash.vst3: `C:\Program Files\Common Files\VST3`
- Signalbash.clap: `C:\Program Files\Common Files\CLAP`
- Signalbash.aaxplugin: `C:\Program Files\Common Files\Avid\Audio\Plug-Ins`

### Linux

Linux installation is performed manually by unzipping the
appropriate zip file containing the Signalbash Plugin types, and
placing them in the desired directories. Common locations include the
following:

- Signalbash.clap:
    - `~/.clap`
    - `/usr/lib/clap`
- Signalbash.vst3:
    - `~/.vst3`
    - `/usr/lib/vst3/`
    - `/usr/local/lib/vst3/`


## Uninstalling

To uninstall the plugin, visit the locations on your computer specified above in
the Installation Locations section and delete the plugin files.


## Plugin Usage

### UI

The plugin consists of three views:

- The Main View

    The main view is the default and features the Signalbash logo mark.

- Session Key Input

    This view is where you can update or change your session key. It opens
    when you load the plugin for the very first time, and can then be
    accessed through the settings view.

- Settings View

    This view allows you to see the DAW/NLE host software detected by the
    plugin, an obfuscated view of your session key, and has an option to
    disable the logo rotation animation. You can also copy or change
    your session key through this view.

All views have a toolbar indicating the current state/network status of the
plugin, and can help diagnose any issues.


### First Use & Setup

In order to start tracking activity in a DAW session, a session key must be
set in the plugin. You can get your session key from your account on
signalbash.com. See the [Session Key](/website/session-key) page for more info.

Once you input your key & hit submit, the plugin will verify the session key
is valid.

If the session key is valid, the plugin will move to the default view, which
should show a green status indicator indicating the session key is verified,
and your internet connection is online and ready to submit your activity.

If the session key is invalid, the indicator will report that it can't
validate the key. You can retry the validation if this is the case.

If your internet connection is offline when you go to validate your key, the
plugin will also report that it cannot validate the key. Ensure your internet
is working, then try again using the retry button.

Once your session key is setup & validated, you won't need to go through this
process again. Every time you initalize the plugin in an new session,
the session key you setup will automatically be loaded. You can however change
your session key at any time if necessary (see the next section).


### Changing Your Session Key

If you've misentered your session key, or want to use a session key
associated with another account, you can do so in the plugin settings.

In the upper right corner of the plugin UI, there is a settings cog button

Click this button to open the settings view. Here, you can click the "Change
Session Key" button to re-open the session key input, and input the new value.

With a new key, the plugin will attempt to validate the key in the same manner
as described above.


### Routine Use

The plugin UI does not need to be open in order to track your activity. However,
a valid session key needs to be set in order for it to work properly.

When the plugin detects a signal, the logo will begin to rotate. This indicates
that your activity is being registered locally by the plugin, and will shortly
be reflected in your Signalbash Account.

### Activity Submission

The plugin will submit your activity to your account approximately every two
minutes.

In the settings view, there is a progress bar that will move across the UI
underneath the toolbar. Shortly after the bar reaches the end of the screen
and "restarts" any unsubmitted activity detected by the plugin will be submitted
to your Signalbash account.

### Plugin Settings View

The plugin settings view allows you to see what host you're running the plugin
through. This is sent along with your activity to be displayed on your
account in the Signalbash Leaderboard.

If the host name displays the value "Unknown" that means you're running the
plugin on a DAW that Signalbash does not currently fully support. If you
want to have this host software formally added, please report an issue on
the issue tracker: 
[Issue Tracker](https://github.com/signalbash-audio/signalbash/issues)

You can also copy your full session key to your clipboard in this view.
This is useful if you're trying to log back into your account and you
have forgotten your password. See the [Session Key](/website/session-key)
help page for more info.

The Change Session Key button will allow you to change the session key the
plugin is currently using to report activity.

If you want to disable the rotation of the logo to indicate that activity
is being registered, you can uncheck the "Enable Animation" checkbox.
If you do this, activity will still be recorded by the plugin, but the
animation won't spin. This functionality will persist between sessions until
you change it.

To return to the Main View, click the settings cog button again.

### Bypassing

You can bypass the plugin entirely through your DAW's native functionality.
If you do so, the plugin will still submit any pending activity to your
account, but any additional activity will not be saved until you re-enable
the plugin.


### Closing a session

If you close a session where the Signalbash plugin is active, any pending
unsubmitted activity will be discarded.

Since the plugin submits activity every two minutes, the maximum unreported
activity will also be two minutes, assuming your internet connection is
healthy.


### Multiple Instances in a Single Session

If you open multiple instances of the plugin in a single session, Signalbash
will discard all activity from all instances except for the one
reporting the highest amount of
activity. This is done to ensure your activity is not over-reported.

This process may be imperfect and may not be reflected instantaneously.
As such, it's
recommended you only add a single instance of the plugin to your master.


### Connection Offline Retry Behavior

Occasionally, signalbash.com may be temporarily offline for maintenace,
or your internet
connection may briefly go down. When this occurs, the status indicator
will change to red in the plugin toolbar to reflect this.

The plugin will automatically attempt to retry submission when it receives an error
until either your internet or signalbash.com comes back
online. Once a connection is re-established, the indicator will show green
"Connection Healthy" status again.

During any downtime from either end, your activity will still be saved
locally through the plugin, and will appear in full in your Signalbash account
once the connection is re-established.

If you have unsubmitted activity in this situation, and you exit your DAW session,
any pending activity gets discarded, and will not be reflected in your account.


## Audio Transparency

When placed on any track or bus in a DAW, the Signalbash Plugin allows
audio to pass through unaltered.

Because the plugin does not affect audio in any way, it is safe to place anywhere on the master chain. Additionally, you do not have to worry about bypassing or
removing the plugin before exporting/bouncing your audio to a file.

Most importantly, **The Signalbash Plugin Does Not Save, Send, or Cache Your
Actual Audio At Any Point**. The plugin is only timing the duration in which
your audio goes above an audible dB threshold, and reporting this information
to signalbash.com, along with the particular DAW you're using, and the time at
which the audible signal was detected.

## System Clock Settings

The Signalbash plugin gets the current time from the your computer where
you're running your DAW.
In most cases, this should be accurate, as most operating systems set the
time automatically.

However, if you set your time/timezone manually, or you purposefully have your
system clock set to be innacurate, the activity may not correctly be reported.
This may mean that your activity could appear inaccurate or not appear in your
account at all.

If this is occuring, reset the clock back to the current time in your system
preferences.
After you've
reset the time, remove the plugin from your session, and then re-add it.
This will resync the
plugin, and subsequent activity should be accurately reported again.


## What type of DAW usage does Signalbash not detect?

Signalbash can only detect activity if there's an audio signal being
sent through the channel/bus where the plugin is placed. Any usage of
your DAW while audio isn't playing can't be quantified or detected,
and thus won't count towards your activity totals. For example: changing
DAW settings, re-organizing/grouping tracks, etc. 

Additionally, certain tasks in a DAW may play audio,
but not route that audio through
the master, such as previewing audio samples that can
be browsed and played through your DAW's UI.


## Usage with Video Editing Software

Certain video editors/non-linear editing software programs support the
use of audio plugins. Currently, Signalbash can report activity from
Adobe Premiere Pro, Davinci Resolve, and Apple Final Cut Pro.

Video editing workflow are distinct from working in a DAW, as video
editing tasks may not involve working with audio at all.

In order for the Signalbash plugin to report activity, it requires
an audio signal to be running through the mix bus/channel where it is
placed. When you're performing editing tasks where no audio is
actively playing, no activity will be reported, even if the timeline
playhead is moving. For example, if you're cutting video without audio, or performing coloring & other VFX related tasks.


## Supported Channel Layouts

Signalbash can be placed on tracks with the following channel layouts:

- Mono
- Dual Mono
- Stereo


## Supported DAW / NLE / Host Software

Signalbash can be used in any DAW/NLE running on one of the above supported
operating systems (see "System Requirements Section Above") that can
load plugins in one or more of the following plugin formats:

- VST3
- CLAP
- AAX
- AU


### Host Name Recognition

While Signalbash can be loaded and properly detect activity in any host
program meeting the above requirements, the Signalbash Plugin can only
detect the name of the DAW/NLE for the following:

- Ableton Live
- Adobe Audition
- Adobe Premiere
- Apple GarageBand
- Apple Logic Pro
- Apple MainStage
- Ardour
- Pro Tools
- Bitwig Studio
- Cakewalk Sonar
- Cakewalk by Bandlab
- DaVinci Resolve
- Digital Performer
- Final Cut
- FL Studio
- Magix Samplitude
- Magix Sequoia
- Pyramix
- Muse Receptor
- NI Maschine
- Reaper
- Reason
- Renoise
- SADiE
- Steinberg Cubase
- Steinberg Nuendo
- Steinberg Wavelab
- Studio One
- Tracktion Waveform
- Vienna Ensemble Pro
- WaveBurner

This means that the Plugin will report "Unknown" or "Other" in your
account or leaderboard if you're using software not in the above list.
The detected name of the host software can also be viewed in the
"Settings" view of the Signalbash plugin (click the settings cog icon
in the plugin toolbar to open this view).

### Requesting Support for New DAWs

It's the intent of Signalbash to accurately support activity reporting
for as many DAWs as possible. If you're using a host that gets
reported as Other or Unknown, please open an issue request through one
of the following methods:

- Open an issue on the Signalbash Issue Tracker:
  [Issue Tracker](https://github.com/signalbash-audio/signalbash/issues) 
- DM Signalbash directly: [Link](https://x.com/signalbash)


## License & Source

The Signalbash Plugin is Free & Open Source Software, licensed under the
AGPL-v3.0. You can obtain a copy of the plugin source at
[github.com/signalbash-audio/signalbash](https://github.com/signalbash-audio/signalbash)
