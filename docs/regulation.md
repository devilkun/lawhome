# 法律法规

## 法律法规列表
<a id=法律法规列表> </a>
### 基本信息

**Path：** /regulation/list

**Method：** GET

**接口描述：**


### 请求参数
**Headers**

| 参数名称  | 参数值  |  是否必须 | 示例  | 备注  |
| ------------ | ------------ | ------------ | ------------ | ------------ |
| web-token  |   | 是  |   |  token 令牌 |

**Query**

| 参数名称  |  是否必须 | 示例  | 备注  |
| ------------ | ------------ | ------------ | ------------ |
| search | 否  |   |  搜索项文本 |
| page | 否  |   |  当前页码 |
| pageSize | 否  |   |  每页显示条数 |

### 返回数据

<table>
  <thead class="ant-table-thead">
    <tr>
      <th key=name>名称</th><th key=type>类型</th><th key=required>是否必须</th><th key=default>默认值</th><th key=desc>备注</th><th key=sub>其他信息</th>
    </tr>
  </thead><tbody className="ant-table-tbody"><tr key=0-0><td key=0><span style="padding-left: 0px"><span style="color: #8c8a8a"></span> code</span></td><td key=1><span>string</span></td><td key=2>必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">返回码</span></td><td key=5></td></tr><tr key=0-1><td key=0><span style="padding-left: 0px"><span style="color: #8c8a8a"></span> msg</span></td><td key=1><span>string</span></td><td key=2>必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">返回码信息</span></td><td key=5></td></tr><tr key=0-2><td key=0><span style="padding-left: 0px"><span style="color: #8c8a8a"></span> data</span></td><td key=1><span>object</span></td><td key=2>必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">数据集</span></td><td key=5></td></tr><tr key=0-2-0><td key=0><span style="padding-left: 20px"><span style="color: #8c8a8a">├─</span> totalSize</span></td><td key=1><span>number</span></td><td key=2>必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">总条数</span></td><td key=5></td></tr><tr key=0-2-1><td key=0><span style="padding-left: 20px"><span style="color: #8c8a8a">├─</span> currentPage</span></td><td key=1><span>number</span></td><td key=2>必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">当前页面</span></td><td key=5></td></tr><tr key=0-2-2><td key=0><span style="padding-left: 20px"><span style="color: #8c8a8a">├─</span> pageSize</span></td><td key=1><span>number</span></td><td key=2>必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">每页显示条数</span></td><td key=5></td></tr><tr key=0-2-3><td key=0><span style="padding-left: 20px"><span style="color: #8c8a8a">├─</span> totalPage</span></td><td key=1><span>number</span></td><td key=2>必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">总页码</span></td><td key=5></td></tr><tr key=0-2-4><td key=0><span style="padding-left: 20px"><span style="color: #8c8a8a">├─</span> list</span></td><td key=1><span>object []</span></td><td key=2>必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">列表集</span></td><td key=5><p key=3><span style="font-weight: '700'">item 类型: </span><span>object</span></p></td></tr><tr key=0-2-4-0><td key=0><span style="padding-left: 40px"><span style="color: #8c8a8a">├─</span> id</span></td><td key=1><span>number</span></td><td key=2>必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">法律法规文章ID</span></td><td key=5></td></tr><tr key=0-2-4-1><td key=0><span style="padding-left: 40px"><span style="color: #8c8a8a">├─</span> title</span></td><td key=1><span>string</span></td><td key=2>必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">法律法规主标题</span></td><td key=5></td></tr><tr key=0-2-4-2><td key=0><span style="padding-left: 40px"><span style="color: #8c8a8a">├─</span> parent</span></td><td key=1><span>string</span></td><td key=2>必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">法律法规一级分类</span></td><td key=5></td></tr><tr key=0-2-4-3><td key=0><span style="padding-left: 40px"><span style="color: #8c8a8a">├─</span> create_time</span></td><td key=1><span>string</span></td><td key=2>必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">法律法规创建时间</span></td><td key=5></td></tr>
               </tbody>
              </table>

### 示例

```json
{
    "code": "200",
    "msg": "获取成功",
    "data": {
        "totalSize": 4,
        "currentPage": 1,
        "pageSize": 10,
        "totalPage": 1,
        "list": [
            {
                "id": 4,
                "title": "水利、水电行业工程勘察设计资格分级标准",
                "parent": "民商法类",
                "create_time": "2019-08-29"
            },
            {
                "id": 3,
                "title": "水利部关于加强水利认证认可工作的若干意见",
                "parent": "民商法类",
                "create_time": "2019-08-29"
            },
            {
                "id": 2,
                "title": "水利部关于加强中小型水利工程建设管理防范廉政风险的指导意见",
                "parent": "民商法类",
                "create_time": "2019-08-29"
            },
            {
                "id": 1,
                "title": "水利部关于京津风沙源治理工程水利水保项目建设管理的指导意见",
                "parent": "民商法类",
                "create_time": "2019-08-29"
            }
        ]
    }
}
```

## 添加法律法规
<a id=添加法律法规> </a>
### 基本信息

**Path：** /regulation/add

**Method：** POST

**接口描述：**


### 请求参数
**Headers**

| 参数名称  | 参数值  |  是否必须 | 示例  | 备注  |
| ------------ | ------------ | ------------ | ------------ | ------------ |
| Content-Type  |  application/x-www-form-urlencoded | 是  |   |   |
| web-token  |   | 是  |   |  token 令牌 |

**Body**

| 参数名称  | 参数类型  |  是否必须 | 示例  | 备注  |
| ------------ | ------------ | ------------ | ------------ | ------------ |
| tid | number  |  是 |    |  法律法规分类ID |
| title | text  |  是 |    |  法律法规主标题 |
| summary | text  |  是 |    |  法律法规简介 |
| issue_unit | text  |  是 |    |  法律法规颁布单位 |
| doc_number | text  |  是 |    |  法律法规文号 |
| issue_time | text  |  是 |    |  法律法规颁布时间 |
| implementation_time | text  |  是 |    |  法律法规实施时间 |
| timeliness | text  |  是 |    |  法律法规时效性 |
| effective_level | text  |  是 |    |  法律法规效力级别 |
| content | text  |  是 |    |  法律法规正文内容 |



### 返回数据

<table>
  <thead class="ant-table-thead">
    <tr>
      <th key=name>名称</th><th key=type>类型</th><th key=required>是否必须</th><th key=default>默认值</th><th key=desc>备注</th><th key=sub>其他信息</th>
    </tr>
  </thead><tbody className="ant-table-tbody"><tr key=0-0><td key=0><span style="padding-left: 0px"><span style="color: #8c8a8a"></span> code</span></td><td key=1><span>string</span></td><td key=2>必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">返回码</span></td><td key=5></td></tr><tr key=0-1><td key=0><span style="padding-left: 0px"><span style="color: #8c8a8a"></span> msg</span></td><td key=1><span>string</span></td><td key=2>必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">返回码信息</span></td><td key=5></td></tr>
               </tbody>
              </table>

### 示例

```json
{
    "code": "200",
    "msg": "添加法律法规成功"
}
```

## 编辑法律法规
<a id=编辑法律法规> </a>
### 基本信息

**Path：** /regulation/edit

**Method：** POST

**接口描述：**


### 请求参数
**Headers**

| 参数名称  | 参数值  |  是否必须 | 示例  | 备注  |
| ------------ | ------------ | ------------ | ------------ | ------------ |
| Content-Type  |  application/x-www-form-urlencoded | 是  |   |   |
| web-token  |   | 是  |   |  token 令牌 |
**Body**

| 参数名称  | 参数类型  |  是否必须 | 示例  | 备注  |
| ------------ | ------------ | ------------ | ------------ | ------------ |
| id | number  |  是 |    |  法律法规文章ID |
| tid | number  |  是 |    |  法律法规分类ID |
| title | text  |  是 |    |  法律法规主标题 |
| summary | text  |  是 |    |  法律法规简介 |
| issue_unit | text  |  是 |    |  法律法规颁布单位 |
| doc_number | text  |  是 |    |  法律法规文号 |
| issue_time | text  |  是 |    |  法律法规颁布时间 |
| implementation_time | text  |  是 |    |  法律法规实施时间 |
| timeliness | text  |  是 |    |  法律法规时效性 |
| effective_level | text  |  是 |    |  法律法规效力级别 |
| content | text  |  是 |    |  法律法规正文内容 |



### 返回数据

<table>
  <thead class="ant-table-thead">
    <tr>
      <th key=name>名称</th><th key=type>类型</th><th key=required>是否必须</th><th key=default>默认值</th><th key=desc>备注</th><th key=sub>其他信息</th>
    </tr>
  </thead><tbody className="ant-table-tbody"><tr key=0-0><td key=0><span style="padding-left: 0px"><span style="color: #8c8a8a"></span> code</span></td><td key=1><span>string</span></td><td key=2>必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">返回码</span></td><td key=5></td></tr><tr key=0-1><td key=0><span style="padding-left: 0px"><span style="color: #8c8a8a"></span> msg</span></td><td key=1><span>string</span></td><td key=2>必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">返回码信息</span></td><td key=5></td></tr>
               </tbody>
              </table>

### 示例

```json
{
    "code": "200",
    "msg": "编辑法律法规成功"
}
```

## 删除法律法规
<a id=删除法律法规> </a>
### 基本信息

**Path：** /regulation/delete

**Method：** GET

**接口描述：**


### 请求参数
**Headers**

| 参数名称  | 参数值  |  是否必须 | 示例  | 备注  |
| ------------ | ------------ | ------------ | ------------ | ------------ |
| web-token  |   | 是  |   |  token 令牌 |

**Query**

| 参数名称  |  是否必须 | 示例  | 备注  |
| ------------ | ------------ | ------------ | ------------ |
| id | 是  |   |  法律法规文章ID |

### 返回数据

<table>
  <thead class="ant-table-thead">
    <tr>
      <th key=name>名称</th><th key=type>类型</th><th key=required>是否必须</th><th key=default>默认值</th><th key=desc>备注</th><th key=sub>其他信息</th>
    </tr>
  </thead><tbody className="ant-table-tbody"><tr key=0-0><td key=0><span style="padding-left: 0px"><span style="color: #8c8a8a"></span> code</span></td><td key=1><span>string</span></td><td key=2>必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">返回码</span></td><td key=5></td></tr><tr key=0-1><td key=0><span style="padding-left: 0px"><span style="color: #8c8a8a"></span> msg</span></td><td key=1><span>string</span></td><td key=2>必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">返回码信息</span></td><td key=5></td></tr>
               </tbody>
              </table>

### 示例

```json
{
    "code": "200",
    "msg": "删除法律法规成功"
}
```

## 读取法律法规
<a id=读取法律法规> </a>
### 基本信息

**Path：** /regulation/read

**Method：** GET

**接口描述：**


### 请求参数
**Headers**

| 参数名称  | 参数值  |  是否必须 | 示例  | 备注  |
| ------------ | ------------ | ------------ | ------------ | ------------ |
| web-token  |   | 是  |   |  token 令牌 |

**Query**

| 参数名称  |  是否必须 | 示例  | 备注  |
| ------------ | ------------ | ------------ | ------------ |
| id | 是  |   |  法律法规文章ID |

### 返回数据

<table>
  <thead class="ant-table-thead">
    <tr>
      <th key=name>名称</th><th key=type>类型</th><th key=required>是否必须</th><th key=default>默认值</th><th key=desc>备注</th><th key=sub>其他信息</th>
    </tr>
  </thead><tbody className="ant-table-tbody"><tr key=0-0><td key=0><span style="padding-left: 0px"><span style="color: #8c8a8a"></span> code</span></td><td key=1><span>string</span></td><td key=2>必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">返回码</span></td><td key=5></td></tr><tr key=0-1><td key=0><span style="padding-left: 0px"><span style="color: #8c8a8a"></span> msg</span></td><td key=1><span>string</span></td><td key=2>必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">返回码信息</span></td><td key=5></td></tr><tr key=0-2><td key=0><span style="padding-left: 0px"><span style="color: #8c8a8a"></span> data</span></td><td key=1><span>object</span></td><td key=2>必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">数据集</span></td><td key=5></td></tr><tr key=0-2-0><td key=0><span style="padding-left: 20px"><span style="color: #8c8a8a">├─</span> id</span></td><td key=1><span>number</span></td><td key=2>必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">法律法规文章ID</span></td><td key=5></td></tr><tr key=0-2-1><td key=0><span style="padding-left: 20px"><span style="color: #8c8a8a">├─</span> title</span></td><td key=1><span>string</span></td><td key=2>必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">法律法规文章标题</span></td><td key=5></td></tr><tr key=0-2-2><td key=0><span style="padding-left: 20px"><span style="color: #8c8a8a">├─</span> summary</span></td><td key=1><span>string</span></td><td key=2>必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">法律法规文章简介</span></td><td key=5></td></tr><tr key=0-2-3><td key=0><span style="padding-left: 20px"><span style="color: #8c8a8a">├─</span> issue_unit</span></td><td key=1><span>string</span></td><td key=2>必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">法律法规颁布单位</span></td><td key=5></td></tr><tr key=0-2-4><td key=0><span style="padding-left: 20px"><span style="color: #8c8a8a">├─</span> doc_number</span></td><td key=1><span>string</span></td><td key=2>必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">法律法规文号</span></td><td key=5></td></tr><tr key=0-2-5><td key=0><span style="padding-left: 20px"><span style="color: #8c8a8a">├─</span> issue_time</span></td><td key=1><span>string</span></td><td key=2>必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">法律法规颁布时间</span></td><td key=5></td></tr><tr key=0-2-6><td key=0><span style="padding-left: 20px"><span style="color: #8c8a8a">├─</span> implementation_time</span></td><td key=1><span>string</span></td><td key=2>必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">法律法规实施时间</span></td><td key=5></td></tr><tr key=0-2-7><td key=0><span style="padding-left: 20px"><span style="color: #8c8a8a">├─</span> timeliness</span></td><td key=1><span>string</span></td><td key=2>必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">法律法规时效性</span></td><td key=5></td></tr><tr key=0-2-8><td key=0><span style="padding-left: 20px"><span style="color: #8c8a8a">├─</span> effective_level</span></td><td key=1><span>string</span></td><td key=2>必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">法律法规效力级别</span></td><td key=5></td></tr><tr key=0-2-9><td key=0><span style="padding-left: 20px"><span style="color: #8c8a8a">├─</span> content</span></td><td key=1><span>string</span></td><td key=2>必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">法律法规正文内容</span></td><td key=5></td></tr><tr key=0-2-10><td key=0><span style="padding-left: 20px"><span style="color: #8c8a8a">├─</span> tid</span></td><td key=1><span>number</span></td><td key=2>必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">法律法规分类ID</span></td><td key=5></td></tr>
               </tbody>
              </table>

### 示例

```json
{
    "code": "200",
    "msg": "获取成功",
    "data": {
        "id": "1",
        "title": "水利部关于京津风沙源治理工程水利水保项目建设管理的指导意见",
        "summary": "为进一步加强和规范这项工程中水利水保项目的管理，确保小流域综合治理、水源及节水灌溉工程建设的顺利实施，充分发挥水利水保工程在防沙治沙中的作用，我部根据《京津风沙源治理工程建设管理办法》和国家基本建设管理的有关规定，结合水利水保工程的特点，提出以下意见。",
        "issue_unit": "水利部",
        "doc_number": "水保[2003]360号",
        "issue_time": "2003-08-19",
        "implementation_time": "2003-08-19",
        "timeliness": "现行有效",
        "effective_level": "部门规范性文件",
        "content": "一、工程建设的原则\n\n(一)坚持综合治理的防治路线。以小流域为单元，因地制宜，因害设防，工程、生物和农业技术措施科学配置，生态、经济和社会效益统筹兼顾，形成多目标、多功能、高效益的水土保持综合防沙治沙体系。\n\n(二)坚持与区域经济发展相结合。根据当地资源优势和区域经济社会发展规划，调整项目区土地利用结构，合理安排农林牧各业生产，有效利用水土资源，培育主导产业，促进传统粗放型农牧业向现代集约高效型农牧业转变。\n\n(三)坚持人工治理与生态自我修复相结合。通过小流域综合治理、水源及节水灌溉工程建设，改善农村生产生活条件，发展集约高效农牧业，为大面积退耕和封育创造条件。加强封禁管护，充分依靠生态的自我修复能力，恢复植被，改善生态环境。\n\n(四)坚持水资源合理配置和有效利用。根据当地水资源条件，合理安排生产、生活和生态用水，要充分利用天然降水，合理开采地下水，积极推广集雨节灌技术。水源与节水灌溉工程建设要与防沙治沙、发展当地经济有机结合起来，与小流域综合治理、基本草场建设相配套，发挥工程整体效益。\n\n(五)坚持群众参与、多元化投入的机制。按照“谁投资、谁所有、谁受益、谁管护”的原则，大力推行承包、拍卖、租赁和股份合作等多种治理开发形式，调动广大群众和社会各界积极参与工程建设与管理。\n\n(六)坚持预防为主，保护优先。认真贯彻执行《水土保持法》，把预防保护工作放在首位，依法保护和合理利用水土资源，坚决遏制新的人为水土流失。\n\n二、前期工作\n\n(一)县级水利水保部门应根据省级计划部门批准的年度工程实施方案和有关技术规范要求，编制工程的初步设计报告。初步设计必须由具有相应设计资质或水土保持方案编制资质的单位承担。\n\n(二)水利水保项目的初步设计中，深水井(井深100米以上)的初步设计由省级水行政主管部门审查，小流域治理、节水灌溉、浅水井及其他小型水源工程的初步设计由省级水行政主管部门或委托地市级水行政主管部门审查，报省级计划主管部门审批。初步设计未经批准，不得开工建设和下达年度计划。\n\n(三)小流域治理初步设计按照我部颁发的《水土保持建设项目前期工作暂行规定》和《水土保持综合治理技术规范》(GB/T 16453.1～6-1996)等有关技术规范编制，水源与节水灌溉工程的初步设计按照《机井技术规范》(SL256-2000)、《节水灌溉技术规范》(SL207-98)等有关技术规范编制。初步设计要图、文、表齐全，各项建设任务要落实到山头地块，达到施工要求。小流域治理工程总体布局及规划图按照1：1000～1：1万的比例尺绘制，其它图件绘制依据《水利水电工程制图标准?水土保持图》(SL73.6-2001)进行。\n\n水源工程建设以水窖、塘坝、浅水井等小型水利水保工程为主，不得盲目大规模开采地下水。对确需建设机井，开采地下水发展节水灌溉的，必须按照《建设项目水资源论证管理办法》和水利部“关于做好建设项目水资源论证工作的通知”(水资源[2002]145号文)精神，做好前期论证工作，并依据《取水许可制度实施条例》和水利部“关于进一步加强取水许可监督管理工作的通知”(水资源[2002]40号文)精神，办理取水许可证。\n\n根据国家计划下达的要求，水源和节水灌溉工程统一按工程处数折算工程量。水窖、蓄水池和塘坝等小型拦蓄水源工程，以拦蓄总库容每200立方米计水源工程一处，节水灌溉工程以灌溉面积每3公顷计节水灌溉工程一处。\n\n(四)初步设计的投资估算和概算，执行我部颁布的《水利水电工程设计概(估)算编制规定》、《水土保持生态建设工程概(估)算编制规定》、《水土保持生态建设工程概算定额》。\n\n(五)京津风沙源治理工程水利水保科技支撑项目按基本建设程序管理，明确科技支撑单位，由省级水行政主管部门组织有关科研单位编制可行性研究报告，经水利部审批后申请列入工程建设年度计划。\n\n三、项目建设管理\n\n(一)水利水保项目实施要严格按照国家的有关要求，建立健全领导责任制，积极推行项目法人责任制、工程建设监理制、招标投标制、资金报账制和 群众投工承诺制等管理制度。\n\n(二)水利水保项目的责任主体是县级水利水保部门，对项目建设的全过程负总责。其主要职责为：负责落实工程建设计划;负责设计、施工和工程建设监理的组织实施;负责工程质量、进度、资金管理;负责项目的监督检查和工程自验。\n\n(三)因地制宜地推行工程招投标制，对以中央投资为主，投资规模超过50万元的大型沟道工程、集中连片机械施工、机井建设、节水灌溉等单项工程，应通过招标投标选择施工单位。优先选择水平高、技术强、信誉好的施工队伍进行施工建设，确保工程进度快、质量好。\n\n承建单位须具备相应的资质和施工能力，严禁转包、分包。\n\n(四)水利水保项目全面推行工程建设监理制。承担工程建设监理的单位必须具有水土保持生态建设工程监理资质，监理工作执行我部颁发的《水土保持生态建设工程监理管理暂行办法》。\n\n(五)推行群众投工承诺制。在初步设计阶段，应把所需群众投工及投工数量向项目区群众公开，征求群众意见。项目区三分之二以上群众同意，并由村民委员会以书面形式向县级主管部门做出承诺，经县级政府批准后，方可申报立项并实施。\n\n组织群众投工一般只在项目实施受益村进行，不得跨村投工或平调使用劳动力;确需跨村投工的采取借工或换工的形式组织进行。\n\n(六)严格按设计施工，不得随意变更设计。如确需变更，属于项目调整、建设规模变化、概算变更等重大变动，需经原设计单位同意，报原审批单位批准;不涉及总投资和治理面积、不降低质量、不影响功能的一般性变更，经原设计单位同意，报项目责任主体备案。\n\n(七)坚持走科技治沙之路。要切实加强技术培训和技术引进，不断总结、借鉴和推广各地防沙治沙的先进经验，提高项目建设的科技含量。科技支撑项目要对工程实施起示范带动作用。\n\n(八)项目验收实行阶段(年度)验收和竣工验收。阶段验收和竣工验收均按县级自验、省级复验和国家核查三个层次进行。县级自验由县水行政主管部门负责组织，对各项治理措施的数量、质量逐项、逐地块地进行验收，提出验收报告。自验结束后报省级水行政主管部门申请复验，复验由省级水行政主管部门组织进行，邀请省级计划、林业部门参加。复验以县为单位，逐条小流域进行(验收抽样比例见附表1)，对大型沟道工程、集中连片机械施工工程要逐个进行验收。复验后省级水行政主管部门将复验报告报水利部，由国家林业局牵头组织有关部委核查。\n\n竣工验收分单项工程竣工验收和项目总体竣工验收。单项工程竣工验收由省级水行政主管部门主持，项目总体竣工验收由国家林业局牵头有关部委进行。\n\n(九)小流域综合治理验收执行《水土保持综合治理?验收规范》;机井及节水灌溉工程按照机井、节水灌溉等有关技术规范进行验收(阶段验收和竣工验收成果表见附表2-3)。\n\n(十)国家和省级检查验收时，项目建设单位应提供下列资料：项目建设工作总结;申请验收报告;建设任务和投资计划完成情况表;项目初步设计文件、图表和现状图;项目竣工财务决算报表;审计部门的资金审计报告;监理单位的监理报告、项目技术档案资料。\n\n四、工程管护\n\n(一)各地要将治理后的土地和水利水保设施及时纳入规范管理，工程项目竣工验收合格后，按原有土地权属关系及国家有关政策，尽快落实治理成果的产权或使用权，并由县级人民政府核发有关权属证明。\n\n(二)按照“谁治理、谁管护、谁受益”的原则，积极探索灵活的、有效的管护机制，鼓励社会各界，企业、社团等参与水利水保项目建设，尽快落实工程管护措施，把管护任务承包到户、到人，保证工程建设成果得以巩固，长期发挥效益。\n\n附表1：水利水保措施省级复查验收抽样比例表(略)\n\n附表2：水利水保措施阶段验收表(略)\n\n附表3：水利水保措施竣工验收表(略)",
        "tid": 6
    }
}
```
