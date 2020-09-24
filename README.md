# AdmPwd project

This is a fork of the AdmPwd project (specifically the UI portion) which supports multi-domain environments by inheriting the domain from the user running the process rather than the logged on user. This allows you to view passwords from other domains even while signed into the PC under a user from a different domain. For example, if you were signed into the PC as `CONTOSO\Eric` and wanted to view passwords from the `ACME` domain, you could run `runas /user:ACME\Eric AdmPwd.UI.exe` to do so. This is not possible with the original project.

**Original README:**

This is source code for AdmPwd project that has been previously hosted on MSDN gallery - project has been used as base for Microsoft branded LAPS solution.

Enhancements over Microsoft LAPS:
* usage of CNG instead of CryptoAPI for crypto operations
* password management on ARM64 machines
* installer supported on pure 64-bit Windows without WoW64
* Support for automatic password change of managed local admin account on fresh install on new machine that reuses computer account of machine where password was previously managed

Moved to github so as make it easier to allow cooperation, contribution and development of the solution. For details on current functionality, see release note for releases.

Feel free to fork and bring updates

--Jiri
