# AI生图作品集
本仓库为个人AI生图创作作品集，包含3个主题共9张2048×2048分辨率的AI生成图片，以及全流程可复现的Prompt指令、参数配置与创作记录。

---

## 📁 仓库结构
| 文件/目录 | 说明 |
|----------|------|
| `prompt-engineer-test.md` | 完整创作记录文档（含正向/反向Prompt、核心参数、创作思路与效果说明） |
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

#### 图1：冬日松鼠（文件名：01-animal_squirrel_winter_2048x2048.png）
**Prompt**：
正向：mmjzcm,(1 single little squirrel, full body, no human, pure animal:2.2),chibi,super cute 3D cartoon animal illustration,round big black shiny eyes,soft fluffy brown fur,wearing warm orange knit hat with white pom-pom,white fluffy scarf,sitting on a snow-covered red mushroom,holding a light blue cup of hot cocoa with marshmallow in both front paws,snowflakes falling around,winter snow scene,green pine trees in background,soft warm lighting,bright vibrant color,smooth clean lines,clear picture layers,harmonious color matching,masterpiece,best quality,8k,ultra detailed,sharp focus,depth of field,mmjzm
反向：(human, person, girl, woman, man, child, human face, human body, anthropomorphic, furry, kemono, animal ears on human:2.2),(multiple squirrels, extra animals:1.6),(overcoat, thick coat, sled, blanket, coffee cup with logo:1.5),lowres,bad anatomy,bad hands,text,error,missing fingers,extra digit,fewer digits,cropped,worst quality,low quality,normal quality,jpeg artifacts,signature,watermark,username,blurry,ugly,deformed,mutated,disfigured,out of frame,extra limbs,floating limbs,disconnected limbs,malformed hands,long neck,duplicate,morbid,mutilated,poorly drawn face,poorly drawn hands,cloned face,gross proportions,nsfw

**核心参数**：Steps: 30, Sampler: DPM++ 2M, CFG scale: 7.0, Seed: 389272458, Size: 1024x1024, Model hash: 8cba4f1ef4, Model: F.1基础算法模型-哩布在线可运行_F.1-dev-fp8.safetensors, Denoising strength: 0.35, RNG: CPU, Lora 1: 萌萌哒胖猫卡通3D插画场景模型, Lora Hash 1: 23917ea983, Lora Weight 1: 0.7, vae_name: automatic, Hires resize: 2048x2048, Hires steps: 15, Hires upscaler: R-ESRGAN_4x+ Anime6B，生成时间：50s±3s（无ControlNet配置）

**创作与效果**：优化拟人化、多动物问题，最终主体清晰，冬日氛围饱满，风格统一。

#### 图2：春日兔子（文件名：01-animal_rabbit_spring_2048x2048.png）
**Prompt**：
正向：mmjzcm,(1 single lop-eared rabbit, full body, no human, pure animal:2.2),chibi,super cute 3D cartoon animal illustration,round big pink shiny eyes,soft fluffy gray fur,wearing dark blue casual suit,white shirt,sitting on green grass field,blowing dandelion,dandelion seeds flying in the wind,sunny spring day,blue sky with white clouds,wild flowers around,bright natural lighting,vibrant color,smooth clean lines,clear layers,harmonious color matching,masterpiece,best quality,8k,ultra detailed,sharp focus,depth of field,mmjzm
反向：(human, person, girl, woman, man, child, human face, human body, anthropomorphic, furry, kemono, animal ears on human:2.2),(multiple squirrels, extra animals:1.6),(overcoat, thick coat, sled, blanket, coffee cup with logo:1.5),lowres,bad anatomy,bad hands,text,error,missing fingers,extra digit,fewer digits,cropped,worst quality,low quality,normal quality,jpeg artifacts,signature,watermark,username,blurry,ugly,deformed,mutated,disfigured,out of frame,extra limbs,floating limbs,disconnected limbs,malformed hands,long neck,duplicate,morbid,mutilated,poorly drawn face,poorly drawn hands,cloned face,gross proportions,nsfw

**核心参数**：Steps: 30, Sampler: DPM++ 2M, CFG scale: 7.0, Seed: 389272458, Size: 1024x1024, Model hash: 8cba4f1ef4, Model: F.1基础算法模型-哩布在线可运行_F.1-dev-fp8.safetensors, Denoising strength: 0.35, RNG: CPU, Lora 1: 萌萌哒胖猫卡通3D插画场景模型, Lora Hash 1: 23917ea983, Lora Weight 1: 0.7, vae_name: automatic, Hires resize: 2048x2048, Hires steps: 15, Hires upscaler: R-ESRGAN_4x+ Anime6B，生成时间：45s±3s（无ControlNet配置）

**创作与效果**：修正耳朵比例、场景亮度，垂耳兔形态自然，春日氛围清新。

#### 图3：夏日橘猫（文件名：01-animal_cat_summer_2048x2048.png）
**Prompt**：
正向：mmjzcm,(1 single orange tabby cat, full body, no human, pure animal:2.2),chibi,super cute 3D cartoon animal illustration,round big green shiny eyes,soft fluffy orange fur,wearing light blue beach shirt,sunglasses on head,sitting on beach wooden chair,holding a rainbow ice cream cone in both front paws,blue sea and sky in background,seagulls flying around,summer beach scene,bright sunlight,vibrant warm color,smooth clean lines,clear layers,harmonious color matching,masterpiece,best quality,8k,ultra detailed,sharp focus,depth of field,mmjzm
反向：(human, person, girl, woman, man, child, human face, human body, anthropomorphic, furry, kemono, animal ears on human:2.2),(multiple squirrels, extra animals:1.6),(overcoat, thick coat, sled, blanket, coffee cup with logo:1.5),lowres,bad anatomy,bad hands,text,error,missing fingers,extra digit,fewer digits,cropped,worst quality,low quality,normal quality,jpeg artifacts,signature,watermark,username,blurry,ugly,deformed,mutated,disfigured,out of frame,extra limbs,floating limbs,disconnected limbs,malformed hands,long neck,duplicate,morbid,mutilated,poorly drawn face,poorly drawn hands,cloned face,gross proportions,nsfw

**核心参数**：Steps: 30, Sampler: DPM++ 2M, CFG scale: 7.0, Seed: 389272458, Size: 1024x1024, Model hash: 8cba4f1ef4, Model: F.1基础算法模型-哩布在线可运行_F.1-dev-fp8.safetensors, Denoising strength: 0.35, RNG: CPU, Lora 1: 萌萌哒胖猫卡通3D插画场景模型, Lora Hash 1: 23917ea983, Lora Weight 1: 0.7, vae_name: automatic, Hires resize: 2048x2048, Hires steps: 30, Hires upscaler: 8x-NMKD-Superscale，生成时间：55s±2s（无ControlNet配置）

**创作与效果**：优化毛发质感、场景细节，完成四季萌宠系列闭环。

---

### 2. 迪士尼风格人鱼系列
- **风格**：经典迪士尼动画质感，唯美梦幻，色彩贴合迪士尼动画审美
- **核心**：单一人鱼主体+海洋场景层次丰富，比例协调
- **亮点**：结合IP-Adapter锁定风格，完成「深海-珊瑚-海岸」海洋场景系列闭环

#### 图1：贝壳上人鱼（文件名：02-mermaid_seashell_coral_2048x2048.png）
**Prompt**：
正向：Disney-style illustration,in the style of the reference picture,masterpiece,best quality,8k,ultra detailed,sharp focus, 1 cute little mermaid,human upper body,green iridescent fish tail,full body, long wavy red hair,big bright green eyes,soft sweet smile,wearing a seashell bra, sitting on a giant white seashell on colorful coral reef,holding a little clown fish in her hands, tropical fish swimming around,colorful corals and sea anemones,clear blue seawater, sunbeam shining through the water,bright vibrant color,smooth lines,clear picture layers, harmonious color matching,cinematic lighting,depth of field
反向：(2girls, multiple girls, duplicate:2),(fish, pure animal, no human, abstract, glitch, distorted, jelly texture, iridescent over-saturated color, plastic 3d render:2), lowres,bad anatomy,bad hands,text,error,missing fingers,extra digit,fewer digits,cropped, worst quality,low quality,jpeg artifacts,signature,watermark,username,blurry,ugly,deformed, mutated,disfigured,out of frame,extra limbs,floating limbs,disconnected limbs,malformed hands, long neck,duplicate,morbid,mutilated,poorly drawn face,poorly drawn hands,cloned face,gross proportions,nsfw

**核心参数**：Steps: 28, Sampler: DPM++ 2M, CFG scale: 7.0, Seed: 3708432142, Size: 1024x1024, Model hash: 8cba4f1ef4, Model: F.1基础算法模型-哩布在线可运行_F.1-dev-fp8.safetensors, Denoising strength: 0.3, RNG: CPU, Lora 1: Disney Anime Style Illustration, Lora Hash 1: 466a765bad, Lora Weight 1: 0.8, Controlnet 0: "preprocessor: ip-adapter-siglip, model: InstantX-F.1-dev-IP-Adapter, weight: 0.6, starting/ending: (0.0, 1.0), resize mode: Crop and Resize, pixel_perfect: False, control mode: Balanced, preprocessor params: (512, None, None)", vae_name: automatic, Hires resize: 2048x2048, Hires steps: 18, Hires upscaler: R-ESRGAN_4x+ Anime6B，生成时间：56s±2s

**创作与效果**：修正比例、色彩问题，迪士尼风格鲜明，场景层次丰富。

#### 图2：珊瑚中嬉戏的人鱼（文件名：02-mermaid_swim_coral_2048x2048.png）
**Prompt**：
正向：Disney-style illustration,masterpiece,best quality,8k,ultra detailed,sharp focus, (1 cute little mermaid:2.5),(long wavy bright red hair:2),(human upper body, green iridescent fish tail, full body:2), Disney-style illustration,big bright green eyes,happy excited expression,wearing a colorful seashell-style outfit, swimming through a vibrant coral reef,surrounded by small colorful tropical fish, sunbeams filtering through clear blue seawater,bubbles floating around,dynamic swimming pose, well-proportioned body,slender waist,smooth cartoon lines,bright ocean colors,cinematic lighting,depth of field
反向：(2girls, multiple girls, duplicate, clone:3),(pink hair, purple hair, blonde hair:2.5), modern clothes,urban setting,indoors,furniture,black crop top,gray pleated skirt, fish,pure animal,no human,abstract,glitch,distorted,plastic 3d render,jelly texture,over-saturated, lowres,bad anatomy,bad hands,text,error,missing fingers,extra limbs,floating limbs,malformed hands, long neck,blurry,ugly,deformed,disfigured,noisy,grainy,signature,watermark,nsfw

**核心参数**：Steps: 28, Sampler: DPM++ 2M, CFG scale: 7.5, Seed: 3540362029, Size: 1024x1024, Model hash: 8cba4f1ef4, Model: F.1基础算法模型-哩布在线可运行_F.1-dev-fp8.safetensors, Denoising strength: 0.3, RNG: CPU, Lora 1: 迪斯尼动漫风格插画, Lora Hash 1: 466a765bad, Lora Weight 1: 0.6, vae_name: automatic, Hires resize: 2048x2048, Hires steps: 18, Hires upscaler: R-ESRGAN_4x+ Anime6B，生成时间：50s±2s（无ControlNet配置）

**创作与效果**：优化姿态、发色，人鱼灵动，场景明亮活泼。

#### 图3：海岸上坐着的人鱼（文件名：02-mermaid_coast_night_2048x2048.png）
**Prompt**：
正向：Disney-style illustration,masterpiece,best quality,8k,ultra detailed,sharp focus, (1 cute little mermaid:2.5),(long wavy bright red hair:2),(human upper body, green iridescent fish tail, full body:2), Disney-style illustration,big bright green eyes,gentle soft smile,wearing a colorful seashell-style outfit, lying on a wet seaside rock above the sea,night scene,full moon hanging in the dark blue sky, stars twinkling,distant sailing ship on the horizon,soft moonlight lighting, glowing bioluminescent sea water,dreamy soft ocean colors,smooth cartoon lines,cinematic volumetric lighting,depth of field
反向：(2girls, multiple girls, duplicate, clone:3),(pink hair, purple hair, blonde hair:2.5), modern clothes,urban setting,indoors,furniture,black crop top,gray pleated skirt, fish,pure animal,no human,abstract,glitch,distorted,plastic 3d render,jelly texture,over-saturated, lowres,bad anatomy,bad hands,text,error,missing fingers,extra limbs,floating limbs,malformed hands, long neck,blurry,ugly,deformed,disfigured,noisy,grainy,signature,watermark,nsfw

**核心参数**：Steps: 30, Sampler: DPM++ 2M, CFG scale: 7.5, Seed: 915792956, Size: 1024x1024, Model hash: 8cba4f1ef4, Model: F.1基础算法模型-哩布在线可运行_F.1-dev-fp8.safetensors, Denoising strength: 0.3, RNG: CPU, Lora 1: 迪斯尼动漫风格插画, Lora Hash 1: 466a765bad, Lora Weight 1: 0.6, vae_name: automatic, Hires resize: 2048x2048, Hires steps: 18, Hires upscaler: R-ESRGAN_4x+ Anime6B，生成时间：50s±2s（无ControlNet配置）

**创作与效果**：强化夜景氛围，画面梦幻，完成海洋场景系列闭环。

---

### 3. 小女孩生活场景系列
- **风格**：写实卡通，温馨明亮，人物特征统一
- **核心**：单人主体+IP-Adapter人脸锁定+生活化场景，贴合日常氛围
- **亮点**：通过多ControlNet单元强化人脸一致性，完成「室内-户外-海边」生活场景系列闭环

#### 图1：画室写生（文件名：03-girl_studio_paint_2048x2048.png）
**Prompt**：
正向：masterpiece,best quality,8k,ultra detailed,sharp focus,photorealistic cartoon style,1 little girl,6 years old,soft cute facial features,fair skin,focused smile,wearing white smock with paint splatters,pink hair clip,sitting on a wooden stool in a bright art studio,holding a paintbrush and painting on a canvas,easel beside her,colorful watercolor paints,paint tubes,sketchbooks on the table,sunbeams through studio window,potted succulent on the windowsill,soft warm lighting,depth of field,smooth lines,vivid colors
反向：lowres,bad anatomy,bad hands,text,error,missing fingers,extra digit,fewer digits,cropped,worst quality,low quality,normal quality,jpeg artifacts,signature,watermark,username,blurry,ugly,deformed,mutated,disfigured,out of frame,extra limbs,floating limbs,disconnected limbs,malformed hands,long neck,duplicate,morbid,mutilated,poorly drawn face,poorly drawn hands,cloned face,gross proportions,nsfw

**核心参数**：Steps: 30, Sampler: DPM++ 2M Karras, CFG scale: 7.5, Seed: 1429596257, Size: 1024x1024, Model hash: aadddd3d75, Model: Deliberate_V3.0.safetensors, Denoising strength: 0.35, Clip skip: 2, RNG: CPU, Controlnet 0: "preprocessor: ip-adapter_face_id_plus, model: ip-adapter-faceid-plus_sd15, weight: 0.7, starting/ending: (0.0, 1.0), resize mode: Crop and Resize, pixel_perfect: False, control mode: Balanced, preprocessor params: (512, None, None)", vae_name: automatic, Hires resize: 2048x2048, Hires steps: 15, Hires upscaler: 8x-NMKD-Superscale，生成时间：100s±2s

**创作与效果**：锁定人脸特征，优化光线，场景温馨，细节丰富。

#### 图2：海边捡贝壳（文件名：03-girl_beach_shells_2048x2048.png）
**Prompt**：
正向：masterpiece,best quality,8k,ultra detailed,photorealistic cartoon style,(extremely solo:1.8),only 1 little girl,6 years old,big blue eyes,light brown hair,wearing white floral dress and white sandals,squatting on a golden sandy beach,holding a small wicker basket filled with colorful seashells,sunny day,blue sky,gentle waves,seagulls flying,soft sunlight,depth of field
反向：lowres,bad anatomy,bad hands,multiple girls,2girls,3girls,no humans,ugly,deformed,blurry,extra limbs,fused fingers,duplicate figures,nsfw

**核心参数**：Steps: 30, Sampler: DPM++ 2M Karras, CFG scale: 7.5, Seed: 373186253, Size: 1024x1024, Model hash: 9ABA26ABDF, Model: 真实感必备模型｜Deliberate_v2.safetensors, Denoising strength: 0.35, Clip skip: 2, RNG: CPU, Controlnet 0: "preprocessor: ip-adapter_face_id_plus, model: ip-adapter-faceid-portrait_sd15, weight: 0.75, starting/ending: (0.0, 1.0), resize mode: Crop and Resize, pixel_perfect: False, control mode: Balanced, preprocessor params: (512, None, None)", Controlnet 1: "preprocessor: ip-adapter_face_id_plus, model: ip-adapter-faceid-plus_sd15, weight: 0.75, starting/ending: (0.0, 1.0), resize mode: Crop and Resize, pixel_perfect: False, control mode: Balanced, preprocessor params: (512, None, None)", Controlnet 2: "preprocessor: ip-adapter_face_id_plus, model: ip-adapter-faceid-plus_sd15, weight: 0.75, starting/ending: (0.0, 1.0), resize mode: Crop and Resize, pixel_perfect: False, control mode: Balanced, preprocessor params: (512, None, None)", vae_name: automatic, Hires resize: 2048x2048, Hires steps: 15, Hires upscaler: R-ESRGAN_4x+ Anime6B，生成时间：55s±2s

**创作与效果**：强化单人约束，优化细节，完成生活场景系列闭环。

#### 图3：星空露营（文件名：03-girl_camp_star_2048x2048.png）
**Prompt**：
正向：masterpiece,best quality,8k,ultra detailed,sharp focus,photorealistic cartoon style,1 little girl,6 years old,big round blue eyes,long curly brown hair,soft cute facial features,fair skin,amazed expression,wearing yellow hoodie and denim shorts,sitting on a checkered picnic blanket beside a small tent,holding a glowing firefly jar,campfire with marshmallows on a stick,starry night sky with milky way,fireflies floating around,distant pine trees,soft warm campfire light mixing with cool starlight,depth of field,smooth lines,dreamy atmosphere
反向：lowres,bad anatomy,bad hands,text,error,missing fingers,extra digit,fewer digits,cropped,worst quality,low quality,normal quality,jpeg artifacts,signature,watermark,username,blurry,ugly,deformed,mutated,disfigured,out of frame,extra limbs,floating limbs,disconnected limbs,malformed hands,long neck,duplicate,morbid,mutilated,poorly drawn face,poorly drawn hands,cloned face,gross proportions,nsfw

**核心参数**：Steps: 30, Sampler: DPM++ 2M Karras, CFG scale: 7.5, Seed: 1777983345, Size: 1024x1024, Model hash: aadddd3d75, Model: Deliberate_V3.0.safetensors, Denoising strength: 0.35, Clip skip: 2, RNG: CPU, Controlnet 0: "preprocessor: ip-adapter_face_id_plus, model: ip-adapter-faceid-plus_sd15, weight: 0.7, starting/ending: (0.0, 1.0), resize mode: Crop and Resize, pixel_perfect: False, control mode: Balanced, preprocessor params: (512, None, None)", vae_name: automatic, Hires resize: 2048x2048, Hires steps: 15, Hires upscaler: 8x-NMKD-Superscale，生成时间：65s±2s

**创作与效果**：强化星空、发光效果，光影协调，露营氛围浓厚。

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
2. 打开 `prompt-engineer-test.md`，可查看每张图的完整Prompt、参数细节与创作过程；
3. 所有配置均可直接复现，便于学习与参考。

---

## 📝 创作总结
### 核心心得
1. **风格统一控制**：不同主题采用差异化的模型+Lora组合，动物类用3D卡通Lora、人鱼类用迪士尼风格Lora、人物类用写实卡通模型，确保同系列风格完全统一，符合主题审美要求。
2. **主体约束优化**：通过提升`solo/single`关键词权重、反向提示词强排除多主体，彻底解决了多人物/多动物重叠的核心问题，保证所有画面主体唯一。
3. **细节与质量平衡**：针对不同场景补充专属细节描述，结合低重绘幅度的高清修复，在保证2048×2048高清分辨率的同时，避免画面失真，兼顾细节丰富度与整体质感。

### 核心挑战与解决方案
| 核心挑战 | 落地解决方案 |
|----------|--------------|
| 人脸/动物特征不一致 | 启用IP-Adapter特征锁定，权重控制在0.7-0.8，平衡特征还原度与画面自然度 |
| 画面色彩过饱和/过暗 | 调整CFG scale至7.0-7.5，补充精准的光影描述词，优化采样步数至28-30步 |
| 高清修复画面失真 | 重绘幅度控制在0.3-0.35，匹配适配的放大算法，分阶段先验证小图再放大生成 |
