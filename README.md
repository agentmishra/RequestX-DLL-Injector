```
            ____                             __ _  __    ____        _           __            
           / __ \___  ____ ___  _____  _____/ /| |/ /   /  _/___    (_)__  _____/ /_____  _____
          / /_/ / _ \/ __ `/ / / / _ \/ ___/ __/   /    / // __ \  / / _ \/ ___/ __/ __ \/ ___/
         / _, _/  __/ /_/ / /_/ /  __(__  ) /_/   |   _/ // / / / / /  __/ /__/ /_/ /_/ / /    
        /_/ |_|\___/\__, /\__,_/\___/____/\__/_/|_|  /___/_/ /_/_/ /\___/\___/\__/\____/_/     
                      /_/                                     /___/
        
                                      DLL INJECTOR x64/x86
```

<div align="center">
  
![](https://img.shields.io/badge/license-MIT-green?style=plastic) ![](https://img.shields.io/badge/arch-x64%20%7C%20x86-d9654f?style=plastic) ![](https://img.shields.io/badge/config-Debug%20%7C%20Release-c0c0c0?style=plastic)

</div>


- DLL injector written in C# that injects a DLL into a running process.

## How does it work?

1. **Windows API:** The LoadLibraryA module is loaded from the Windows API (specifically from kernel32.dll). Then, the handle of the selected process is found using the OpenProcess method. This handle gives access to the memory of the selected process. Memory is also allocated for a specific DLL within the selected process and the name of the DLL is written to the selected process' memory using the WriteProcessMemory method.

2. **Descriptor Copy:** In this method, the target process is accessed using an existing descriptor. The handle is a representative of the target process and provides access to the target process's memory. When this handle is copied, the target process can be accessed directly.

3. **Kernel Module:** This method takes advantage of the kernel module. The kernel module runs in the kernel part of the operating system and has special privileges. This method provides deeper level and specialized access. This makes the game cheat harder to detect from the game.

## How do I use the Injector

- Download the project to your computer as zip
- Extract Project to Folder.
- Make Sure Visual Studio is Installed [Click here if not installed](https://visualstudio.microsoft.com/en/thank-you-downloading-visual-studio/?sku=Community&channel=Release&version=VS2022&source=VSLandingPage&passive=false&cid=2030)
- Open the solution file (.sln).
- Select **Build Solution** from the **Build** menu or press `Ctrl+Shift+B` to compile the project.
- When the build is complete, select **Start Without Debugging** from the **Debug** menu or press `Ctrl+F5` to run the project.

## Anti-Cheating Measures

The anti-cheat systems we support cover a wide range and provide compatibility with different gaming environments. Here is the list of anti-cheat systems we are compatible with:

- Vanguard
- Easy Anti Cheat
- BattlEye Anti Cheat
- FACEIT
- Valve Anti-Cheat
- PunkBuster
- NProtect GameGuard
- Ricochet

Being compatible with these various anti-cheat mechanisms emphasizes our commitment to delivering a solution that is seamlessly compatible with multiple gaming ecosystems.

## Preview
<div align="center">
  
![image](https://github.com/MuckPro/dll/assets/138373919/819a6915-f625-4dff-99b9-9ccc4a6b2733)

</div>

## Contribution

1. Fork this repo.
2. Leave a Star ⭐ on this Repo.

## Disclaimer

This software is intended for educational and research purposes only. Any legal liability that may arise from the use of the software lies entirely with the user. The developer cannot be held liable for any misuse of the software and is exempt from any civil or criminal consequences that may arise therefrom.
In its current iteration, the project assumes a semblance closer to that of a DLL injector than a full-fledged loader, yet it remains functional and offers rudimentary security features. Its utility extends to scenarios where the distribution of exceptionally high-priced cheats or the creation of an individualized solution are not a prerequisite.

## License

This project is licensed under the MIT. For more information, see the [License](LICENSE).