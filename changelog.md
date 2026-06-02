1.4.7
1、接入tiktok sdk
2、修复登录页面page_view source字段
3、岗位详情页这四个点击对应事件未登录上报
翻译点击	job_translate_btn_click
收藏点击	job_favorite_btn_click
举报点击	job_report_entry_click
联系按钮点击	job_contact_btn_click
4、推荐按钮，未登录上报
5、新增系统授权弹窗埋点permission_prompt_show、permission_authorization_result、

1.4.6
1、版本检查
2、首页如果用户没有城市，授权城市后，直接选中当前城市
3、新增onboarding_job_intent_action
ios
4、修复求职意向岗位选择bug

v1.4.5更新内容
1、岗位反馈收集
2、简历引导

1、岗位 tab 完善简历 banner
显示条件：
已登录
联系次数>= 3
简历未完善（必填字段未填写）
当天没有关闭过对应入口（一天只弹一次）
2、岗位详情页完善简历浮窗
显示条件：
已登录
联系次数>= 3
简历未完善（必填字段未填写）
当天没有关闭过对应入口（一天只弹一次）
点击联系按钮后先弹出该浮窗
3、岗位反馈浮窗
显示条件：
已登录
点击联系按钮后，用户联系后返回app，弹出该浮窗

1.4.4
新增国家区号
搜索试试这样问替换为接口配置

1.4.3
1、修改必填字段
  必填字段：姓名、性别、出生年份、手机号、想在那里工作、想找什么工作
  非必填：真实照片
2、城市选择优化
  a、求职意向页面，请求定位权限，更新用户资料表，默认选中当前城市
  b、城市选择弹窗新增当前城市badge
  c、创建简历页面第三步，选择城市时默认选中当前城市
  d、岗位tab新增获取定位权限，城市modal/sheet显示当前城市


1.4
1、添加/编辑简历
2、job_list_filter埋点
3、首页默认显示最新
4、


ios 1.3.5
1、ios bug 岗位分类详情页面、岗位详情页面更多好工作、ai搜索结果列表jobitemview缺少了关闭按钮
2、Facebook登录
3、修改dodojob-pm v1.3的/analytics-latest.html
  1、job_preference_tag_click新增字段分类job_category_id、page（岗位tab页面、岗位详情页面）
  2、job_preference_submit新增字段job_category_id、page（岗位tab页面、岗位详情页面）
  3、更新后替换v1.4的/analytics-latest.html
  4、更新ios、安卓这两个埋点

android 1.3.5
1、安卓bug，岗位详情页更多好工作jobitemcard缺少了关闭按钮
2、
3、修改dodojob-pm v1.3的/analytics-latest.html
  1、job_preference_tag_click新增字段分类job_category_id、page（岗位tab页面、岗位详情页面）
  2、job_preference_submit新增字段job_category_id、page（岗位tab页面、岗位详情页面）
  3、更新后替换v1.4的/analytics-latest.html
  4、更新ios、安卓这两个埋点