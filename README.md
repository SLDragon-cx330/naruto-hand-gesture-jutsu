# Webcam Ninjutsu FX · 摄像头手势忍术特效

纯前端网页 Demo：打开摄像头后，用 **MediaPipe Hands** 识别结印手势，再用 **Three.js** 叠加粒子 / 电弧 / 火焰等特效。

> 本项目为粉丝向技术演示，与《火影忍者》及相关权利方无关，仅供学习与个人娱乐。

## 功能

| 页面 | 忍术 | 触发手势（简述） |
|------|------|------------------|
| `effects/rasengan.html` | 螺旋丸 | 双手靠近合拢 / 单手握拳捧于胸前 |
| `effects/chidori.html` | 千鸟 | 单手食指竖起 |
| `effects/gokakyu.html` | 豪火球之术 | 双手五指张开并拉开 |
| `effects/chibaku-tensei.html` | 地爆天星 | 双手举过头顶 |
| `effects/all-jutsu.html` | 合集页 | 多招切换（持续可扩展） |

## 快速开始

1. 用本地静态服务器打开（摄像头在 `file://` 下常被浏览器拦截）：

```bash
# 任选其一
npx --yes serve .
# 或
python -m http.server 5179
```

2. 浏览器访问对应 HTML，允许摄像头权限。
3. 光线充足、手势正对镜头、动作稍慢更稳。

手机浏览器同样可用：部署到任意 HTTPS 静态托管后，用手机打开链接即可。

## 技术栈

- [MediaPipe Hands](https://developers.google.com/mediapipe/solutions/vision/hand_landmarker)（CDN）
- [Three.js](https://threejs.org/)（CDN）
- 原生 HTML / CSS / JS，无需构建

## 目录

```
effects/
  rasengan.html          # 螺旋丸
  chidori.html           # 千鸟
  gokakyu.html           # 豪火球
  chibaku-tensei.html    # 地爆天星
  all-jutsu.html         # 合集
```

## 隐私

- 手势识别在浏览器本地运行，画面默认不上传服务器。
- 本仓库不含账号、密钥、私有配置。

## 免责声明

- 视觉效果仅为致敬向娱乐实现，不构成对任何商标 / 版权作品的授权或关联。
- 请勿用于商业侵权用途；二次分发请保留本说明与许可证。
- 使用摄像头请遵守当地法律与他人隐私。

## License

MIT — 见 [LICENSE](./LICENSE)
