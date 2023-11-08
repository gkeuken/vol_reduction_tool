# vol_reduction_tool
Installing the sample code for z/OS Volume Reduction Tool


- Transfer feucvoli in binary (sftp) to z/OS Unix System Services and ensure it's executable
- Upload zdt.load.xmit in binary to z/OS sequential data set, ensure RECFM=FB,LRECL=80
- Receive inds(zdt.load.xmit) 
- execute feucvoli without any parameters for help information

Note you could do a git clone from z/OS to obtain the files directly into USS, then send zdt.load.xmit from USS to an MVS Sequential (Fixed Block 80) and perform RECEIVE INDS('ZDT.LOAD.XMIT') 
