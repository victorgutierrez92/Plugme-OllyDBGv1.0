Memory data conversion OD-Plugin
;================================================= ==============================================
This plug-in memory data can be converted into (asm, vb, vc, delphi) programming language and static arrays
Masm32 source code. Can be said to incorporate "memory data format conversion. Dll" and "Asm2Clipboard.dll",
But the solution there are two plug-in bug. This powerful plug-ins a lot Oh, greatly facilitate the work of anti-source ....

Selected code or data, and then right "data conversion"
Converted data in the ClipBoard, right out to you can paste


[B] download the attachment [url = http://www.unpack.cn/redirect.php?goto=findpost&pid=897281&ptid=61200] 172 # [/ url] [i] ttabcs [/ i] [/ b]

;============================== Q & Operating Tips =============== =======================================

<1> Q: How large range of selected data block?
A: click on "Start address", then skip to the "end address", then press the "Shift" key, then click the "End address" position.

<2> Q: Why is point "package functor process" when the crash?
A: Because too many children in the process of Call, disassemble the data out of time, it will be wrong, in the. Net more prominent in this issue.

<3> Q: Why does not the configuration file, how to modify?
A: I personally can directly modify the configuration dll file, modify the file pointer at the 400H, numeric hexadecimal number, yes / no with a '1 ', '0'
EditDlg = <0 or 1>; whether to convert data pop-up dialog box Text
LineCount = <Hex Values ​​"; set the number of data per line
SetTabLen = <Hex Values ​​"; Settings Tab aligned digits, if not 0, then use a space instead of N
MultiAsmLabel = <0 or 1>; set MUltimate Assembler plug label

;============================== Update History ================= ============================================

2011-03-01
Setting Tab align with the median SetTabLen = <hexadecimal Values ​​", and the other to change the mode of application memory to reduce memory for pasting board.

2011-02-27
Fixed problem of disassembly when int3 breakpoint

2011-02-26
Dump with dump and load data, corrected some minor errors.

2011-02-23
MUltimate Assembler v1.3 plus the label on the support switch MultiAsmLabel = <0 or 1>, in FileIP: 0420h at
With signature extraction function.

2011-02-22
Clear the address of the module with the name of the other sub-processes if there is added the function name, the resulting sub-procedure name proc directly

2011-2-10
Box with shells the number of options and data line, prefer DIY please use the hex editor to modify their datachage.dll
fileIP 400 at (EditDlg = <0 or 1>, LineCount = 