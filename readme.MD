# KIM-1 tipps

--
This is just a collection of tipps:

How to onefile Papertape files?

Imagine you have a prg to be loaded to different playes and the assembler produced several papertape files.
You can load them either one after the other or "onefile" them:

Copy all papertape sneppets (Without the ending checksum) to one file.
Use the command ["srec_cat" ][1] to recalculate the checksum.
You can also change some bytes in the code with the -ignore-checksum switch

 >  srec_cat.exe -ignore-checksum .\Baseball_papertape_test.pap -MOS_Technologies  -o .\bb_test1.pap -MOS_Technologies



[1] http://srecord.sourceforge.net/
