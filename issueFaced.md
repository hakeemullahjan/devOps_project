Steps:
Create Azure account
Clone and run Project 
Create VM 
connect using SSH

issues faced:
creating and choosing zones based on rate was issue 
then connecting using ssh from cmd as chmod has to be changed so i used there commands to fix that issue:
icacls .\obaidVM_key.pem /inheritance:r
 
icacls .\obaidVM_key.pem /grant:r "$($env:USERNAME):(R)"
 
ssh -i .\obaidVM_key.pem azureuser@20.240.217.21
 
