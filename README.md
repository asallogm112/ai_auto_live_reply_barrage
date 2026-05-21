# ai_auto_live_reply_barrage

参考 他这个AI-XiaoPi 项目 , 我现在 已经 拿到 抖音的弹幕 了,   后面 的 ai 回复 ( 根据弹幕内容 使用deepseek 生成 回复内容) , 对接 llm , 对接 index tts (qwen tts 等等), flow 流量控制  等等 代码 , 你给我  完整的 写出来  , 单独 新建一个 文件 将代码放进去 ,


回复 弹幕 是这个 逻辑 ,   1:  首先有一个队列 ,  根据关键词 触发 ,    将这个弹幕 放到队列里,  并且 每次 只处理一条 使用 deepseek 生成回复内容 , 然后生成tts,  这个队列 也 可以 手动 添加 需要处理的 弹幕 ,  也可以手动 剔除 等待需要处理的 弹幕 .    并且 这个弹幕 等等时间 过长 , 系统 会自动 剔除调 ,  超过 1分钟 自动 剔除 .  


QWEN_TTS_URL  现改用 免费的 edgetts 把 , 等功能调通了 , 我再 租用一个 云服务器 部署 qwentts 和 index tts . 后面只需 改动 QWEN_TTS_URL  INDEX_TTS_URL , 就 可以完成 切换
