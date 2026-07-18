# GitKraken-TW 是 gitkraken-chinese 非官方繁體中文分支
[簡體中文](https://github.com/yk47g/gitkraken-chinese)  



### 手動替換

從項目根目錄或 `./舊版本文件` 中找到與你當前 GitKraken 版本匹配的 `.json` 文件，將其重命名為 `strings.json`，並替換
GitKraken 安裝目錄下的 `strings.json` 文件。該文件的位置根據你的操作系統有所不同：

#### <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/5/5f/Windows_logo_-_2012.svg/1280px-Windows_logo_-_2012.svg.png" alt="Windows Icon" style="width: 18px; height: 18px;"> Windows （

`x.x.x` 表示 GitKraken 版本號）

- `%程序安裝目錄%\gitkraken\app-x.x.x\resources\app\src\strings.json`
- `%程序安裝目錄%\gitkraken\app-x.x.x\resources\app.asar.unpacked\src\strings.json`

#### <img src="https://cdn-icons-png.flaticon.com/512/2/2235.png" alt="macOS Icon" style="width: 18px; height: 18px;"> macOS

- `/Applications/GitKraken.app/Contents/Resources/app/src/strings.json`
- `/Applications/GitKraken.app/Contents/Resources/app.asar.unpacked/src/strings.json`

#### <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/3/35/Tux.svg/1280px-Tux.svg.png" alt="Linux Icon" style="width: 18px; height: 18px;"> Linux（不同安裝方式下路徑可能不同）

- （由[@lyydhy](https://github.com/lyydhy)補充）通過 `deb` 安裝（例如 Deepin 系統），路徑可能是：

  `/usr/share/gitkraken/resources/app.asar.unpacked/src/strings.json`
- 通過 `AUR` 安裝（例如 Arch Linux），路徑可能是：

  `/opt/gitkraken/resources/app.asar.unpacked/src/strings.json`

完成文件替換後，重啟 GitKraken 即可生效。




### 屏蔽更新（可選）
> 防止被更新洗掉  
> 需要注意的是，Windows平台自動更新後並不會自動卸載舊版軟件，而且這些無用的文件會佔用較大的磁盤空間（大概1~2G），最好手動删除，目錄是C:\Users\{用戶名}\AppData\Local\gitkraken\app-xxx
<!-- no toc --> 
**通用方案:**
```
0.0.0.0 release.gitkraken.com
```