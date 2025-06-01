# Audacity-Macros
Audacity Macros for automated mastering (e.g., for ACX, Spotify, etc)

##Loading Macros in Audacity

1. Open Audacity (version 3.7 used to develop these macros)
2. Navigate to "Tools" --> "Macro Manager" in the menu bar
3. Click on the "Import..." button located just left of center in the Manager window that appears.
4. Choose the macro file to import

## Applying the Macro in Audacity

All of the macros included in this repository preserve the original recording, under the assumption that the first (top most) track is the original. The macro will make a copy of the first track and mute the new preserved track (which will appear as the new last track), and then apply the adjustments to the top track in grey.

To run the macro:
1. Open Audacity (version 3.7 used to develop these macros)
2. Navigate to "Tools" --> "Apply Macro" --> <Macro Name of Your Choice>
3. Let the macro run. It will pop up several temporary windows as it works, and finish with a status message.

To re-run the macro, move the preserved original track back to the first rack position and repeat the above steps.

## Macro Details

### Audacity Macro_Audiobook Mastering for ACX.txt

Depends on the following (free) plug-ins:
- ACX_Check (https://plugins.audacityteam.org/analyzers/analysis-plugins) for Peak, RMS, and Noise Floor checks.
- OpenVino Whisper (https://plugins.audacityteam.org/ai-plugins/ai-plugins) for audio transcription as an editing and verification aid.
- TDR Nova (https://www.tokyodawn.net/tdr-nova/free/) for Dynamic (reactive) EQ Sibilance taming.

Adjustments are made based on recordings for a female narrator in a treated room using an MXL Cr24 mic and ZoomH4 Interface. EQ adjustments may be needed to fit other voices and recording setups, particularly regarding sibilance and resonance frequencies.
Be sure to follow the instructions to enable OpenVino (e.g., go to Edit-->Preferences --> Modules --> mod-openvino = Enabled) the first time. 

### Audacity Macro_Audiobook Mastering for ACX_Deluxe.txt

This version also provides noise suppression (bringing the noise floor even lower), ensures 44.1KHz sample rate, and prompts the user for MP3 Meta-data.

Depends on the following (free) plug-ins:
- ACX_Check (https://plugins.audacityteam.org/analyzers/analysis-plugins) for Peak, RMS, and Noise Floor checks.
- OpenVino Whisper & NoiseSuppression (https://plugins.audacityteam.org/ai-plugins/ai-plugins) for audio transcription as an editing and verification aid.
- TDR Nova (https://www.tokyodawn.net/tdr-nova/free/) for Dynamic (reactive) EQ Sibilance taming.

Adjustments are made based on recordings for a female narrator in a treated room using an MXL Cr24 mic and ZoomH4 Interface. EQ adjustments may be needed to fit other voices and recording setups, particularly regarding sibilance and resonance frequencies.
Be sure to follow the instructions to enable OpenVino (e.g., go to Edit-->Preferences --> Modules --> mod-openvino = Enabled) the first time. 

### Audacity Macro_Audiobook Mastering for ACX_lite.txt
Similar to the non-lite version, but removes any dependancies (i.e., default Audacity functions only)
This version will not provide dynamic EQ (just static EQ), full ACX check, nor auto-transcription labels
Adjustments are made based on recordings for a female narrator in a treated room using an MXL Cr24 mic and ZoomH4 Interface. EQ adjustments may be needed to fit other voices and recording setups, particularly regarding sibilance and resonance frequencies.

