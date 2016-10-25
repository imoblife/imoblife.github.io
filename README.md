**All-In-One-Toolbox**

GooglePlay: https://play.google.com/store/apps/details?id=imoblife.toolbox.full
Background: http://naotu.baidu.com/file/484dfc7d182509c049491858c20ef87b?token=d7bc58785b6f68ef

===================================================================================================
**功能模块**

*	base 基础类
    * base_titlebar标题栏
	* base_statusbar状态栏
	* base_toolbar工具栏

*	splash 欢迎界面
    * Admob预加载 （AdHelper.getInstance(ASplash.this);）
    * 定时提醒检查 （NotifierRemind.getInstance(this).check();）
    * 桌面快捷方式检查 （ShortcutUtil.checkShortcut(getApplicationContext());）
    * 通知栏检查 （Notifier.getInstance(getApplicationContext()).checkNotifier();）
    * 初始化白名单检查 （WhitelistHelper.getInstance(getApplicationContext()).check();）
    * LuckAd预加载 （LuckAdNew.get(getContext(), this).checkAd();）
    * 强制清除友盟配置 （clearUmeng();）
    * 扫描结果重置 （ScanManage.getInstance(this).reset();）
    * 友盟后台统计检查 （countManager.checkUpdateAlartRotation();）

*	main 主界面

*	clean 清理模块
	* cache 缓存
	* leftover 卸载残留
	    filepath.db中存在路径记录，类型为0会清理时会自动打勾，卸载时会有清理弹窗提醒；类型大于0，勾选时警告，卸载时无清理弹窗。
	* apk 安装包清理
	* trash 存储卡清理
		* temp 临时文件
		* thumb 缩略图
	* recycle 回收站
	    * 大于1MB的图片文件

*	privacy 隐私
	* history历史
	    * clipboard 剪切板
	    * browser 浏览器历史记录
	    * Gmail搜索记录
	    * GoogleEarth搜索记录
	    * Google Maps搜索记录
	* StorageAnalysis 磁盘分析
	* cmct通信清理
		* call通话
		* sms短信
    * Chrome
    * Youtube
    * QuickSearch
    * Downloads
    * Wifi
    * 预置列表中数据大于零的应用
        * com.alibaba.android.babylon
        * com.alibaba.mobileim
        * com.facebook.orca
        * com.facebook.katana
        * com.google.android.apps.plus
        * com.igg.android.im
        * com.immomo.momo
        * com.linkedin.android
        * com.snapchat.android
        * com.skype.raider
        * com.tencent.mm
        * com.tencent.mobileqq
        * com.twitter.android
        * com.whatsapp
        * jp.naver.line.android
        * kik.android
        * org.buffer.android
        * com.opera.mini.android
        * com.opera.browser

*	boost 加速模块
	* process进程
	* startup启动项

*   boost+ 超级加速
    * 支持4.4及以上系统

*   cooling 冷却机制
    * boost & boost+
          * 完整扫描，完整查杀则冷却
          * 超过五分钟则不冷却
          * 未扫描完全则不冷却
          * 未全选查杀则不冷却
          * 由主界面退出则不冷却
          * 由欢迎界面进入则不冷却

*	QuickBoost 快速优化
	* process目前只包括进程清理

*	toolbox 工具箱
	* install安装
	* uninstall卸载
	* slimming系统精简
		* slimming_bin回收站
	* bakrst备份还原
		* backup备份
		* restore还原
	* app2sd
	* file文件管理
	* startup_add启动项添加
	* plugin插件

*	prokey 专业版

*	info 系统信息

*	setting 设置界面

*	whitelist 进程白名单

*	ignorelist 清理白名单

*	feedback 反馈

*	share 分享弹窗

*	rate 评论弹窗

*	about 关于

*	notifier 通知栏
	* 每10分钟刷新一次，解锁时立即刷新

*	widget 小部件
	* widget_custom自定义小部件
	* widget_expand扩展页面

*	shortcut 快捷方式
	* shortcut_boost加速动画页面

*	schedule 定时检测

*	track 数据跟踪
	* GoogleAnalytics谷歌分析
	* UmengCount友盟统计

*	LauncheMessage 推送消息

*	CPU Cooler

	* 1 开启CPU监测

	* 2.1 电池温度小于43

	* 2.1.1 一天监测两次

	* 2.2 电池温度大于43

	* 2.2.1 每分钟检测一次

	* 3 某个进程CPU占用率超过40%

	* 4 某个进程电池使用量大于1%

	* 5 非当前运行进程

	* 6 提示CPU占用过高

*	RateDialog 评论弹窗
	* http://naotu.baidu.com/file/0d0e678983395dd6ed8cc7957db3ccb8?token=4d98ecc27c61b475

*	DrawMachine 抽奖机 (5.2.1.1 Only)
	* 日期
	* 未参与（偏好+文件/Toolbox/.drawed）
	* 预设概率
	* 服务器奖品数量充足（remians>1）
	* 抽中奖品

*  Immerse 沉浸模式
    * 支持Android 4.4及以上(sdk>=19)

*	Drawable（保留资源，请勿删除以下模块图片）

	* tools_install.png
	* tools_uninstall.png
	* tools_backuprestore.png
	* system_lose.png
	* tools_tranfer.png
	* tools_startupmanager.png
	* tools_startupadd.png
	* tools_file.png

*	NativeAd 广告页面

*	InterstitialAd 全屏广告
	* 说明：未安装谷歌市场(com.android.vending, market.android.com)，点击礼物盒子打开全屏广告。
	* 时机：1.点击礼物盒子时才加载。
	* 位置：Main、Clean、Boost标题栏礼物盒子图标。
	* 用户：未安装Google Play的用户。
	* 机制：

*	FacebookAd
	* 说明：Clean、Boost结果页面列表嵌入广告条目。
	* 时机：1.首次出现结果页面时加载一次。2.解锁屏幕後广告被置空，再次显示结果页时重新加载一次。 3.点击广告后后台加载一条新广告 4.退出主程序根据频率更新陈旧广告
	* 位置：Clean、Boost结果页面。
	* 用户：所有用户（MotoX，S5测试与是否安装Facebook或是否登陆Facebook无关）
	* 机制：
		*	1.广告缓存在AIO系统缓存中，AIO系统缓存清除后图片需要重新加载。
		*	2.每次加载一条广告


*	LuckAd 原生广告（目前计划尝试使用42，然后调优更新广告时间）

	* 实现机制I：   YeahMobi的SDK调用，请求15个广告，点击礼物盒子显示广告，依次循环显示。
	* 实现机制II：  Yeahmobi的API机制，每次加载5个，并在后台提前转换5个GP链接
	* 实现机制III： Glispa的API机制，每次加载5个广告，并在后台提前转换5个GP链接
	* 实现机制IV：  Yeahmobi的API和Glispa的API合并机制，实现机制II和机制III
	* 实现机制V：   Yeahmobi的API和Glispa的API混合机制，每次进入程序，两者交替调用，但不同时出现。
	* 实现机制VI：  Glispa的API机制，每次只加载5个广告，但只在后台提前转换1个GP链接，剩余的在每次点击礼物盒子的时候加载，点击一下加载下一个。
	* 实现机制VII： Glispa的API机制，每次只加载5个广告，但只在后台不提前转换任何GP链接，点击才加载。
	* 实现机制VIII：Glispa的API机制，每次加载5个广告，首次进入或者进入广告列表为空时，在后台提前转换5个GP链接。以后在进入程序，根据时间限制，重新加载5个新广告，但只在后台提前转换1个GP链接。用户点击礼物盒子时，加载下一个GP链接。
	* 实现机制IX：与机制VII相似，但引入缓存机制，减少不必要的重复加载。


	* type=1-->实现机制I

	* type=2-->实现机制IV，每8小时更新一次广告列表
	* type=12-->实现机制IV，每12小时更新一次广告列表
	* type=22-->实现机制IV，每24小时更新一次广告列表

	* type=3-->换量
	* type=4-->ironsource(!禁用，否则会大量报错)
	* type=5-->ironsource和ym混合(!禁用，否则会大量报错)
	* type=6-->换量和实现机制I混合

	* type=7-->实现机制II，每8小时更新一次广告列表
	* type=17-->实现机制II，每12小时更新一次广告列表
	* type=27-->实现机制II，每24小时更新一次广告列表

	* type=8-->实现机制III，每24小时更新一次广告列表
	* type=18-->实现机制III，每24小时更新一次广告列表
	* type=28-->实现机制III，每24小时更新一次广告列表

	* type=9-->ym的shuffle方式（弃用）
	* type=10-->实现机制V
	* type=11-->Glispa旧API方式（弃用）

	* type=20-->实现机制VI
	* type=30-->实现机制VII

	* type=31-->实现机制VIII，每次加载10个广告，每2小时更新一次广告列表
	* type=32-->实现机制VIII，每次加载10个广告，每4小时更新一次广告列表
	* type=33-->实现机制VIII，每次加载10个广告，每6小时更新一次广告列表
	* type=34-->实现机制VIII，每次加载10个广告，每8小时更新一次广告列表
	* type=35-->实现机制VIII，每1小时更新一次广告列表
	* type=36-->实现机制VIII，每2小时更新一次广告列表
	* type=37-->实现机制VIII，每4小时更新一次广告列表
	* type=38-->实现机制VIII，每6小时更新一次广告列表
	* type=39-->实现机制VIII，每8小时更新一次广告列表
	* type=40-->实现机制VIII，每10小时更新一次广告列表

	* type=41-->实现机制IX，每4小时更新一次广告列表
	* type=42-->实现机制IX，每6小时更新一次广告列表
	* type=43-->实现机制IX，每8小时更新一次广告列表
	* type=44-->实现机制IX，每10小时更新一次广告列表
	* type=45-->实现机制IX，每12小时更新一次广告列表


*	GoogleAnalytics(4.0)
    * 欢迎界面100%统计
    * 其他界面关联设置中的‘软件改进’，勾选则统计，否则不统计。


===================================================================================================
代码规范补充：
===================================================================================================

* 自定义方法不要和系统方法同名
* ModernAsyncTask主要用作主功能，AsyncTaskEx主要用作网络操作
* 建议把颜色等资源复制到别的库后， 加一个前缀。  现在资源有些id对应多个res文件
* 新加代码尽量置于原有代码之后
* 防御式编程，过滤掉空指针等错误。对没有把握的功能，可以try catch暂时加以保护
* 提高代码可读性，提交可读性。尽量每个任务相关文件整理为单词提交，便于review。
* 新模块统一定一个内部模块名



===================================================================================================
谷歌分析对应页面统计名称
===================================================================================================

模块名	GA名字
欢迎界面	v6_splash
主页	v6_homepage
普通清理界面	v6_clean
高级清理	v6_advanced_clean
清理设置界面	v6_clean_settings
清理白名单	v6_clean_whitelist
清理还原中心	v6_clean_restore_center
清理结果界面	v6_clean_result
占用分析	v6_storage_analysis
加速界面	v6_boost
超级加速	v6_boost_plus
加速白名单	v6_boost_whitelist
加速结果界面	v6_boost_result
插件list view	v6_plugins_list
插件grid	v6_plugins_grid
工具界面-list view	v6_tools_list
工具界面-grid	v6_tools_grid
CPU降温	v6_cpu_cooler
批量安装	v6_install
批量卸载	v6_uninstall
备份	v6_backup
还原	v6_restore
系统应用卸载	v6_preinstalled_app
系统应用卸载还原中心	v6_preinstalled_restore
软件搬家手机界面	v6_app2sd_phone
软件搬家SD卡界面	v6_app2sd_sd
开机加速用户应用	v6_boot_speedup_user
开机加速系统应用	v6_boot_speedup_system
添加启动项主界面	v6_add_startup_main
添加启动项用户应用界面	v6_add_startup_user
添加启动项系统应用界面	v6_add_startup_system
文件管理器	v6_file_manager
文件管理器-多选	v6_file_manager_multiselect
备份弹窗	v6_backup_window
设置界面	v6_settings
暗色通知栏	v6_custom_notification_dark
亮色通知栏	v6_custom_notification_light
自定义通知栏	v6_custom_notification
卸载残留提醒	v6_leftover_dialogue
1X1小部件	v6_1x1_widget
4x1小部件自定义界面	v6_4x1_widget_custom
快捷方式选择界面	v6_pick_shortcut
clean快捷方式	v6_clean_shortcut
boost快捷方式	v6_boost_shortcut
通知栏ram	v6_notificationbar_ram
系统信息	v6_system_info
自定义主页	v6_diy_homepage
关于	v6_about
关于（用户手册）	v6_about_user_manual
关于（FAQ）	v6_about_faq
关于（权限）	v6_about_permission
关于（翻译）	v6_about_translator


===================================================================================================
//android.os.Build.java
1   BASE	                    October 2008: The original, first, version of Android.
2   BASE_1_1	                February 2009: First Android update, officially called 1.1.
3   CUPCAKE	                    May 2009: Android 1.5.
5   DONUT	                    September 2009: Android 1.6. / ECLAIR	November 2009: Android 2.0
6   ECLAIR_0_1	                December 2009: Android 2.0.1
7   ECLAIR_MR1	                January 2010: Android 2.1
8   FROYO	                    June 2010: Android 2.2
9   GINGERBREAD	                November 2010: Android 2.3
10  GINGERBREAD_MR1	            February 2011: Android 2.3.3.
11  HONEYCOMB	                February 2011: Android 3.0.
12  HONEYCOMB_MR1	            May 2011: Android 3.1.
13  HONEYCOMB_MR2	            June 2011: Android 3.2.
14  ICE_CREAM_SANDWICH	        October 2011: Android 4.0.
15  ICE_CREAM_SANDWICH_MR1	    December 2011: Android 4.0.3.
16  JELLY_BEAN	                Android 4.1.
17  JELLY_BEAN_MR1              November 2012: Android 4.2, Moar jelly beans!
18  JELLY_BEAN_MR2              July 2013: Android 4.3, the revenge of the beans.
19  KITKAT                      October 2013: Android 4.4, KitKat, another tasty treat.
20  KITKAT_WATCH                Android 4.4W: KitKat for watches, snacks on the run.
21  L                           Temporary until we completely switch to {@link #LOLLIPOP}.
21  LOLLIPOP                    Lollipop.  A flat one with beautiful shadows.  But still tasty.
22  LOLLIPOP_MR1                Lollipop with an extra sugar coating on the outside!
23  M                           M comes after L.(Nexus 5)
24  N                           N (Nexus 6)



===================================================================================================
*   IconFont

*   FontCreator打开ttf文件，右键新建，粘贴图标
*   右键属性，修改映射值为上一图标的映射值+1
*   Toolbox.java文件中Icon类中新增一条枚举：AIO_ICON_NAME('\uE907')
*   Xml中，引用IconicsTextView,IconicsImageView,IconicsButton等组件（推荐使用IconicsTextView，兼容性好，占用内存小），
    其中IconicsTextView的text属性指定"{AIO_ICON_NAME}"，IconicsImageView的iiv_icon属性指定图标 AIO_ICON_NAME，iiv_color指定颜色。
*   代码中，IconFontDrawable drawable = new IconFontDrawable(context)
                                        .icon(Toolbox.Icon.AIO_ICON_NAME)
                                        .colorRes(colorRes)
                                        .contentRatio(1 / 1.7f)
                                        .sizeDp(40);


===================================================================================================
插件确认自身是否为注册版流程

0.AIO:ProkeyHelper.java:

        //Prokey设置项和广播定义
        public static final String PROKEY_PREFERENCE_KEY =  "isPro";
        public static final String PLUGIN_ACTION_PROKEY_QUERY =  "com.pro.provider";
        public static final String PLUGIN_ACTION_PROKEY_RESULT =  "com.pro.provider.result";

1.Applock:Splash.java:

        //若插件非PRO版本，则发送广播询问AIO状态
        public void checkPro() {
            if (!PreferenceHelper.isPro(this)) {
                sendBroadcast(new Intent(PLUGIN_ACTION_PROKEY_QUERY));
            }
        }

2.AIO:CommandReceiver.java:

        //若AIO为PRO版本，则发送广播通知所有插件
        else if (action.equals(PLUGIN_ACTION_PROKEY_QUERY)) {
            if (PreferenceHelper.isPro(context)) {
                Intent i = new Intent(PLUGIN_ACTION_PROKEY_RESULT);
                context.sendBroadcast(i);
            }
        }

3.Applock:KeepAliveReceiver.java:

        //若插件确认AIO为PRO版，则将自身注册为PRO版。
        if (action.equals(PLUGIN_ACTION_PROKEY_RESULT)) {
			PreferenceHelper.setBoolean(context, PROKEY_PREFERENCE_KEY, true);
		}

