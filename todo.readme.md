APP框架搭建：
1、环境切换、接口配置、状态管理
2、谷歌统计
3、多语言支持
4、logo、slogan图片处理
5、gogle登陆接入、telegram登陆接入、facebook登陆接入
6、

我继续把 iOS 的 Firebase SDK 真正接进工程，并在启动时加入 FirebaseApp.configure
我继续把 Android 页面按你给的 HTML 视觉做更高保真还原
我继续把 iOS 页面按同一套 HTML 参考做更细的视觉还原和交互补全

1、生成constant文件，存储常用变量，比如：官网地址，用户协议地址、隐私协议地址、会员协议地址等，APP主题色是#ff6d08
2、添加环境支持：开发环境、测试环境、生产环境
3、增加多语言支持：中文、英语、高棉语（柬埔寨）（默认英文）
4、app页面如下：（强制要求登陆）
a、登录页面：
    - 右上角语言切换按钮
    - logo
    - slogan
    - facebook登陆
    - telegram登陆
    - google登陆
    - 底部是隐私政策链接，点击sheet/modal弹出打开隐私政策
b、求职意向页面：

c、tab页面：
    - 岗位列表tab
        右上角语言切换按钮
    - AI Bot tab
    - 我的tab
d、岗位详情
e、搜索页面

公共组件
1、语言切换按钮+sheet/modal弹窗
2、城市选择sheet/modal
3、岗位类型选择sheet/modal
4、岗位item（岗位列表用）

可以参考html进行还原

安卓使用Jetpack Navigation，ios使用liquid glass

接入谷歌分析

1、APP内部不要支持环境切换，我说的支持环境是支持开发、测试、生产环境的配置和打包，不是在app内部切换不同环境
2、

下个版本需求

ai求职助理、token的消耗、skills、


ios、安卓 app名称修改：生产环境就是dodojob,其他是dodojob+环境名称


1、登陆后应该全局状态管理，并且下次打开app应该已经是登陆状态
2、参考old-project实现，如果未登陆打开app后显示登陆，已登陆未选择求职意向Onboarding打开求职意向，已登陆，已选择求职意向显示tab页面


获取当前用户的求职信息get：/api/v1/job_intentions/me
更新当前用户的求职信息put：/api/v1/job_intentions/me
expected_positions: 求职岗位列表，可选，数组类型，多选，选项由业务提供
expected_salary_min: 期望薪资最小值，可选，整数，单位美元，≥0
expected_salary_max: 期望薪资最大值，可选，整数，单位美元，≥0，且 ≥ min
expected_location: 期望求职地点，可选，字符串类型，选项由业务提供

创建当前用户的求职信息post：/api/v1/job_intentions/me
expected_positions: 求职岗位列表，可选，数组类型，多选，选项由业务提供
expected_salary_min: 期望薪资最小值，可选，整数，单位美元，≥0
expected_salary_max: 期望薪资最大值，可选，整数，单位美元，≥0，且 ≥ min
expected_location: 期望求职地点，可选，字符串类型，选项由业务提供

IntentionScreen选择城市、选择岗位类型点击确定后需要创建
jobscreen选择城市、选择岗位类型点击确定后需要更新


<!-- 意见反馈 -->
<!-- telegram配置（接口） -->
<!-- telegram icon -->
<!-- 文字截断 -->
<!-- aibot增加...动画、意向、 -->
<!-- ai人物头像、应用商店宣传图 -->
facebook登陆

翻译确认

<!-- 对话中的工作岗位列表只取前5条，点击查看更多显示全部 -->

<!-- 测试过程中bug的修复、体验的优化 -->

<!-- 1、热门职位、 -->
<!-- 2、职位排序、城市排序 -->
3、
公司的logo

公司信息多语言支持
新增版本检测和更新
岗位要求中数据混杂：岗位要求、福利、时间

要是有公司门头或logo更好看
下面内容，分开描述才好看，不然太挤了

<!-- 列表item中的地址，有的是中文、英文、高棉语 -->
详情：fulltime、 month

埋点、

消息推送：
1、接入并记录设备信息
2、千人千面信息推送

分类没那么长
@陈邦冬  回复的内容文案要更有真人感一点
顶部工作时间怎么去了

埋点数据：页面访问量

<!-- 金刚区点击item跳转详情页面 -->