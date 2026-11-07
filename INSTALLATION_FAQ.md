# Windows Alpha installation FAQ
UNPUBLISHED ALPHA CANDIDATE — download pending.

**Does it need installation?** Extract the entire ZIP to a writable folder and
run AimCoach.exe. Do not run from the ZIP preview. No installer is included.

**Do I need Godot or Python?** No. Those are development tools; the accepted EXE
contains its runtime resources.

**How do I save?** After completing a practice, choose Save practice on Results.
This explicitly writes a JSON recording and CSV summary. Saved practices finds
and reopens recordings for read-only Replay; Saved files opens their folder.

**Where are sessions?** The default Windows location is
%APPDATA%\Godot\app_userdata\AimCoach\sessions. Keep copies of recordings you value.

**How do I free the mouse?** Esc stops a running practice and releases the pointer.
Settings & controls explains navigation and Replay controls.

**Does it need internet or upload my data?** Local practice requires no account
or network connection. The application does not automatically upload recordings.
Saving a file does not send it to a website. Only deliberately shared files leave
your control; website import acceptance is a separate check.

**Why might Windows show an unknown-publisher warning?** This candidate is unsigned.
No antivirus or reputation acceptance is promised. Check the file source and
published checksum, and ask the provider if uncertain. Do not disable security
software to install this Alpha.

**How can I check the ZIP?** In PowerShell, run:
~~~powershell
Get-FileHash -LiteralPath ".\AimCoach-Windows-x64-0.1.0-alpha.1-candidate.zip" -Algorithm SHA256
~~~
Compare the Hash field with cd32254a1346174f10d8397abb47e754583794f65bdc930b8aeb0408690a6b20.
A matching checksum confirms the file matches that published digest; it does
not establish publisher identity or prove absence of malware.
[Microsoft Get-FileHash documentation](https://learn.microsoft.com/en-us/powershell/module/microsoft.powershell.utility/get-filehash?view=powershell-7.5)

**Can every Windows PC run it?** No universal compatibility claim is made. Only
the specified Windows 11 Pro x64 acceptance host was verified. Other systems,
hardware and sustained performance remain unverified.

**Where can I report a problem?** Use this repository's Issues. Include the
candidate version, Windows version and reproducible steps. Do not post personal
JSON/CSV recordings, private information or unredacted screenshots.
