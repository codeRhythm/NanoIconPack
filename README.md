# NanoIconPack 图标包APP模板

![Developing](https://img.shields.io/badge/Developing-v3.0.0-green.svg)
[![Release](https://img.shields.io/badge/Release-v2.1.0-brightgreen.svg)](https://github.com/by-syk/NanoIconPack/releases/tag/2.1.0)
[![Download](https://img.shields.io/badge/Download-Sample%20APP-brightgreen.svg)](https://github.com/by-syk/NanoIconPack/raw/master/out/com.by_syk.nanoiconpack.sample_v3.0.0.7.nightly(17060600).apk)
[![License](https://img.shields.io/badge/License-Apache%202.0-yellowgreen.svg)](https://github.com/by-syk/NanoIconPack/blob/master/LICENSE)

![NanoIconPack](art/ic_launcher_nanoiconpack.png)


NanoIconPack 是一个简单轻量的图标包APP模板，支持主流启动器，**支持图标申请及统计**，并提供一些辅助功能。

您可以基于此进行二次开发，只需要装配图标、修改少量文件（不涉及Java代码）即可打包出自己的图标包。


### 下文目录

+ [支持启动器](#支持启动器)
+ [辅助功能](#辅助功能)
+ [服务器支持](#服务器支持)
+ [二次开发](#二次开发)
+ [更新日志](#更新日志)

其他：
+ [基于 NanoIconPack 的 APP](#基于-nanoiconpack-的-app)
+ [致谢](#致谢)
+ [更好的图标包模板推荐](#更好的图标包模板推荐)
+ [联系开发者](#联系开发者)
+ [License](#license)


### 支持启动器

目前核心支持以下3个元老级的启动器：

| Launcher | ICON |
| :---- | :----: |
| Nova Launcher | [![Nova](art/ic_launcher_nova.png)](http://www.coolapk.com/apk/com.teslacoilsw.launcher) |
| Apex Launcher | [![Apex](art/ic_launcher_apex.png)](http://www.coolapk.com/apk/com.anddoes.launcher) |
| ADW Launcher | [![ADW](art/ic_launcher_adw.png)](http://www.coolapk.com/apk/org.adw.launcher) |

这三个应该是启动器界的元老了（未考究），很多后来启动器沿用或支持它们的图标包规范。

NanoIconPack 同时还支持许多未列出的启动器，比如
+ Smart Launcher Pro
+ Action 3
+ Aviate
+ Holo Launcher
+ Arrow桌面
+ S桌面
+ Hola桌面
+ Go桌面
+ 冷桌面
+ 等……

以及一些系统默认启动器，比如
+ Xperia Home Launcher
+ 氢桌面
+ 等……

> 已知不支持并不打算支持：
> + ~~TSF桌面~~
> + ~~Atom桌面~~


### 辅助功能

除了图标包最基本的功能外，我们还为 NanoIconPack 开发了一些有用的辅助功能。以下列举一二，更多请下载 Sample APP 体验。

+ 主界面三大页
  
  ![NanoIconPack](art/show1.png)

+ 图标查看
  
  ![NanoIconPack](art/show2.png)
  
+ 「更新了啥」页面展示新图标

  ![NanoIconPack](art/show6.png)
  
+ 图标申请适配统计

  ![NanoIconPack](art/show4.png)
  
  > 该界面默认不可见，进入方法：双击主界面底栏的 **未适配** 图标

+ 版权描述

  ![NanoIconPack](art/show5.png)
    
+ 支持启动器的手动替换图标

  ![NanoIconPack](art/show3.png)


### 服务器支持

NanoIconPack 拥有一个轻量的服务器，提供图标申请和申请统计两大服务。

详情请移步 [NanoIconPack 服务端项目](https://github.com/by-syk/NanoIconPackServer)了解。


### 二次开发

请移步 [:book: Wiki 页面](https://github.com/by-syk/NanoIconPack/wiki)查看二次开发步骤和相关开发帮助。


### 更新日志

当前开发中的版本日志：

```
- 「申请统计」页面「显示未标记」时隐藏「TOP」菜单项
- 增加一个主页切换效果供选择，但调整默认为无效果
- 修复不识别大写字母支付宝转账链接的问题
- 不再重复保存图标
- 修复APP列表中非方形APP图标显示变形的问题（fitXY -> fitCenter）
- 移除APP列表中最后一条多余的分割线
- 「申请统计」从统计最小单元 pkg 变更到 pkg + launcher，更便于查漏补缺（服务端增加新接口来支持，同时原接口仍可正常使用；但标记数据不共通，也就是说更新到该版本后图标包作者需要重新标记）
- 「申请统计」支持提醒标记（小绿点）、提醒补缺（小红点）
- 在关于界面添加申请统计入口和APP代码速查入口
- 申请图标操作提示（使用了 MaterialTapTargetPrompt 库）
- Glide 加载图标列表，缓解速滑卡顿
- 整合网页，推出微控制台，提供服务：APP代码速查、常用APP代码、图标包统计、申请管理等。http://nano.by-syk.com
- 申请统计 Activity 独立展示在「最近任务」中
- 增加 enable_req_stats_module 配置变量用于启用/停用申请统计模块
- 图标对话框标题对多适配图标的区分形式由小黑点改进为标签（备用「ALT」、无适配「UND」）
- 「申请统计」底部显示标记点说明文字
- 支持发送图标到桌面（快捷方式）（感谢 @pandecheng 的创造性建议）
- 图标列表的图标不再支持隐晦的长按菜单，而是在图标展示对话框底部显示操作菜单
- 近乎重构核心代码，利用缓存加快各界面加载速度
- 加载动画（使用了 AVLoadingIndicatorView 库）
```

历史版本日志请移步[此处查看](out/changelog.txt)


### 基于 NanoIconPack 的 APP

| APP | ICON |
| :---- | :----: |
| [@atony](http://www.coolapk.com/u/474222) / [OriginalWish图标包 <sub>new version</sub>](http://www.coolapk.com/apk/com.atony.iconpack.originalwish) | ![OriginalWish](art/ic_launcher_original_wish.png) |
| [@pandecheng](http://www.coolapk.com/u/531994) / [PDC图标包 <sub>new version</sub>](http://www.coolapk.com/apk/com.pandecheng.iconpack) | ![PDC](art/ic_launcher_pdc.png) |
| [@大神sjk](http://www.coolapk.com/u/458995) / [Smalite图标包](http://www.coolapk.com/apk/com.sjk.smaliteiconpack) | ![Smalite](art/ic_launcher_smalite.png) |
| [@可以and不行](http://www.coolapk.com/u/444646) / [Pelmix图标包](http://www.coolapk.com/apk/com.edward.iconpack.pelmix) | ![Pelmix](art/ic_launcher_pelmix.png) |
| [@派大鑫](http://www.coolapk.com/u/511319) / [Party Star](http://www.coolapk.com/apk/com.paidax.iconpack.partystar) | ![Party Star](art/ic_launcher_party_star.png) |
| [@CookDev](http://www.coolapk.com/u/315615) / [Cardicons Ⅱ 图标包 <sub>new version</sub>](http://www.coolapk.com/apk/cookdev.iconpack.ii) | ![Cardicons](art/ic_launcher_cardicons.png) |
| [@Markuss](http://www.coolapk.com/u/529718) / [Aeroblast图标包](http://www.coolapk.com/apk/com.markusslugia.iconpack.aeroblast) | ![Aeroblast](art/ic_launcher_aeroblast.png) |
| [@tsengyong](http://www.coolapk.com/u/931477) / [NoShadow图标包](http://www.coolapk.com/apk/com.tseng.iconpack.design) | ![NoShadow](art/ic_launcher_no_shadow.png) |
| [@ClydeSHenry](http://www.coolapk.com/u/609006) / [Galet IconPack](http://www.coolapk.com/apk/com.clydeshenry.iconpack.galet) | ![Galet](art/ic_launcher_galet.png) |
| [@sftmi](http://www.coolapk.com/u/491391) / [OMFG图标包](http://www.coolapk.com/apk/com.sftmi.iconpack.omfg) | ![OMFG](art/ic_launcher_omfg.png) |
| [@梁月丶](http://www.coolapk.com/u/620760) / [HHope](http://www.coolapk.com/apk/com.hhope.iconpack.ken) | ![HHope](art/ic_launcher_hhope.png) |
| [@LYCSKY497](http://www.coolapk.com/u/477979) / [LYCSKY图标包](http://www.coolapk.com/apk/com.lycsky.iconpack) | ![LYCSKY](art/ic_launcher_lycsky.png) |
| [@Laihz](http://www.coolapk.com/u/748141) / [迷之图标包](http://www.coolapk.com/apk/com.laihz.gradualiconpack.gamma) | ![Gamma](art/ic_launcher_gamma.png) |
| [@sftmi](http://www.coolapk.com/u/491391) / [Square图标包](http://www.coolapk.com/apk/com.sftmi.iconpack.square) | ![Square](art/ic_launcher_square.png) |
| [@gushixing](http://www.coolapk.com/u/991472) / [X-Flat图标包](http://www.coolapk.com/apk/com.wokee.xflat) | ![X-Flat](art/ic_launcher_xflat.png) |
| [@crazypig321](http://www.coolapk.com/u/940496) / [lineicons](http://www.coolapk.com/apk/com.crazypig321.lineicons2) | ![line](art/ic_launcher_line.png) |
| [@Trumeet](http://www.coolapk.com/u/543424) / [滑稽图标包 <sub>new version</sub>](http://www.coolapk.com/apk/kh.android.funnyiconpack) | ![Funny](art/ic_launcher_funny.png) |
| [@lmn011223](http://www.coolapk.com/u/515642) / [萤火虫图标包](http://www.coolapk.com/apk/com.lnm011223.iconpack.fireflies) | ![Fireflies](art/ic_launcher_fireflies.png) |

如果您基于 NanoIconPack 开发了自己的图标包作品并且愿意[告诉我](#联系开发者)，我将把它展示在这里。


### 致谢

致敬开源！NanoIconPack 使用了如下开源项目：
+ [Li Min / pinyin4j](https://sourceforge.net/projects/pinyin4j/) licensed under [GPLv2](https://www.gnu.org/licenses/old-licenses/gpl-2.0.html)
+ [fython / AlipayZeroSdk](https://github.com/fython/AlipayZeroSdk) licensed under [Apache-2.0](http://www.apache.org/licenses/LICENSE-2.0)
+ [kenglxn / QRGen](https://github.com/kenglxn/QRGen) licensed under [Apache-2.0](http://www.apache.org/licenses/LICENSE-2.0)
+ [square / retrofit](https://github.com/square/retrofit) licensed under [Apache-2.0](http://www.apache.org/licenses/LICENSE-2.0)
+ [bumptech / glide](https://github.com/bumptech/glide) licensed under [BSD, part MIT and Apache-2.0](https://github.com/bumptech/glide/blob/master/LICENSE)
+ [timusus / RecyclerView-FastScroll](https://github.com/timusus/RecyclerView-FastScroll) licensed under [Apache-2.0](http://www.apache.org/licenses/LICENSE-2.0)
+ [sjwall / MaterialTapTargetPrompt](https://github.com/sjwall/MaterialTapTargetPrompt) licensed under [Apache-2.0](http://www.apache.org/licenses/LICENSE-2.0)

NanoIconPack 参考了如下资料：
+ [teslacoil / Example_NovaTheme](https://github.com/teslacoil/Example_NovaTheme)
+ [[GUIDE] Apex Launcher Theme Tutorial](https://forum.xda-developers.com/showthread.php?t=1649891)
+ [IconShowcase](https://github.com/jahirfiquitiva/IconShowcase)
+ [酷安开源版](https://github.com/bjzhou/Coolapk)

感谢伴随 NanoIconPack 开发过程的一群小伙伴们，他们来自酷安，提出了很多建设性建议：
+ [@ArchieLiu](http://www.coolapk.com/u/801526)
+ [@atony](http://www.coolapk.com/u/474222)
+ [@Childish](http://www.coolapk.com/u/596651)
+ [@CookDev](http://www.coolapk.com/u/315615)
+ [@hk流星](http://www.coolapk.com/u/555883)
+ [@可以and不行](http://www.coolapk.com/u/444646)
+ [@Markuss](http://www.coolapk.com/u/529718)
+ [@pandecheng](http://www.coolapk.com/u/531994)
+ [@sftmi](http://www.coolapk.com/u/491391)
+ 等……


### 更好的图标包模板推荐

NanoIconPack 追求简单轻量，只支持图标，如果您有更多需求，比如还需要支持壁纸、字体，还需要支持更多启动器，还需要更漂亮的 UI 等，可以参考以下开源项目：

| Dashboard | ICON |
| :---- | :----: |
| [jahirfiquitiva / IconShowcase-Dashboard](https://github.com/jahirfiquitiva/IconShowcase-Dashboard) | ![IconShowcase](art/ic_launcher_iconshowcase.png) |
| [afollestad / polar-dashboard](https://github.com/afollestad/polar-dashboard) | ![Polar](art/ic_launcher_polar.png) |
| [danimahardhika / candybar-library](https://github.com/danimahardhika/candybar-library) | ![CandyBar](art/ic_launcher_candybar.png) |


### 联系开发者

+ E-mail: [By_syk@163.com](mailto:By_syk@163.com "By_syk")
+ 酷安主页：[@By_syk](http://www.coolapk.com/u/463675)


### License

    Copyright 2017 By_syk

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

       http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.


*Copyright &#169; 2017 By_syk. All rights reserved.*