# 构图：景别、机位、视角、焦距

> 用到才读：写 `t2i` 开篇句、要给画面定「相机怎么拍」时才打开。本章不重复 SKILL.md 的八步流程。

## 三条纪律（先看）

1. **一律写成陈述句，不是指令。** `t2i` 是观察者报告视角 —— `shot from just inside the entrance at chest height` 陈述的是「这张照片从什么视角拍的」，合法；`shoot this at chest height` 是祈使句，违反语气纪律。
2. **别把「横向画幅」和「广角镜头」混成一个词。** 开篇句模板里的 `wide` 指画面**朝向**，由 `wh_ratio` 决定；`wide-angle lens` 是**焦段**。两者可以同时成立，也可以只有其一。
3. **每层取一个值就够了。** 景别 × 机位高度 × 视角角度各选一格，堆多个会让描述自相矛盾（模型自己挑一个，等于白写）。

---

## 1. 景别（画面里装多少）

| 写法 | 装多少 | 适用题材 |
|---|---|---|
| `an extreme long shot` | 主体极小，环境占绝对主导 | 风景、天际线、人群、大场面 |
| `a long shot` / `a wide shot` | 全身 + 大量环境 | 建筑外观、街头、群像 |
| `a full shot` | 人物全身刚好入画，几乎不留上下余量 | 时装、模特、演示动作 |
| `a medium shot` | 腰部以上 | 访谈、带动作的人物 |
| `a medium close-up` | 胸部以上 | 对话、肖像 |
| `a close-up` | 头肩，或单件物体填满画面 | 面部、食物、道具 |
| `an extreme close-up` | 局部：一只眼、一处纹理、一道边缘 | 材质、微观细节 |
| `an insert shot` | 单独交代一个细节物件 | 手部动作、仪表读数 |

---

## 2. 机位高度

| 写法 | 效果 | 适用题材 |
|---|---|---|
| `shot from ground level` | 贴地，前景被压得很扁 | 宠物、车轮、草丛、童趣视角 |
| `shot from knee height` | 低机位 | 儿童视角、地面物件 |
| `shot from waist height` | 略低于视线 | 桌面静物、日常随手 |
| `shot from chest height` | 与站姿视线齐平 | **通用默认** |
| `shot from eye level` | 与被摄对象视线齐平 | 人像、对峙感 |
| `shot from just above shoulder height` | 略俯，视线越过近处障碍 | 展示台面内容、越过人群 |

---

## 3. 视角角度

| 写法 | 效果 | 适用题材 |
|---|---|---|
| `shot straight on, camera level and squared to the subject` | 正面平视，无透视变形 | 建筑立面、界面、菜单板、要求对称的画面 |
| `shot slightly from above, angled down` | 轻微俯拍 | 桌面、商品平铺、地图 |
| `a high angle looking down` | 强俯视，主体被压扁 | 人群、棋盘格局、脆弱感 |
| `shot slightly from below, angled up` | 仰拍 | 威严、高耸、压迫感 |
| `a worm's-eye view` | 极低仰视 | 夸张高度、英雄感 |
| `a bird's-eye view` | 接近垂直向下俯视 | 交通、俯瞰规划、图案感 |
| `a three-quarter view` | 约 45° 侧转 | 人像与产品的通用解 |
| `tilted slightly off level` | 轻微倾斜（荷兰角） | 不安、动感、街头快照 |

---

## 4. 焦距与透视

| 写法 | 效果 | 适用题材 |
|---|---|---|
| `shot on a wide-angle lens, with the edges stretching outward` | 透视夸张、前后景距离被拉开 | 局促空间显得更宽、建筑内部 |
| `shot on a standard lens` | 接近人眼所见 | 通用默认 |
| `shot on a short telephoto, the background drawn slightly closer` | 轻微空间压缩，背景贴近主体 | 人像 |
| `shot on a long telephoto, flattening the distance between foreground and background` | 强烈压缩，背景被拉近甚至呈环状 | 远景裁切、运动场、远距观察 |

⚠️ 同一句里焦段与透视效果要一致 —— 写了 `wide-angle` 却描述「背景被拉近」，等于给模型两个互斥指令。这与 Step 7 的光照自洽是同一条纪律。

---

## 5. 景深与焦平面

和 Step 5「单主体填满」里那句「背景及虚化程度」配套：

| 写法 | 场景 |
|---|---|
| `with the sharpest plane landing on ⟨X⟩` | 明确指定锐焦点落在哪个元素 |
| `everything from front to back in focus` | 全景深：风光、产品图、图表 |
| `shallow depth of field, the background thrown out of focus` | 浅景深：人像、特写 |
| `background softened but still readable` | 半虚化：要保留环境信息时 |
| `with bokeh in the out-of-focus background` | 背景光斑 |

---

## 6. 给收尾句的构图词（法则层）

Step 8 的收尾句默认是 `balanced and near-symmetrical`。画面不是对称结构时可以换成：

| 写法 | 法则 |
|---|---|
| `balanced and near-symmetrical` | 居中对称（默认） |
| `composed roughly on thirds, with ⟨X⟩ set slightly left of centre` | 三分法 |
| `built on strong diagonals running from the lower left to the upper right` | 对角线动势 |
| `framed by ⟨X⟩ in the foreground, which falls out of focus` | 前景框景 / 框中框 |
| `with generous negative space around ⟨X⟩` | 留白 |
| `with leading lines that carry the eye from ⟨X⟩ to ⟨Y⟩` | 视线动线 |

⚠️ 收尾句**只写一句**，同一句里把构图、调色板、风格、氛围一次说完。

---

## 实测对照（诚实标注）

同 seed 受控对比下，**以下写明后被兑现**：

- `shot from just inside the entrance at chest height` → 机位确实是齐胸高
- `camera level and squared to the counter line` → 正面平视，水平线横贯全幅
- `with the sharpest plane landing on ⟨X⟩` → 焦平面落在指定元素上
- `conical metal shades hanging in a row`（连数量一起写）→ 数量与形状均兑现

**其余词条尚未验证**，按摄影惯例列出。⇒ 某个构图要求若是关键需求，**出图后自查一遍是否真的兑现**，不要假设写了就成立。
