# dsh-whale-girl-pet 🐋

住在 DeepSeek Harness 界面里的 Q 版鲸鱼娘看板娘桌宠，右下角可拖拽。

基于 [Sutera-Diffusus/dsh-whale-musume](https://github.com/Sutera-Diffusus/dsh-whale-musume) 改造，新增：

- 🪙 **悬停显示账户余额** —— 鼠标放到看板娘身上，弹出余额气泡（读 DSH 内置账户接口，**无需外部代理**）
- 🎨 **右键「切换皮肤」** —— 联动 deep-whale 皮肤管理器，在「官方默认 / 深海女仆工坊 / 虎鲸链路」间即时切换
- 👀 **右键「查看余额」「显示/隐藏看板娘」** —— 与原生投喂 / 戳一下 / 夸夸 / 小游戏等动作并列

## 安装

```sh
dsh plugin --profile web add github:geniusstarshine/dsh-whale-girl-pet
```

装好后**重启一次 DSH**（或刷新页面），右下角即出现看板娘。

## 前置依赖

- 「切换皮肤」需要先装 [dsh-deep-whale 皮肤管理器](https://github.com/Small-tailqwq/dsh-deep-whale)：
  ```sh
  dsh plugin --profile web add '@smalltailqwq/dsh-client-ui-skin-deep-whale-manager'
  dsh plugin --profile web add '@smalltailqwq/dsh-client-ui-skin-maid-atelier'
  dsh plugin --profile web add '@smalltailqwq/dsh-client-ui-skin-orca-link'
  ```
- 余额来自 DSH 的 `deepseekAccount` 服务，登录 DeepSeek 账户即可。

## 设置

`设置 → 看板娘` 里有完整面板；悬停余额默认开启、默认显示具体数字，可在「余额」折叠项里调成只显示档位（不暴露金额）。

## 许可

- 代码：MIT（沿用上游）
- 立绘：AI 生成（沿用上游，版权见上游仓库）

## 致谢

原项目 [dsh-whale-musume](https://github.com/Sutera-Diffusus/dsh-whale-musume)。
