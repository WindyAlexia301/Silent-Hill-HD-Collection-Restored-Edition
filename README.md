# Silent-Hill-HD-Collection-Restored-Edition
A Fan-Made Patches That Fix The Hijinx Studios Shit (W.I.P)


# FORUM FROM EMU-LAND.NET

(X360)

VGM tool box (extract audio)
----------------------------
Note:Go to Misc.Tools->Extraction Tools->Generic->Advanced Cutter/Offset Finder
Criteria: 52494646
Treat as Hex:+
Extract Files:+
Output File Extension: .XMA
Use Terminator String: 52494646
Treat as Hex:+
Cut to EOF when Terminator Not Found:+
Source Files: DEV\sh2_360\data\sound\s_force*.SFC - soundpacks
Source Files: DEV\sh2_360\data\sound\sound_da*.SND - soundpacks
Source Files: DEV\sh3_360\data\sound*.SND - soundpacks

VGM tool box (convert audio)
----------------------------
Note1: towav.exe,xma_test.exe,xmaencode.exe must be in vgmtoolbox\external\xma\ folder
Note2:Go to Misc.Tools->XMA->XMA Converter
Presets: [XBOX360] Fallout: New Vegas
Load: +
Use xma_parse.exe: +
XMA Type: 2
Ignore Errors: +
Set Start Offset after RIFF Header: +
Edit Block Size: 0x20000
Get DATA Size from RIFF Header: +
Get Frequency from RIFF Header: +
Get Channels from RIFF Header: +
Execute ToWav.exe on the Output Files: +
Drag and Drop.XMA in window
DEV\data\launcher*.XMA - music(MS XMA2)

xmash 0.8(extract XMA and POS)
------------------------------------
Note: create batch file with command:
for %%a in (.XMA) do xmash.exe "%%a"
DEV\sh2_360\data\sound**.XMA - music, sounds, speech, fonsound(MS XMA)
DEV\sh3_360\data\sound**.XMA - music, sounds, speech, fonsound(MS XMA)
frequency: 48000
Channels: 6, 2

ToWav Music Converter v.17.04.2009(XMA to WAV)
------------------------------------
Open File:
DEV\sh2_360\data\sound**.XMA ->.XMA - music, sounds, speech, fonsound(MS XMA)
DEV\sh3_360\data\sound**.XMA ->.XMA - music, sounds, speech, fonsound(MS XMA)
frequency: 48000
Channels: 2

Any Media Player
------------------------------------------------------------------------
DEV\sh2_360\data\sound**.XMA ->.XMA ->.WAV - music, sounds, speech, fonsound(PCM WAV)
DEV\sh3_360\data\sound**.XMA ->.XMA ->.WAV - music, sounds, speech, fonsound(PCM WAV)
frequency: 48000
Channels: 2

in_vgmstream (winamp plugin)(play \ convert)
--------------------------------------------
DEV\sh2_360\data\sound**.XMA ->.XMA ->.WAV - music, sounds, speech, fonsound(PCM WAV)
DEV\sh3_360\data\sound**.XMA ->.XMA ->.WAV - music, sounds, speech, fonsound(PCM WAV)
DEV\sh2_360\data\sound**.XMA ->.POS - header(Little Endian 16-bit PCM: RIFF WAVE header and .pos for looping)
DEV\sh3_360\data\sound**.XMA ->.POS - header(Little Endian 16-bit PCM: RIFF WAVE header and .pos for looping)
frequency: 48000
Channels: 2

RAD Video Tools (play \ convert)
------------------------------------
DEV\sh2_360\data\movie*.BIK - video(BIK)
DEV\sh3_360\data\movie*.BIK - video(BIK)

xbdecompress from XDK(unpack LZX)
------------------------------------------------------------------------
Note: create batch file with command:
for /r %%x in (.) do xbdecompress.exe "%%x" "%%x.new"
DEV\sh**. - datafiles
DEV\sh2_360\data\etc\message*.MES - text
DEV\sh3_360\data\msg*.MES - text
DEV\sh2_360\data\font*.TEX - fonts
DEV\sh3_360\data\font*.TEX - fonts
DEV\sh2_360\data\globtex*.DDS - graphics
DEV\sh3_360\data\globtex*.DDS - graphics
DEV\sh2_360\data\pic**.TEX - graphics
DEV\sh3_360\data\pic**.TEX - graphics

Any Image Viewer
------------------------------------------------------------------------
DEV\data\launcher*.DDS - graphics(DDS)
DEV\sh2_360\data\font*.TEX ->.DDS - fonts(DDS)
DEV\sh3_360\data\font*.TEX ->.DDS - fonts(DDS)
DEV\sh2_360\data\globtex*.DDS ->.DDS - graphics(DDS)
DEV\sh3_360\data\globtex*.DDS ->.DDS - graphics(DDS)
DEV\sh2_360\data\pic**.TEX ->.DDS - graphics(DDS)
DEV\sh3_360\data\pic**.TEX ->.DDS - graphics(DDS)




(PS3)

VGM tool box r837(extract)
----------------------------
Note:Go to Misc.Tools->Extraction Tools->Generic->Advanced Cutter/Offset Finder
Criteria: 4D534643
Treat as Hex:+
Extract Files:+
Output File Extension: *.MSF
Use Terminator String: 4D534643
Treat as Hex:+
Cut to EOF when Terminator Not Found:+
Source Files: DEV\\PS3_GAME\USRDIR\sh2\data\sound\s_force\*.SFC - sound
Source Files: DEV\\PS3_GAME\USRDIR\sh2\data\sound\sound_dat\*.SND - sound
Source Files: DEV\\PS3_GAME\USRDIR\sh3\data\sound\*.SND - sound

QuickBMS,script “MSF to AT3.bms”(add at3 header)
------------------------------------
*Note:unplayble 6 and 1 Channel
Open File:
DEV\\PS3_GAME\USRDIR\sh2\data\sound\adx\voice\*.AT3 - speech(ATRAC3 codec)
DEV\\PS3_GAME\USRDIR\sh3\data\sound\*\*.AT3 - speech, fonsound(ATRAC3 codec)
DEV\\PS3_GAME\USRDIR\sh3\data\sound\*\*.AT3 - music(ATRAC3 codec)*
DEV\\PS3_GAME\USRDIR\sh2\data\sound\adx\voice\*.NEW - speech(ATRAC3 codec)*
DEV\\PS3_GAME\USRDIR\sh2\data\sound\adx\*.AT3 - music, fonsound(ATRAC3 codec)*
DEV\\PS3_GAME\USRDIR\launch\data\launcher\*.AT3 - music, fonsound(ATRAC3 codec)*

Sony Sound Forge v.9.0(play \ convert)
------------------------------------
Open File:
DEV\\PS3_GAME\USRDIR\sh2\data\sound\adx\voice\*.AT3 ->*.AT3 - speech(ATRAC3 codec)
frequency: 48000
bitrate: 104 Kbps
Channels: 2

Installed ATRAC3 codec in OS and Any WAV Convertor \ Player(play \ convert)

For Example:FLV to AVI MPEG WMV 3GP MP4 iPod Converter, GoldWave 5.16, MMConvertGUI Version 1.0.5
------------------------------------
Open file:
DEV\\PS3_GAME\USRDIR\sh2\data\sound\adx\voice\*.AT3 ->*.AT3 - speech(ATRAC3 codec)
frequency: 48000
bitrate: 104 Kbps
Channels: 2

RAD Video Tools (play \ convert)
------------------------------------
DEV\\PS3_GAME\USRDIR\sh2\data\movie*\*.BIK - video(BIK)
DEV\\PS3_GAME\USRDIR\sh3\data\movie\*.BIK - video(BIK)

Any Image Viewer
------------------------------------------------------------------------
Note: rename *.TEX to *.DDS
DEV\\PS3_GAME\USRDIR\launch\data\launcher\*.DDS - graphics, fonts(DDS)
DEV\\PS3_GAME\USRDIR\sh2\data\font\*.TEX ->*.DDS - fonts(DDS)
DEV\\PS3_GAME\USRDIR\sh2\data\*\*.DDS - graphics(DDS)
DEV\\PS3_GAME\USRDIR\sh3\data\font\*.TEX ->*.DDS - fonts(DDS)
DEV\\PS3_GAME\USRDIR\sh3\data\*\*.DDS - graphics(DDS)
DEV\\PS3_GAME\USRDIR\sh*\data\*\*.TEX ->*.DDS - graphics(DDS)

Hex Workshop(edit)
--------------------------------------------
DEV\\PS3_GAME\USRDIR\sh2\data\etc\message\*.MES - text(BIN)
DEV\\PS3_GAME\USRDIR\sh3\data\msg\*.MES - text(BIN)
--- Конец кода ---
