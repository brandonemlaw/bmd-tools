bmd-tools
=========

Tools to connect with and manage Blackmagic Design video
equipment with built-in H.264 encoder.

Currently tested device:

 * ATEM TV studio
 * H.264 Pro Recorder

Use *bmd-extractfw* to extract the firmware out from
BMDStreamingServer.exe (part of the Windows drivers).

*bmd-streamer* can be used to upload the extracted firmwares,
and to stream out (currently to stdout) the MPEG TS stream
from the device. For example, to dump stream to vlc you could
do "bmd-streamer | vlc stream:///dev/stdin".

Dependencies:
 * libusb (1.0.16 or newer) or libusbx

