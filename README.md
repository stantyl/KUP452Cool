# KUP452Cool

Encrypted archive handoff: `KUPA_452.7z`

The archive is **AES-256 encrypted, including its file listing**. Without the
password you cannot open it, extract it, or even see what filenames are inside.
The password is not stored in this repository — ask me for it directly.

## Contents

Source for the CoolingOffEmailRunner .NET Framework 4.5.2 solution
(`CoolingOffEmailRunnerConsole` + `SendEmailAndText`), including git history.
Build output (`bin/`, `obj/`, `.vs/`) was excluded, so restore NuGet packages
and rebuild after extracting.

## How to extract

You need 7-Zip or a compatible tool. Windows Explorer's built-in "Extract All"
cannot open this archive.

**Windows** — install 7-Zip (free, <https://www.7-zip.org>), then either
right-click the file → *7-Zip* → *Extract Here* and enter the password, or:

    7z x KUPA_452.7z

**macOS** — `brew install p7zip`, then:

    7z x KUPA_452.7z

**Linux** — `apt install p7zip-full` (or your distro's equivalent), then:

    7z x KUPA_452.7z

7-Zip will prompt for the password before it shows you anything.

You should end up with a `NET452-Share/` folder containing the solution.
