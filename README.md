# 通用游戏设计文档（GDD）框架

## 一、基础信息（Basic Information）

1. **游戏名称**  
   `{{GAME_TITLE}}`

2. **背景故事**  
   `{{GAME_BACKGROUND}}`

3. **游戏类型**
    - **主类型**: `{{PRIMARY_GENRE}}`
    - **副类型**: `{{SECONDARY_GENRE}}`
    - **玩法特色**: `{{MECHANIC_LIST}}`

4. **美术风格**
    - **核心风格**: `{{CORE_ART_STYLE}}`
    - **色彩基调**: `{{COLOR_TONE}}`
    - **视觉特效**: `{{VISUAL_EFFECTS}}`
    - **动态表现**: `{{DYNAMIC_EXPRESSION}}`

5. **游戏尺寸**  
   `{{RESOLUTION_WIDTH}} × {{RESOLUTION_HEIGHT}}`（`{{SCREEN_ORIENTATION}}`）

6. **游戏题材**  
   `{{CORE_THEME}}`

7. **文化背景**  
   `{{CULTURAL_BACKGROUND}}`

8. **核心关键词**  
   `{{KEYWORD_LIST}}`

9. **游戏描述**
    - **游戏大纲**: `{{INFORMATION}}`
    - **玩家目标**: `{{PLAYER_GOAL}}`

---

## 二、系统功能（System Features）

### 2.1 玩法核心层（所有游戏必填）

#### 2.1.1 输入与交互
- **玩家交互方式**: `{{PLAYER_INTERACTION}}`
- **核心操作动词**: `{{CORE_ACTIONS}}`

#### 2.1.2 核心机制
- **核心玩法机制**: `{{CORE_MECHANICS}}`
- **反馈机制**: `{{FEEDBACK_SYSTEM}}`

### 2.2 功能模块层
**已启用模块**: `{{ENABLED_MODULES}}`

#### □ 模块 A：角色与成长
> **适用**: RPG / ARPG / Roguelike / 养成 / 模拟经营  
> **启用**: `{{MODULE_A}}`

- **角色模式**: `{{CHARACTER_MODE}}`
- **核心属性**: `{{CHARACTER_STATS}}`
- **成长路径**: `{{CHARACTER_GROWTH}}`
- **养成周期**: `{{GROWTH_CYCLE}}`

#### □ 模块 B：关卡与地图
> **适用**: 线性叙事 / 动作 / 解谜 / 平台跳跃 / Roguelike  
> **启用**: `{{MODULE_B}}`

- **地图类型**: `{{MAP_TYPE}}`
- **章节总数**: `{{CHAPTER_COUNT}}`
- **关卡类型**: `{{LEVEL_TYPES}}`
- **关卡评价维度**: `{{RATING_CRITERIA}}`
- **通关奖励**: `{{CLEAR_REWARDS}}`

#### □ 模块 C：战斗与敌人
> **适用**: 动作 / RPG / 射击 / 塔防 / RTS / 格斗  
> **启用**: `{{MODULE_C}}`

**战斗设计**
- **战斗类型**: `{{COMBAT_TYPE}}`
- **核心战斗机制**: `{{COMBAT_MECHANICS}}`

**敌人设计**
- **敌人等级分类**: `{{ENEMY_TIERS}}`
- **AI 架构方式**: `{{ENEMY_AI_ARCH}}`
- **各级 AI 行为**: `{{ENEMY_AI_BEHAVIORS}}`

**□ 含 Boss 设计（子选项）**
- **Boss 特殊机制**: `{{BOSS_MECHANICS}}`
- **Boss 阶段数**: `{{BOSS_PHASE_COUNT}}`

#### □ 模块 D：经济与商店
> **适用**: 模拟经营 / RPG / 开放世界 / 卡牌 / 含内购游戏  
> **启用**: `{{MODULE_D}}`

**货币系统**
- **货币种类数**: `{{CURRENCY_COUNT}}`
- **货币列表**: `{{CURRENCY_LIST}}`
- **货币获取方式**: `{{CURRENCY_GET}}`

**商店系统**
- **商店类型**: `{{SHOP_TYPES}}`
- **商品分类**: `{{ITEM_CATEGORIES}}`

#### □ 模块 E：社交与多人
> **适用**: MMO / 多人联机 / 竞技 / 合作类  
> **启用**: `{{MODULE_E}}`

- **多人模式**: `{{MULTIPLAYER_MODE}}`
- **社交功能**: `{{SOCIAL_FEATURES}}`
- **通讯频道**: `{{CHAT_CHANNELS}}`
- **竞技系统**: `{{COMPETITIVE_SYSTEM}}`

#### □ 模块 F：特色玩法扩展
**启用**: `{{MODULE_F}}`

- **□ F-1 节奏/音乐玩法**
    - **节奏判定机制**: `{{RHYTHM_JUDGE}}`
    - **音符类型**: `{{NOTE_TYPES}}`
    - **连击系统**: `{{COMBO_SYSTEM}}`

- **□ F-2 模拟/经营玩法**
    - **模拟核心机制**: `{{SIMULATION_CORE}}`
    - **经营目标**: `{{MANAGEMENT_GOAL}}`

- **□ F-3 建造/沙盒玩法**
    - **建造维度**: `{{BUILD_DIMENSION}}`
    - **建造限制规则**: `{{BUILD_RULES}}`

- **□ F-4 卡牌/策略玩法**
    - **卡牌机制**: `{{CARD_MECHANICS}}`
    - **策略深度**: `{{STRATEGY_DEPTH}}`

- **□ F-5 其他特色玩法（兜底）**
    - **玩法名称**: `{{CUSTOM_FEATURE_NAME}}`
    - **核心规则**: `{{CUSTOM_FEATURE_RULES}}`

### 2.3 系统配置层

#### 2.3.1 设置系统
- **画质档位**: `{{QUALITY_OPTIONS}}`
- **操作设置项**: `{{CONTROL_OPTIONS}}`
- **语言支持**: `{{LANGUAGE_OPTIONS}}`

#### 2.3.2 音频系统
- **音频分轨控制**: `{{AUDIO_TRACKS}}`
- **动态音频机制**: `{{DYNAMIC_AUDIO}}`

## 三、游戏数值（Game Values）

### 3.1 玩家成长体系

#### 3.1.1 进度系统（玩家成长逻辑）
- **最大进度点数**: `{{PROGRESS_MAX}}`
- **进度增长计算公式**: `{{PROGRESS_FORMULA}}`
- **基础生命值**: `{{HP_BASE}}`
- **每进度点生命增长**: `{{HP_MULTIPLIER}}`
- **专属属性基础值**: `{{SPECIAL_ATTR_BASE}}`
- **专属属性进度增长系数**: `{{SPECIAL_ATTR_MULTIPLIER}}`
- **进度经验获取倍率**: `{{PROGRESS_EXP_MULTIPLIER}}`

#### 3.1.2 实体成长系统（怪物/单位/道具通用逻辑）
- **最小等级**: `{{ENTITY_MIN_LEVEL}}`
- **最大等级**: `{{ENTITY_MAX_LEVEL}}`
- **生命值计算公式**: `{{ENTITY_HP_FORMULA}}`
- **普通实体属性基础系数**: `{{NORMAL_ENTITY_COEF}}`
- **稀有实体属性强化系数**: `{{RARE_ENTITY_COEF}}`
- **稀有实体等级成长系数**: `{{RARE_ENTITY_LEVEL_COEF}}`

---

### 3.2 战斗与收益体系

#### 3.2.1 效果计算（伤害/收益通用公式）
- **攻击效果基础倍率**: `{{COEFFICIENT_ATTACK}}`
- **治疗效果基础倍率**: `{{COEFFICIENT_HEAL}}`
- **固定数值加成**: `{{FIXED_VALUE}}`
- **物理减伤率**: `{{PHYSICAL_REDUCTION_RATE}}`
- **法术减伤率**: `{{MAGIC_REDUCTION_RATE}}`
- **基础暴击率**: `{{BASE_CRIT_RATE}}`
- **暴击伤害倍率**: `{{CRIT_MULTIPLIER}}`
- **技能冷却缩减系数**: `{{COOLDOWN_REDUCTION}}`（
---

### 3.3 经济系统

#### 3.3.1 资源流通逻辑
- **基础货币名称**: `{{CURRENCY_A}}`
- **高级货币名称**: `{{CURRENCY_B}}`
- **基础货币兑换高级货币比例**: `{{CURRENCY_A_RATIO}}`
- **普通资源定价公式**: `{{COMMON_RESOURCE_PRICE}}`
- **稀有资源定价乘数**: `{{RARE_RESOURCE_PRICE_FACTOR}}`
- **付费资源定价基准**: `{{PAID_RESOURCE_BASE}}`
- **每日资源产出上限**: `{{DAILY_RESOURCE_LIMIT}}`

---

### 3.4 资源获取体系

#### 3.4.1 掉落与奖励通用逻辑
- **基础资源掉落率**: `{{BASE_RESOURCE_DROP}}`
- **等级递增掉落率**: `{{DROP_PER_LEVEL}}`
- **首通通关奖励数量**: `{{FIRST_CLEAR_BONUS}}`
- **稀有资源专属掉落率**: `{{RARE_RESOURCE_RATE}}`
- **每日资源保底次数**: `{{DAILY_DROP_MIN}}`
- **稀有资源保底概率**: `{{RARE_DROP_GUARANTEE}}`
- **保底重置周期**: `{{GUARANTEE_RESET_CYCLE}}`


## 四、角色设定（Character Design）

### 4.1 角色数量
**`{{MAIN_CHAR_COUNT}}`位主角 + `{{BOSS_COUNT}}`位Boss + `{{NPC_COUNT}}`个关键NPC**

---

### 4.2 主角设定

#### 4.2.1 {{MAIN_CHARACTER_NAME}}
- **身份**：`{{CHARACTER_ROLE}}`
- **性别**：`{{GENDER}}`
- **年龄**：`{{AGE}}`
- **外貌特征**：
    - `{{APPEARANCE_1}}`
    - `{{APPEARANCE_2}}`
    - `{{APPEARANCE_3}}`
    - `{{APPEARANCE_4}}`

- **角色风格**：`{{ART_STYLE}}`（如东方水墨/赛博朋克/奇幻童话）
- **性格特点**：`{{PERSONALITY_TRAITS}}`
- **核心能力**：
    - `{{ABILITY_1}}`：`{{ABILITY_DESCRIPTION_1}}`
    - `{{ABILITY_2}}`：`{{ABILITY_DESCRIPTION_2}}`
    - `{{ABILITY_3}}`：`{{ABILITY_DESCRIPTION_3}}`

- **成长曲线**：
    - `{{GROWTH_PHASE_1}}`：`{{PHASE_1_DESCRIPTION}}`
    - `{{GROWTH_PHASE_2}}`：`{{PHASE_2_DESCRIPTION}}`
    - `{{GROWTH_PHASE_3}}`：`{{PHASE_3_DESCRIPTION}}`

---

### 4.3 Boss角色设定

#### 4.3.1 {{BOSS_COUNT}}位Boss（示例：`{{BOSS_1_NAME}}`、`{{BOSS_2_NAME}}`...）
1. **`{{BOSS_1_NAME}}`**
    - **特点**：`{{BOSS_TRAIT_1}}`
    - **战斗风格**：`{{COMBAT_STYLE}}`
    - **核心机制**：`{{BOSS_MECHANICS}}`

2. **`{{BOSS_2_NAME}}`**
    - **特点**：`{{BOSS_TRAIT_2}}`
    - **战斗风格**：`{{COMBAT_STYLE}}`
    - **核心机制**：`{{BOSS_MECHANICS}}`

> *（注：按`{{BOSS_COUNT}}`数量自动生成，模板内保留3个示例）*

---

### 4.4 NPC角色

#### 4.4.1 关键NPC（`{{NPC_COUNT}}`个）
1. **`{{NPC_1_NAME}}`**
    - **身份**：`{{NPC_ROLE}}`
    - **功能**：`{{NPC_FUNCTION}}`
    - **交互内容**：`{{NPC_INTERACTION}}`

2. **`{{NPC_2_NAME}}`**
    - **身份**：`{{NPC_ROLE}}`
    - **功能**：`{{NPC_FUNCTION}}`
    - **交互内容**：`{{NPC_INTERACTION}}`

> *（注：按`{{NPC_COUNT}}`数量自动生成，模板内保留2个示例）*

---

### 4.5 角色关系网
- **核心羁绊**：`{{CORE_RELATIONSHIP}}`（如"师徒/仇敌/盟友"）
- **关键剧情触发点**：`{{KEY_PLOT_TRIGGER}}`
- **角色专属台词**：`{{CHARACTER_DIALOGUE}}`（示例：`"墨剑未寒，血债血偿"`）

## 五、视觉设计（Visual Design）

### 5.1 视觉风格定位

#### 5.1.1 整体风格
- **核心理念**: `{{CORE_VISUAL_CONCEPT}}`
- **色彩方案**:
    - 主色调: `{{PRIMARY_COLOR}}`
    - 辅助色: `{{SECONDARY_COLOR}}`
    - 点缀色: `{{ACCENT_COLOR}}`
- **艺术风格**: `{{ART_STYLE}}`
- **视觉特点**:
    - `{{VISUAL_FEATURE_1}}`: `{{VISUAL_FEATURE_1_DESC}}`
    - `{{VISUAL_FEATURE_2}}`: `{{VISUAL_FEATURE_2_DESC}}`

#### 5.1.2 场景/环境风格
- **环境类型**: `{{ENVIRONMENT_TYPE}}`
- **风格统一性**: `{{STYLE_CONSISTENCY}}`
- **氛围营造**: `{{ATMOSPHERE}}`

---

### 5.2 界面设计（UI Design）

#### 5.2.1 界面架构
- **布局模式**: `{{LAYOUT_MODE}}`
- **导航结构**: `{{NAVIGATION_STRUCTURE}}`
- **信息密度**: `{{INFO_DENSITY}}`

#### 5.2.2 核心界面
> **注**: 根据项目类型选择适用界面

| 界面类型 | 启用 | 布局描述 | 风格要点 |
|---------|------|---------|---------|
| 主界面 | `{{HOME_ENABLED}}` | `{{HOME_LAYOUT}}` | `{{HOME_STYLE}}` |
| 功能界面 | `{{FUNCTION_ENABLED}}` | `{{FUNCTION_LAYOUT}}` | `{{FUNCTION_STYLE}}` |
| 交互界面 | `{{INTERACTION_ENABLED}}` | `{{INTERACTION_LAYOUT}}` | `{{INTERACTION_STYLE}}` |
| 数据界面 | `{{DATA_ENABLED}}` | `{{DATA_LAYOUT}}` | `{{DATA_STYLE}}` |
| 设置界面 | `{{SETTINGS_ENABLED}}` | `{{SETTINGS_LAYOUT}}` | `{{SETTINGS_STYLE}}` |
| 其他界面 | `{{CUSTOM_ENABLED}}` | `{{CUSTOM_LAYOUT}}` | `{{CUSTOM_STYLE}}` |

#### 5.2.3 UI 组件规范
- **按钮样式**: `{{BUTTON_STYLE}}`
- **输入框样式**: `{{INPUT_STYLE}}`
- **列表样式**: `{{LIST_STYLE}}`
- **弹窗样式**: `{{MODAL_STYLE}}`
- **字体规范**: `{{FONT_SPEC}}`（字体家族/字号层级/行距）
- **间距规范**: `{{SPACING_SPEC}}`（统一间距单位）

---

### 5.3 空间/关卡设计（Space/Level Design）

> **适用**: 含场景/关卡/地图的项目（平台跳跃/解谜/探索类等）  
> **启用**: `{{SPACE_MODULE_ENABLED}}`

#### 5.3.1 空间结构
- **空间数量**: `{{SPACE_COUNT}}`
- **通用结构**（按`{{SPACE_COUNT}}`生成）：
    1. **`{{SPACE_NAME_1}}`**
        - 环境: `{{SPACE_ENV_1}}`
        - 特色: `{{SPACE_FEATURE_1}}`
        - 互动元素: `{{SPACE_INTERACTION_1}}`

    2. **`{{SPACE_NAME_2}}`**
        - 环境: `{{SPACE_ENV_2}}`
        - 特色: `{{SPACE_FEATURE_2}}`
        - 互动元素: `{{SPACE_INTERACTION_2}}`

#### 5.3.2 空间元素
- **可交互元素**: `{{INTERACTIVE_ELEMENTS}}`
- **障碍/限制**: `{{OBSTACLES}}`
- **引导元素**: `{{GUIDANCE_ELEMENTS}}`（如：路径指示/视觉引导）

---

### 5.4 角色/对象外观（Character/Object Appearance）

> **适用**: 含角色/可操作对象的项目  
> **启用**: `{{CHARACTER_MODULE_ENABLED}}`

#### 5.4.1 主要角色/对象
- **默认外观**: `{{DEFAULT_APPEARANCE}}`
- **变体系统**:
    - `{{VARIANT_1}}`: `{{VARIANT_DESC_1}}`
    - `{{VARIANT_2}}`: `{{VARIANT_DESC_2}}`

#### 5.4.2 次要角色/对象
- **NPC/辅助对象**: `{{SECONDARY_OBJECTS}}`
- **装饰元素**: `{{DECORATIVE_ELEMENTS}}`

---

### 5.5 图标与图形系统（Icon & Graphics System）

#### 5.5.1 功能图标
| 图标类型 | 样式描述 | 尺寸规范 |
|---------|---------|---------|
| 导航图标 | `{{NAV_ICON_STYLE}}` | `{{NAV_ICON_SIZE}}` |
| 功能图标 | `{{FUNC_ICON_STYLE}}` | `{{FUNC_ICON_SIZE}}` |
| 状态图标 | `{{STATUS_ICON_STYLE}}` | `{{STATUS_ICON_SIZE}}` |
| 其他图标 | `{{OTHER_ICON_STYLE}}` | `{{OTHER_ICON_SIZE}}` |

#### 5.5.2 内容图标
- **物品/道具**: `{{ITEM_ICON_STYLE}}`
- **资源/货币**: `{{RESOURCE_ICON_STYLE}}`
- **成就/徽章**: `{{BADGE_ICON_STYLE}}`

#### 5.5.3 图形规范
- **图标风格统一性**: `{{ICON_CONSISTENCY}}`
- **色彩编码规则**: `{{COLOR_CODING}}`（如：红色=警告/绿色=成功）

---

### 5.6 动效与反馈（Motion & Feedback）

#### 5.6.1 交互动效
- **点击反馈**: `{{CLICK_FEEDBACK}}`
- **过渡动画**: `{{TRANSITION_ANIMATION}}`
- **加载动画**: `{{LOADING_ANIMATION}}`
- **状态变化**: `{{STATE_CHANGE_ANIMATION}}`

#### 5.6.2 视觉反馈
- **成功反馈**: `{{SUCCESS_FEEDBACK}}`
- **错误反馈**: `{{ERROR_FEEDBACK}}`
- **进度反馈**: `{{PROGRESS_FEEDBACK}}`

#### 5.6.3 特殊效果
> **适用**: 含特效需求的项目  
> **启用**: `{{VFX_MODULE_ENABLED}}`

- **粒子效果**: `{{PARTICLE_EFFECTS}}`
- **光影效果**: `{{LIGHTING_EFFECTS}}`
- **屏幕效果**: `{{SCREEN_EFFECTS}}`

---

### 5.7 品牌标识（Brand Identity）

#### 5.7.1 主标识
- **Logo 文字**: `{{LOGO_TEXT}}`
- **Logo 图形**: `{{LOGO_GRAPHIC}}`
- **色彩规范**: `{{LOGO_COLORS}}`
- **使用场景**: `{{LOGO_USAGE}}`

#### 5.7.2 辅助标识
- **简化版**: `{{SIMPLIFIED_LOGO}}`
- **图标版**: `{{ICON_LOGO}}`
- **衍生标识**: `{{DERIVATIVE_LOGOS}}`
