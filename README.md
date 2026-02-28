```markdown
# AI生图作品集
本仓库为 **Prompt工程师岗位测试** 的完整成果，包含3个主题共9张2048×2048分辨率的AI生成图片，以及全流程可复现的Prompt指令、参数配置与调试记录。

---

## 📁 仓库结构
| 文件/目录 | 说明 |
|----------|------|
| `prompt-engineer-test.md` | 完整创作记录文档（含正向/反向Prompt、核心参数、调试思路与效果说明） |
| `01-animal_squirrel_winter_2048x2048.png` | 萌趣动物系列 - 冬日松鼠 |
| `01-animal_rabbit_spring_2048x2048.png` | 萌趣动物系列 - 春日兔子 |
| `01-animal_cat_summer_2048x2048.png` | 萌趣动物系列 - 夏日橘猫 |
| `02-mermaid_seashell_coral_2048x2048.png` | 迪士尼风格人鱼系列 - 贝壳上人鱼 |
| `02-mermaid_swim_coral_2048x2048.png` | 迪士尼风格人鱼系列 - 珊瑚中嬉戏的人鱼 |
| `02-mermaid_coast_night_2048x2048.png` | 迪士尼风格人鱼系列 - 海岸月夜人鱼 |
| `03-girl_studio_paint_2048x2048.png` | 小女孩生活场景系列 - 花房画室写生 |
| `03-girl_beach_shells_2048x2048.png` | 小女孩生活场景系列 - 海边捡贝壳 |
| `03-girl_camp_star_2048x2048.png` | 小女孩生活场景系列 - 星空露营 |

---

## 🎨 创作主题与风格
### 1. 萌趣动物系列
- **风格**：Q版3D卡通，明亮饱满，符合欧美卡通审美
- **核心**：四季场景+单动物主体+拟人化穿搭，无人类元素
- **亮点**：通过强权重约束实现风格统一，完成「春夏秋冬四季萌宠」系列闭环

### 2. 迪士尼风格人鱼系列
- **风格**：经典迪士尼动画质感，唯美梦幻，色彩贴合迪士尼动画审美
- **核心**：单一人鱼主体+海洋场景层次丰富，比例协调
- **亮点**：结合IP-Adapter锁定风格，完成「深海-珊瑚-海岸」海洋场景系列闭环

### 3. 小女孩生活场景系列
- **风格**：写实卡通，温馨明亮，人物特征统一
- **核心**：单人主体+IP-Adapter人脸锁定+生活化场景，贴合日常氛围
- **亮点**：通过多ControlNet单元强化人脸一致性，完成「室内-户外-海边」生活场景系列闭环

---

## 🛠️ 核心创作配置
- **生图平台**：LibLibAI（哩布哩布AI WebUI可视化界面）
- **基础Checkpoint模型**：
  - F.1基础算法模型-哩布在线可运行_F.1-dev-fp8.safetensors
  - Deliberate_V3.0.safetensors
  - Deliberate_v2.safetensors
- **风格Lora模型**：
  - 萌萌哒胖猫卡通3D插画场景模型（权重0.7）
  - Disney Anime Style Illustration（权重0.6-0.8）
- **ControlNet配置**：
  - ip-adapter-siglip / InstantX-F.1-dev-IP-Adapter（权重0.6）
  - ip-adapter_face_id_plus / ip-adapter-faceid-plus_sd15（权重0.7-0.75）
- **通用生成参数**：
  - 采样器：DPM++ 2M / DPM++ 2M Karras
  - 迭代步数：28-30步
  - CFG scale：7.0-7.5
  - 高清修复：放大算法R-ESRGAN_4x+ Anime6B / 8x-NMKD-Superscale，重绘幅度0.3-0.35，最终分辨率2048×2048

---

## 📖 查看与使用
1. 直接点击图片文件名，可在GitHub中预览2048×2048高清成品；
2. 打开 `prompt-engineer-test.md`，可查看每张图的完整Prompt、参数细节与调试过程；

---

## ✅ 合规说明
- 全程未使用禁用的LCM/Lightning蒸馏模型、强结构ControlNet；
- 仅使用合规开源Diffusion模型与IP-Adapter类特征锁定工具；
- 所有生图参数、Prompt均可复现.
```
