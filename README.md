# vol_reduction_tool
Installing the sample code for z/OS Volume Reduction Tool


- Download feucvoli in binary (sftp) to z/OS Unix System Services and ensure it's executable
- Download zdt.dump.trs in binary to z/OS sequential, ensure RECFM=FB,LRECL=1024
- Copy and Execute the restore JCL after updating statements having "??????" as necessary
- Execute feucvoli without any parameters for Help.


Note you could do a git clone from z/OS to obtain the files directly into USS, however if doing so you will have to convert the restore JCL to ibm-1047. This can be done by running command: 
   - iconv -f iso8859-1 -t ibm-1047 restore > restore.jcl

Then pre-allocate mvs sequential file zdt.dump.trs (RECFM=FB,LRECL=1024,TRKS(2,2)) then from ispf run:
   - oget '/path/to/zdt.dump.trs' 'zdt.dump.trs' binary
