# v0.3.0
- Install [v2rayN 5.32](https://github.com/2dust/v2rayN/releases/tag/5.23) to %appdata%. 
- [ ] setting->V2rayN 设置 -> 开机自启动 - 解除win10UWP回环
- [ ] 全局热键设置->清除系统代理Ctrl+Alt+Shift+P, 自动配置系统代理Ctrl+Alt+P
- [ ] 路由设置->保留全局，添加FlyToWorld和BackToChina


- `TrafficMonitor_V1.83_x64_Lite`安装到%appdata%。
- [ ] close main window
- [ ] show taskbar window
- [ ] Setting -> Taskbar setting -> auto set the background color according to taskbar color -> Yes ; Auto adapted to Win10 theme -> Yes; display setting ->  add CPU and MEM; Show resource usage graph; show net speed graph; color -> bottom left second gray; 
- [ ] General setting -> Check for update -> No; auto run when windows start->Yes; Show notify icon->No
- remove news from taskbar

- `QuickLook-3.7.1`insall.
- `Snipaste-1.16.2-x64` install: Run on system startup; as administrator; use Hex value for color picker; hotkey: snip->Ctrl+Alt+A, Paste->Ctrl+Alt+Shift+A, others->none; check for update on startup->no

- install `vlc-3.0.17.4-win32`, set as win setting default video app
- scoop install git, git config --global credential.helper manager-core; 
- scoop install aria2
- scoop install python
- scoop cache rm *
- install `Wox-1.3.524`, hide wox on start; hide wox when focus is lost; auto update->No; python path->~/scoop/app/python/current; shell->replace win+R->No; theme-> Light; 
- install `Everything-1.4.1.1017.x64-Setup`, show search everything folder content; show tray icon->No; 
- install `DittoSetup_64bit_3_24_214_0`, show startup message->no; active ditto->Ctrl+Shift+V; test only paste->Ctrl+Alt+V; positions->Ctrl+Alt+Win+Num; Copy buffer->Ctrl+Alt+Win+(Shift)+C/V

# v0.2.0
 - Open `dism++` and select `System Optimizer`. Change the following settings:   
 - [ ] How Cortana is shown on the taskbar -> Hidden
 - [ ] Hide task view button -> Yes
 - [ ] Taskbar clock displays seconds -> Yes
 - [ ] Disable suggestions in start menu -> Yes
 - [ ] Disable search for associated application in Windows Store -> Yes
 - [ ] Disable Ads from Windows Store -> Yes
 - [ ] Disable automatical installition of recommended apps -> Yes
 - [ ] Disable Cortana -> Yes
 - [ ] Open File Explorer to this PC -> Yes
 - [ ] Show extentions to all file types -> Yes
 - [ ] Prevent adding the suffix shortcut when creating a shortcut -> Yes
 - [ ] Hide 3D Object, Desktop...... in computer -> Yes
 - [ ] Disable Autoplay -> Yes
 
 - Install MadobeFamily2015Winter Theme
 - Install 'iotcat/win-wallpaper' with totaluninstall.
 - Open setting, do the following changes:
 - [ ] Background -> Slideshow - Pcitures/Wallpapers - 10min
 - [ ] Colors -> Light -> purple
 - [ ] Start -> show more tile on start - show most used apps
 - [ ] Date&Time -> set timezone automatically
 - [ ] Language -> add a language 中文（中华人民共和国）- Microsoft Pinyin -> General -> Default Mode -> English
 - [ ] Privacy -> Location -> Location for this devices - on - allow app visit - Maps, weather
 - [ ] Easy of access -> mouse pointer -> Third
 - [ ] Easy of access -> Text cursor -> on
 - [ ] System -> Display -> Night light setting -> schedule sunset to sunrise
 - [ ] Language -> keyboard -> Override -> Chinese Pinyin
 - [ ] uninstall solitaire collection games..

 - Classify taskbar (file explorer, mail, edge) and windows sticker (photo, weather camera, app store).

# v0.1.0
 - Move [`YerongAI/Office-Tool`](https://github.com/YerongAI/Office-Tool) `v8.3.3.11` to `c:/tools/Office Tool`.
 - Using `YerongAI/Office-Tool` to install word, excel, ppt. (O365ProPlusRetail; Excel, PowerPoint, Word; en-us, zh-cn; 64 Bit; Current Channel).
 - Using `YerongAI/Office-Tool` to active the Office with `Office Mondo 2016 Volume`License` and `kms.yimian.xyz`.
 - Install [`Total Uninstall`](https://www.martau.com/uninstaller-download.php) `v7.2.1` into default position and with default config. Active with my key.
 - Install [`scoop`](https://scoop.sh) in powershell by exec `Set-ExecutionPolicy RemoteSigned -scope CurrentUser` and `iwr -useb get.scoop.sh | iex`
 - Install `7-zip` with scoop. Add `[HKEY_CURRENT_USER\SOFTWARE\Classes\Directory\shellex\DragDropHandlers\7-Zip]
@="{23170F69-40C1-278A-1000-000100020000}"` and `[HKEY_CURRENT_USER\SOFTWARE\Classes\Drive\shellex\DragDropHandlers\7-Zip]
@="{23170F69-40C1-278A-1000-000100020000}"`and Delete `"MenuIcons"=dword:00000001` to `scoop/apps/7zip/install-context.reg`. Run this file with `Total Uninstall`. (scoop hold)


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
