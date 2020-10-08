# ZZRTL-WAAS
## ZZRTL With Audio And Stuff

These **.rtl** scripts are expansions to the sample scripts at: https://github.com/z64me/zzrtl

You must use the included **zzrtl-r5b-4.exe**.

**oot-debug.z64** and **oot-1.0.z64** are not included!

## Credit and Thanks
**z64me** for zzrtl and original scripts, **Zel** for creating scripts for expandable audio and help, **Rankaisija** for testing and vanilla folder idea, **ZeldaBoy14** and **Aria Hiroshi 64** for testing, **Dragorn421** for getting me started in zzrtl and working in C, **CloudMax** and **Gamma** for text help, and **Sauraen** for audio guidance.

## These Scripts Include
- Audiosample editing
- Audiobank editing
- Audiosequence Binaries
- Restriction Flags editing
- Entrance Cutscenes editing
- Message Binaries editing (compatible with **Zelda's Letter** and **Ocarina Text Editor**)
- Routing editing (Entrance Table)
- Custom map select for Debug *AND* 1.0

## Simple Starting Guide
1. Include **oot-debug.z64** or **oot-1.0.z64**, **oot-build.rtl**, **oot-dump.rtl**, **oot-names.tsv**, and **zzrtl.exe** in the one folder.
2. Drag & drop **oot-dump.rtl** inside **zzrtl-r5b-4.exe**.
3. Apply changes to the project using tools like **SharpOcarina**, **Custom Actor Toolkit**, **seq64**, **N64SoundTool**, **Zelda's Letter**, etc.
4. To rebuild the ROM with your changes, simply drag & drop **oot-build.rtl** inside **zzrtl-r5b-4.exe**.
5. Launch your newly modified ROM with either **build.z64** or **build-yaz0.z64**.

### A Few Notes:
- You must use a rom called **oot-debug.z64** or **oot-1.0.z64** to use these scripts.
- ZZRTL uses indexed folders and files like "4 - customcontent.bin".
- All .tsv files are editable inside of notepad and *should* look ok.
- Check out **config.tsv** in the root folder customization options.
- ZZRTL skips files and folders starting with  "_" or "." which is useful for temporarily removing content.

## About The Vanilla Folder System
Assets dumped from ocarina of time are stored inside of **vanilla** folders named "**_vanilla-debug**" or "**_vanilla-1.0**". When you add custom content to the game you should place it **outside** of the **vanilla** folder. When zzrtl rebuilds the game, it checks for custom content first before fetching the **vanilla** content from the **vanilla** folder. Even **tables** such as route.tsv can be kept outside of the **vanilla** folders. You can delete assets from the **vanilla** folders to free up space if needed. You can even dump **oot-debug** and **oot-1.0** in to the same folder and switch between builds.

## Sharp Ocarina and Custom Actor Toolkit
It is very easy to save custom content from **Sharp Ocarina** and **Custom Actor Toolkit** to your zzrtl project. In **Sharp Ocarina** you can go to file->**Save Binary** to export your scene. You will target your **.zzrpl** file in the root of your project. It will always warn you about replacing the project, just say yes. Now your custom scene will appear in the **scenes** folder. In **Custom Actor Toolkit** you compile your actor and click **send to zzrp** and target your **.zzrpl**.

## Audiobank Editing
Inside the **audio** and **banks** folder is a series of **bank** folders. Each audiobank has **.tsv** files for **instruments**, **drums**, and or **soundeffects**. To edit a bank make a copy of the bank outside of the **vanilla** folder and copy **instruments** files from other banks into the custom one. Inside the **instrument** file you can edit things like which **sample** is used, pitch, and envelope.

## Custom Audio Samples
Inside the **audio** and **audiotable** folder is a list of **sample folders**. To add a custom sample copy a sample folder to the outside of the **vanilla** folder. Then in **N64SoundTool** import a custom .wav file. Use export **16bit-Raw** and**Predictors** to replace the files inside the **sample folder**. You may also need to export and replace **Loop Predictors** if your custom sample will loop. Then open the **config.tsv** file inside the **sample folder** and copy the **start**, **end** and **count** from **N64SoundTool**.

## Custom Audio Sequences
You can import a midi file into **seq64** and export raw. That data can be placed inside the **sequences** folder, and must be appropriately indexed. eg. "6 - mysequence.bin".
To change what bank sequence uses, make a copy of **sequencetable.tsv** outside the **vanilla** folder and edit the bank number in the table.

## Message Editing
Overwrite the message binary files in the **message** folder and ouside the **vanilla** folder.
- For **Zelda's Letter**: Press *CTRL+P* and select **Application: Save Binaries**.
- For **Ocarina Text Editor**: Go to *File->Save to Extracted data*.

# Enjoy!
