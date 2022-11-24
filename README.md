# Simple RunPE Binder for .NET programs.  

![winx](https://user-images.githubusercontent.com/113988354/203790267-ef9f8236-4648-4fbf-84ce-209108bf56d0.PNG)  
  
The Victim is the file that injects into itself, the Payload is the trojan that injects to the process.
  
Notes:
  
    With RunPE, Admin privileges are not possible, same with adding to startup because it will just add what it injected to startup. (Not your payload itself)  
    Stub is in C# .net, the victim will inject into itself, so the victim cannot be in native, only .net. however if the payload is native then it can be injected into a native process like vbc.exe or cvtres.exe  
    If you run into an error while compiling, try downloading/enabling the .NET 3.5 Framework/Runtime, it should solve the error. If not, open an issue. 
    
  With custom inject you need to add the name of an executable within the .NET folder, here's a list of executables:  
  AppLaunch.exe  
  aspnet_compiler.exe  
  aspnet_regbrowsers.exe  
  aspnet_regiis.exe  
  aspnet_regsql.exe  
  aspnet_state.exe  
  aspnet_wp.exe  
  CasPol.exe  
  csc.exe  
  cvtres.exe  
  dfsvc.exe  
  dw20.exe  
  IEExec.exe  
  ilasm.exe  
  InstallUtil.exe  
  jsc.exe  
  MSBuild.exe  
  mscorsvw.exe  
  ngen.exe  
  RegAsm.exe  
  RegSvcs.exe  
  vbc.exe  
  
