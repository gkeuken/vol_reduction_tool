# vol_reduction_tool
Sample code for z/OS Volume Reduction Tool

1. Download feucvoli in binary (sftp) to z/OS Unix System Services and ensure it's executable
2. Download zdt.dump.trs in binary to z/OS sequential, ensure RECFM=FB,LRECL=1024
3. Execute the restore JCL after updating statements having "??????" as necessary
4. Execute feucvoli without any parameters for Help.
