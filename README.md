### YamlScriptHelper

yaml(yml)文件助手，提供树视图，JSON视图查看yaml文件。<br/>
可以配置yaml key 备注，在树视图中展示备注。<br/>
可以在树视图中，复制key，value，key-value，node path。<br/>
可以从树视图跳转到yaml文件对应行

本项目参考了以下项目：

Json-Assistant : https://github.com/MemoryZy/Json-Assistant

Maven Helper : https://github.com/krasa/MavenHelper/

YamlHelper: https://github.com/LerDer/YamlHelper/tree/master

### 安装插件

您可以通过以下方式安装 YamlHelper 插件：

1.  **通过 IntelliJ IDEA Marketplace (推荐)**:
    *   打开 IntelliJ IDEA。
    *   进入 `File -> Settings -> Plugins` (Windows/Linux) 或 `IntelliJ IDEA -> Preferences -> Plugins` (macOS)。
    *   切换到 `Marketplace` 标签页。
    *   搜索 `YamlHelper`。
    *   点击 `Install` 并重启 IDE。

2.  **通过本地 .zip 文件安装**:
    *   从插件发布页面下载最新的 `.zip` 包。
    *   打开 IntelliJ IDEA。
    *   进入 `File -> Settings -> Plugins` (Windows/Linux) 或 `IntelliJ IDEA -> Preferences -> Plugins` (macOS)。
    *   点击齿轮图标，选择 `Install Plugin from Disk...`。
    *   选择下载的 `.zip` 文件并重启 IDE。

### 主要功能

*   **YAML 文件树视图**：以树状结构清晰展示 YAML 文件内容。
*   **JSON 视图**：将 YAML 文件转换为 JSON 格式查看。
*   **Key/Value 备注**：可配置 YAML Key 的备注，并在树视图中显示。
*   **便捷复制**：在树视图中方便地复制 Key、Value、Key-Value 对或节点路径。
*   **代码跳转**：从树视图快速跳转到 YAML 文件中的对应行。
*   **快速生成 YAML 模板**：通过 `File -> New -> Generate YAML Template` (或在项目视图右键菜单 `New -> Generate YAML Template`) 快速创建一个预设的 YAML 脚本文件。
*   **YAML 脚本标签提示**：在编辑 YAML 文件时，自动提示常用的脚本标签 (如 `description`, `input`, `output`, `steps`, `set`, `call` 等)，提高编写效率。

### 兼容性

本插件兼容 IntelliJ IDEA 2024.3 Community Edition 。

### 使用方法：

#### 快速生成 YAML 模板

1.  在项目视图中，右键点击目标目录或父级目录。
2.  选择 `New -> Generate YAML Template`。
3.  输入文件名，插件将自动生成一个包含预设脚本结构的 YAML 文件，并在编辑器中打开它。

#### YAML 脚本标签提示

在 `.yaml` 或 `.yml` 文件中编写内容时，当您输入可能匹配预定义脚本标签的字符时，IDE 会自动弹出提示列表，您可以从中选择合适的标签。


#### 树视图

![](/pic/Snipaste_2025-03-07_13-25-15.png)

#### JSON视图

![](/pic/Snipaste_2025-03-07_13-25-01.png)

#### 右键菜单

![](/pic/Snipaste_2025-03-07_12-07-54.png)

#### 定位

![](/pic/16.gif)

#### 配置文件示例 

keys_mark.yaml

```yaml
name: 名称
serviceCode: 服务编码
serviceScene: 服务场景
tranCode: 交易码
mock: 是否mock
active: 环境
url: 地址
username: 用户名
password: 密码
driverClassName: 驱动
db-type: 数据库类型
cache: 是否缓存
prefix: 前缀
static-locations: 静态资源
port: 端口
sensitive-column: 敏感字段
db-name: 数据库名
queryConfig: 查询字段
mapper-locations: mapper路径
map-underscore-to-camel-case: 下划线转驼峰
encodeKey: 加密key
mocks: 是否mock
element: 元素
profiles: 配置
```

![](/pic/Snipaste_2025-03-07_13-31-34.png)

![](/pic/Snipaste_2025-03-07_13-34-29.png)

---

**注意**: 上述截图主要展示插件原有的核心功能。新增的“快速生成 YAML 模板”和“YAML 脚本标签提示”功能旨在提升 YAML 脚本文件的编写效率。
