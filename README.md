# MyTune

MyTune is a Windows tuning app for gaming. It turns on proven Windows, network and graphics settings that lower input lag and keep frame rates steady, and every change can be undone.

## What's new in 2.4.3

- **Resizable BAR check**: the PC check on Home now tells you if this graphics-card setting is off on an RTX 30, 40 or 50 card, and where to turn it on in the BIOS.

## Install

1. Download `MyTune-Setup-<version>.exe` from the [latest release](https://github.com/castielcx/MyTune/releases/latest).
2. Run it. Windows may show a "Windows protected your PC" notice because the setup is not code-signed. Click **More info**, then **Run anyway**.
3. On the last page of the setup you can tick two optional drivers:
   - **PawnIO** lets MyTune read your CPU temperature. It is ticked by default.
   - **ViGEmBus** is only needed for the controller features.
4. Start MyTune. It needs administrator rights, so Windows asks for permission each time.

Requires 64-bit Windows 10 or 11.

## First start

- The welcome window offers a set of recommended tweaks (Optimization and Debloat). Nothing marked Risky or Security risk is included.
- A Windows restore point is created before the first change.

## Tips

- **Restart after applying.** Tweaks marked Restart only take effect after Windows restarts. A bar at the top of MyTune lists what is still waiting.
- **Undo anything.** The Restore page reverts a tweak to the value it had before MyTune changed it. If MyTune has no saved original for a tweak, it changes nothing.
- **Games.** Add your games on the Game Hub page to give each one its own CPU core choice, NVIDIA profile, GPU choice and network priority.
- **Start with Windows.** This is off by default. You can turn it on in Settings, and MyTune then starts hidden in the tray without a permission prompt.
- **Risky tweaks.** Open "What does this change?" before turning on anything labelled Risky, Experimental or Security risk.
- **After a big Windows update.** When Windows moves to a new build, MyTune switches off its risky tweaks and keeps them off until you install a newer MyTune version.
- **Updates.** MyTune checks this page for new versions and shows a banner. Click **Update now** and it installs the new version and restarts itself.

## If something goes wrong

- **A tweak is greyed out.** The card says why, for example that your network driver does not offer that setting.
- **Windows will not start properly.** Boot into Safe Mode and run `MyTune-Rescue.bat`. MyTune keeps a copy on your Desktop and in `C:\ProgramData\MyTune`. It puts back the original values of everything MyTune changed. It does not work from the Windows recovery screen.
- **Asking for help.** In MyTune open **Settings** and press **Support file**. It saves `MyTune-support.txt` on your Desktop with your system details, network adapters and the end of the log. Send that file along with your question. The Windows user name is replaced, but log lines can still show program paths, so look through it first.
- **Log file.** `C:\ProgramData\MyTune\mytune.log`.

## Uninstall

Remove MyTune in Windows **Settings > Apps**. Tweaks stay applied after uninstalling. Revert them on the Restore page first if you want your original settings back.
