# Discord-IG-Virus-Decoded
The popular virus that hijack your social media and sending weird fucking images to people

## Back Story:-
We all know there is a virus that keeps using other people accounts to send fuck images everywhere, all the discord servers, users etc etc.
I had my GF PC having the virus and now I'm here to expose the virus.
!! Do not execute any py file in this repo as you'll get infected ！！

### Logic
The virus is having few steps to get through and bypassing AVs:-
1. While you downloaded any cracks or whatever, it will have a python.exe copied over with some pyd files, the main virus is in node_modules.asar which actually is a python script.
2. By faking the extension, python will executed normally, the code itself is having few layers of base85 and base64 encoded. The injection code is exposed in injection.txt in this repo
3. It executes OPCodes to inject itself into ntdll to bypass any AV that might caught it. OPCodes are in the injection.txt.

### What it does:-
Credential Theft: Injected code in explorer.exe can monitor keystrokes or access browser data to steal passwords.
Persistence: It may attempt to write itself to other common startup locations or system processes to ensure it survives a reboot even if the original Python files are removed.
External Command & Control: Many stagers of this type are designed to reach out to a remote server to download additional malware, which could potentially spread across your local network.

To kill this shit:-
Just do a full reinstall of Windows, this would be the most secure way.
