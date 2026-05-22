# Portable NSIS IDE and Zip2EXE - A full-blown NSIS IDE with context-sensitive help based on Scitilla (SciTE)

<div style="text-align: center">
  <img width="882" height="648" alt="IDE" src="https://github.com/user-attachments/assets/5ee2b1be-3773-4f44-949e-0e1df933acd8" />
</div>

## NSIS zip2exe with uninstaller-support in order to quickly rollout config-packages (over software) that can be uninstalled.

This version will use a modified NSIS "Base.nsh"-header-script and utilizes an inline powershell-script, that will build an uninstaller section for NSIS in a reverse order from the provided ZIP-file during initiated NSIS Installer-Build by Zip2EXE. Zip2EXE was also modded with a german dialog, a new icon-set and a version-string in resource-structure.

For example, we're now able to rollout very quick an Autoconfig-Package over a Thunderbird-Installation, that only derives from a simple ZIP-file !!

The contend of the ZIP-file can be uninstalled later, without touching the original package-files :-) ...

<div style="text-align: center">
  <img width="542" height="467" alt="NSIS-3.12 Zip2EXE Deutsch" src="https://github.com/user-attachments/assets/382a4c93-d587-4ace-bb05-f15859191de9" />
</div>
