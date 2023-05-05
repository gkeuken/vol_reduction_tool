# vol_reduction_tool
Installing the sample code for z/OS Volume Reduction Tool


- Download feucvoli in binary (sftp) to z/OS Unix System Services and ensure it's executable
- Download zdt.dump.trs in binary to z/OS sequential, ensure RECFM=FB,LRECL=1024
- Copy and Execute the restore JCL after updating statements having "??????" as necessary
- Execute feucvoli without any parameters for Help.
