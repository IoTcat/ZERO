# v0.1.0
 - Move [`YerongAI/Office-Tool`](https://github.com/YerongAI/Office-Tool) `v8.3.3.11` to `c:/tools/Office Tool`.
 - Using `YerongAI/Office-Tool` to install word, excel, ppt. (O365ProPlusRetail; Excel, PowerPoint, Word; en-us, zh-cn; 64 Bit; Current Channel).
 - Using `YerongAI/Office-Tool` to active the Office with `Office Mondo 2016 Volume`License` and `kms.yimian.xyz`.
 - Install [`Total Uninstall`](https://www.martau.com/uninstaller-download.php) `v7.2.1` into default position and with default config. Active with my key.
 - Install [`7-zip`](https://www.7-zip.org/download.html) `21.07` with default config.


# v0.0.0
 - Download Windows 10 US-EN x64 Version 21H2 ISO from [https://tb.rg-adguard.net/](https://tb.rg-adguard.net/).
 - Using vmware to create a new VM (cpu:2,2; RAM:4GB; Disk:60G) from the ISO.
 - The username is set as `zero`.
 - Update OS to the latest version.
 - The hostname is set as `ZERO`.
 - Move [`iotcat/kms`](https://github.com/IoTcat/kms) `v1.2` to `c:/tools/kms`.
 - Run `iotcat/kms` to active Windows OS.
 - Move [`Dism++`](https://github.com/Chuyu-Team/Dism-Multi-language) `v10.1.1002.1` to `c:/tools/dism++`

# General Procedures for Packaging
1. Update `log.md`.
2. Shutdown the VM and take a snapshot with Version info.
3. Start the VM and using `Dism++` to generate an image file, named `zero_vx.x.x.esd`.
4. Upload the image file to server with URL `http://eee.dog/zero@x.x.x`.
5. Redirect the URL `http://eee.dog/zero` to latest image's URL.
6. Commit and push the Git repo.
7. Publish a release on Github repo named `vx.x.x` with log details.