remote.conf files for the Arcam AVR31 remote in default configuration.

With an Arcam receiver connect the Ugoos to the corresponding HDMI port.
The device key itself sends an IR command (not changeable) which switches the Arcam receiver to this HDMI port.
Only PVR and STB, which uses NEC codes, are usable with the Amlogic driver.

The  PVR keys has the most keys defined.

The STB device key has from the 8 blue keys only the Chapter keys defined.
Not defined remote keys: Rewind, Fastforward, Stop, Play, Pause, Record.
Use ENTER to start play, while playing use ENTER and the player controls.
Or map Play/Pause in the keymap editor to one of the color keys, or set the DISP key below to 0x60 207 # KEY_PLAY.

With PVR and STB the 4 color keys are having a strange problem with the keymap editor.
If they are defined directly as the Kodi color keys, the keymap recognice all keys with the same key number.
Because of this the color keys are defined as F1-F4 and can be mapped in the keymap editor.

The SAT and BD device keys use in default configuration RC6 keys which are not recognized from the Amlogic driver.
But it is possible to use them with the meson-ir driver.

The UHD and GAME device keys have no predefined configuration, you have to learn every key from another remote.

The AV key is predefined for a (Philips) TV.

With all device keys it is possible to learn keys from another remote.
To use the learned key in Kodi you also have to define it in remote.conf. This may not always work.
