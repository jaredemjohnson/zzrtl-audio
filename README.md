# ZZRTL-WAAS
## ZZRTL With Audio And Stuff

These **.rtl** scripts are expansions to the sample scripts at: https://github.com/z64me/zzrtl
Go there for a zzrtl full starter guide.

**oot-debug.z64** and **zzrtl.exe** not included!

## These Scripts Include
- Audiobank editing
- Audiosequence Binaries editing
- Restriction Flags editing
- Entrance Cutscenes editing
- Message Binaries editing (compatible with **Zelda's Letter** and **Ocarina Text Editor**)
- Routing editing (Entrance Table)

## Simple Starting Guide
1. Include **oot-debug.z64**, **oot-build.rtl**, **oot-dump.rtl**, **oot-names.tsv**, and **zzrtl.exe** in the one same folder.
2. Drag & drop **oot-dump.rtl** inside **zzrtl.exe**.
3. Apply changes to the project using tools like **SharpOcarina**, **Custom Actor Toolkit**, **Zelda's Letter**, etc.
4. To rebuild the ROM with your changes, simply drag & drop **oot-build.rtl** inside **zzrtl.exe**.
5. Launch your newly modified ROM with either **build.z64** or **build-yaz0.z64**

### All the tables related to scenes will be dumped to the **scene** folder.

## Audiobank Editing
Inside the **audio** and **banks** folder is a list of audiobanks. Each audiobank is comprised of instruments folders. Move/copy instrument folders from one bank to another and edit the config file inside the **instrument** folder to change the instrument's envelope and pitch.

(The binary files inside the **bank** folder are mostly for debugging. leave them alone.)

## Message Editing
Overwrite the message binary files in the **message** folder.

- For **Zelda's Letter**: Press *CTRL+P* and select **Application: Save Binaries**.
- For **Ocarina Text Editor**: Go to *File->Save to Extracted data*.

# Enjoy!
