# chat-image-inserter-
Chat Image Inserter 是一款为 SillyTavern（酒馆）设计的轻量级扩展，让角色对话中的文字能自动插入图片。

正文插图插件
中文介绍
Chat Image Inserter 是一款为 SillyTavern（酒馆）设计的轻量级扩展，让角色对话中的文字能自动"长出"图片。当 AI 的输出里出现你预设的关键词或正则模式时，插件会在文字下方无缝插入对应的本地图片——就像给聊天加了一层可编程的"表情系统"。

它能做什么
自定义文字匹配：每条规则支持普通文本或正则表达式，比如 *微笑*、（叹气）、^\[场景.*\]$ 都可以作为触发条件。

本地图片上传：图片直接存在浏览器 IndexedDB 里，不经过服务器，没有 404，不占酒馆后端空间。

按需加载：只有消息匹配到某条规则时才读取该规则的图片；设置页中的图片预览也会在滚动到附近时再加载。

自动插入：消息渲染时自动扫描文字，匹配到就在该位置下方插入图片，不改动原始对话内容。

次数限流：每条规则可设置"每则消息最多插入 N 次"，0 表示不限，避免长回复里同一张图刷屏。

尺寸控制：竖版图片和横版图片可分别设置最大宽度，图片保持原始比例；正方形图片使用横版上限。

存储管理：实时显示已缓存图片的数量与占用空间，一键清除全部图片（规则保留，只需重新上传）。

主题跟随：界面配色全部使用酒馆主题变量，深色/浅色自动适配。


Chat Image Inserter is a lightweight extension for SillyTavern that makes text in roleplay conversations automatically "grow" images. When the AI's output contains a keyword or regex pattern you've defined, the plugin seamlessly inserts the corresponding local image right below the matched text 

