# NovelAI（AINovel Editor）· 产物发布面

这个仓**只放桌面端安装包与自动更新元数据**，不放源码、不放历史：

- Windows：`AINovelEditor-Setup-<版本>-x64.exe`、便携包、`latest.yml`、`*.blockmap`
- macOS：`AINovelEditor-<版本>.dmg`、`AINovelEditor-<版本>.zip`、`latest-mac.yml`、`*.blockmap`

`latest*.yml` 与 `*.blockmap` 由打包那一次产出（文件名与哈希出自同一次构建），
桌面端的自动更新读的就是它们，所以请把它们当作发布通路的一部分，不要手工改动或删掉。

源码不在这里。构建用的树是一个单 commit 镜像，Release 正文里会写明它对应源仓的哪一次 commit。

这里的 tag 由发布流水线自动创建（GitHub 的 Release 必须挂在一个指向**本仓内 commit** 的 ref 上，
所以本仓至少要有这一颗 commit）——不要手工删这些 tag，删掉之后下一次发布就无处可挂。
