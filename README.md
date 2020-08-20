# zzrtl-complete
Complete is an overstatement.

These .rtl scripts are expansions to the sample scritps at:<br>
https://github.com/z64me/zzrtl<br>
go there for a zzrtl full starter guide.<br>

oot-debug.z64 and zzrtl.exe not included!

[ simple starter guide ]<br>
-inculde oot-debug.z64, oot-build-complete.rtl, oot-dump-complete.rtl, oot-names.tsv, and zzrtl.exe in the same folder.<br>
-open oot-dump-complete.rtl with zzrtl.exe<br>
-apply changes to the project using tools like Sharp Ocarina, Custom Actor Toolkit, Zelda's Letter.<br>
-open oot-build-complete.rtl with zzrtl.exe<br>
-run build.z64

[ These scripts include ]<br>
-audiobank editing<br>
-audiosequence binaries<br>
-restriction flags<br>
-entrance cutscenes<br>
-message binaries (compatible with Zelda's Letter and Ocarina Text Editor)<br>
-routing (entrance table)<br>

All the tables related to scenes will be dumped to the [scene] folder.

[audiobank editing]<br>
Inside the [audio] and [banks] folder is a list of audiobanks.<br>
each audiobank is comprised of instruments folders. <br>
Move/copy instrument folders from one bank to another <br>
and edit the config file inside the instrument folder <br>
to change the instrument's envelope.<br>
<br>
there are binary files inside the bank folder that are mostly for debugging. <br>
leave them alone.<br>
<br>
[message editing]<br>
overwrite the message binary files in the [message] folder<br>
ZELDA'S LETTER: Press ctr-P and select "application: save binaries"<br>
OCARINA TEXT EDITOR: Go to File->Save to Extracted data.<br>

Enjoy!
