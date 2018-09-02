# Changelog

> 更新日志


### 5.4.2

- 调整：可以通过快捷键置顶图片文件，让右键可以捕获图片


### 5.4.1

- 修复：导致 `WebP` 等格式的图片上传失败的一处递归错误


### 5.4.0

- 新增：导出日志功能，便于分析问题的原因
- 调整：用户处于已登录状态，上传失败不再中断后续队列


### 5.3.0

- 移除：微博图片用户信息卡（CSP及框架之间的跨越问题造成普适性较差）
- 移除：周期性请求用户状态（不具有实用性）
- 调整：使用样式注入而不是插入样式（样式注入不受网站的CSP策略影响）
- 新增：通知我更新详情（可选关闭更新时的日志弹窗）


### 5.2.2

- 新增：快捷键 `Alt+Shift+C` 来禁用/启用当前域名下的微博信息卡功能


### 5.2.1

- 新增：微博图片用户信息卡，一键查看图片PO主的信息（可以在选项页面中启用此功能）


### 5.2.0

- 优化：重新设计微博相关的APIs，移除冗余的代码
- 新增：长期保持微博用户登录状态的功能（可以在选项页面中启用此功能）


### 5.1.1

- 恢复：网页图片、视频帧的采集自动写入剪切板


### 5.1.0

- 移除：腾讯云存储(COS)+万象优图的图片处理功能
- 其他：接入 V4 版本的功能，详情请查看 V4 版本的更新记录


### 4.0.0 (Beta)

- 移除：网页增强功能，取消自定义微博传图（breaking change）
- 调整：上传记录页面改为瀑布流模式（UX breaking change）
- 调整：网页图片、视频帧的采集不在自动写入剪切板（breaking change）
- 新增：支持腾讯云存储(COS)+万象优图的图片处理
- 新增：上传记录中的图片支持批量删除


### 3.2.0

- 重要：新版仅支持 Chrome 66+
- 移除：对 weibo.com 域下 cookies 的 secure 属性校验和警告提示
- 调整：自动置前已打开的上传弹窗，不在用闪烁表示上传窗口已打开
- 优化：粘贴区域扩展到弹窗大小，消除多余的点击操作（UX breaking change）


### 3.1.0

- 重要：新版仅支持 Chrome 65+（降级浏览器至 65 以下无法使用此扩展）
- 改版：完全启用 ES-next Modules
- 优化：更换为新的上传接口（感谢 @xmdhs 提供新接口信息）
- 优化：弹窗上传页面最大适应至浏览器 125% 的放大效果


### 2.2.9

- 新增：打开上传窗口的快捷键（Shift+Alt+W）
- 新增：对 weibo.com 域下 cookies 的 secure 属性校验和警告提示


### 2.2.8

- 冲突：解决 [LeaVerou/prefixfree](https://github.com/LeaVerou/prefixfree/issues/6131) bug 引起样式泄漏的问题


### 2.2.5

- 修复：QQ 邮箱重用扩展注入的 Style 导致的样式泄露问题


### 2.2.3

- 新增：支持把视频的当前帧上传为 JPG 图像
- 其他：汉化上传弹窗中的部分英文词组


### 2.2.1

- 改动：上传方式改为串行，预防微博限制并发数量而导致上传失败
- 其他：代码风格的变动，部分借鉴 Angular 2.0+ 的编码规范


### 2.1.0

- 改动：用户模块中的属性变更，由 postfix 改为 suffix（breaking change）
- 移除：不再支持 SVG 有损转换为 PNG
- 优化：从字节流中读取图片正确的 MIME Type


### 2.0.0

- 改版：2.0.0
- 完善：所有图片的上传和下载操作均支持进度显示
- 优化：右键上传获取图片时，应用 Referer 请求头


### 1.6.1

- 修复：微相册达到存储上限后不能添加图片（现在自动移除最前的 50 张图片）


### 1.6.0

- 新增：BMP、WebP、ico、SVG 格式支持（有损转换为 PNG）


### 1.5.1

- 修复：国外网络下打开微博登录页面不正确的问题


### 1.5.0

- 优化：自动重试微博登录，不再频繁提示微博未登录
- 修复：潜在的重复创建微相册的问题
- 完善：支持 Animated PNG(APNG) 标准的 MIME Type