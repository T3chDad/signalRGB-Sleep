# SignalRGB-Sleep
It would be so awesome if the SignalRGB team would add a "Turn off RGB when screen is off/idle" option.  

I'm impatient, so this is my attempt at a kludge to add this functionality via an open source windows utility. This is largely just an excersize to dust off my coding activities. I'm sharing this application in case anyone else would like to have this functionality to SignalRGB without too much trouble. No installation is needed. Just download the zip and extract it somewhere on your system that SignalRGB is installed on and create a shortcut for the `"signalRGB-Sleep.exe"` in the `%userprofile%\Microsoft\Windows\Start Menu\Programs\Startup` folder so it loads when Windows starts.

This app is essentially a proof of concept and should not be considered a production worthy release and likely has bugs. It was authored in VS2022 in C# under .NET Core 8.0. It functions as a GUI wrapper between the SignalRGB command line capability and detecting the different idle/lock state of the computer. When the program detects a lock or idle timeout, it uses the shell to tell SignalRGB to change to the desired "OFF" effect. When it detects a wake or unlock event, it tells SignalRGB to change to the desired "ON" effect...simple right?!

For Example:  
--The default "OFF" effect is "Solid Color" with the settings of Black and 0 brightness.  
--The default "ON" effect is "Screen Ambience". 

You can change the desired effects in the app settings (double-click tray/notification area icon). The effects you specify must already be installed and configured with SignalRGB itself. You need to ensure the effect names specified here must match the names in the SignalRGB interface. Spaces are supported.

![SignalRGB-Sleep_g3PxN62RAC](https://github.com/user-attachments/assets/8b7f993e-8d1c-4d18-8b4f-02db645692bb)

If you enjoy this project or I have helped you...feel free to [buy me a coffee](https://www.buymeacoffee.com/hVmOfsXjX1).
************************************************************************************************
Use this program at your own risk. I'm not responsible for anything that happens on your system.
************************************************************************************************

