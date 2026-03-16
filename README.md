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