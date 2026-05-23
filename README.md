# Portable NSIS IDE and Zip2EXE - A full-blown NSIS IDE with context-sensitive help based on Scitilla (SciTE)

<img src="https://github.com/user-attachments/assets/5ee2b1be-3773-4f44-949e-0e1df933acd8"
  alt="IDE"
  width="882"
  height="648"
  style="display: block; margin: 0 auto" />

## NSIS zip2exe with uninstaller-support in order to quickly rollout config-packages (over software) that can be uninstalled.

This version will use a modified NSIS "Base.nsh"-header-script and utilizes an inline powershell-script, that will build an uninstaller section for NSIS in a reverse order from the provided ZIP-file during initiated NSIS Installer-Build by Zip2EXE. Zip2EXE was also modded with a german dialog, a new icon-set and a version-string in resource-structure.

For example, we're now able to rollout very quick an Autoconfig-Package over a Thunderbird-Installation, that only derives from a simple ZIP-file !!

The contend of the ZIP-file can be uninstalled later, without touching the original package-files :-) ...

<img src="https://github.com/user-attachments/assets/382a4c93-d587-4ace-bb05-f15859191de9"
  alt="IDE"
  width="542"
  height="467"
  style="display: block; margin: 0 auto" />

For backround-infos and customizing the installer see:

```
 "IDE\Contrib\zip2exe\Base.nsh"
```

and the text-block between:

```
; ###################################### My DEFINITIONS ### BEGIN ###
...
; ###################################### My DEFINITIONS ###  END  ###
```
Due to the installer-design, to install this stuff into an already installed target-path of another installer, the uninstaller WILL NOT REMOVE THE ROOT-PATH. If you want to do this, you may modify the NSIS-Base header-file: "IDE\Contrib\zip2exe\Base.nsh" above, but be aware that this behavior <b>is not the primary use-case for the application objective presented here</b>.
