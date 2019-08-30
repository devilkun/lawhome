# 合同范本

## 合同范本列表
<a id=合同范本列表> </a>
### 基本信息

**Path：** /contract/list

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
| pageSize | 是  |   |  每页显示条数 |

### 返回数据

<table>
  <thead class="ant-table-thead">
    <tr>
      <th key=name>名称</th><th key=type>类型</th><th key=required>是否必须</th><th key=default>默认值</th><th key=desc>备注</th><th key=sub>其他信息</th>
    </tr>
  </thead><tbody className="ant-table-tbody"><tr key=0-0><td key=0><span style="padding-left: 0px"><span style="color: #8c8a8a"></span> code</span></td><td key=1><span>string</span></td><td key=2>必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">返回码</span></td><td key=5></td></tr><tr key=0-1><td key=0><span style="padding-left: 0px"><span style="color: #8c8a8a"></span> msg</span></td><td key=1><span>string</span></td><td key=2>必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">返回码信息</span></td><td key=5></td></tr><tr key=0-2><td key=0><span style="padding-left: 0px"><span style="color: #8c8a8a"></span> data</span></td><td key=1><span>object</span></td><td key=2>必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">数据集</span></td><td key=5></td></tr><tr key=0-2-0><td key=0><span style="padding-left: 20px"><span style="color: #8c8a8a">├─</span> totalSize</span></td><td key=1><span>number</span></td><td key=2>必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">总条数</span></td><td key=5></td></tr><tr key=0-2-1><td key=0><span style="padding-left: 20px"><span style="color: #8c8a8a">├─</span> currentPage</span></td><td key=1><span>number</span></td><td key=2>必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">当前页码</span></td><td key=5></td></tr><tr key=0-2-2><td key=0><span style="padding-left: 20px"><span style="color: #8c8a8a">├─</span> pageSize</span></td><td key=1><span>number</span></td><td key=2>必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">每页显示条数</span></td><td key=5></td></tr><tr key=0-2-3><td key=0><span style="padding-left: 20px"><span style="color: #8c8a8a">├─</span> totalPage</span></td><td key=1><span>number</span></td><td key=2>必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">总页码</span></td><td key=5></td></tr><tr key=0-2-4><td key=0><span style="padding-left: 20px"><span style="color: #8c8a8a">├─</span> list</span></td><td key=1><span>object []</span></td><td key=2>必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">列表集</span></td><td key=5><p key=3><span style="font-weight: '700'">item 类型: </span><span>object</span></p></td></tr><tr key=0-2-4-0><td key=0><span style="padding-left: 40px"><span style="color: #8c8a8a">├─</span> id</span></td><td key=1><span>number</span></td><td key=2>必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">合同范本文章ID</span></td><td key=5></td></tr><tr key=0-2-4-1><td key=0><span style="padding-left: 40px"><span style="color: #8c8a8a">├─</span> title</span></td><td key=1><span>string</span></td><td key=2>必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">合同范本文章主标题</span></td><td key=5></td></tr><tr key=0-2-4-2><td key=0><span style="padding-left: 40px"><span style="color: #8c8a8a">├─</span> parent</span></td><td key=1><span>string</span></td><td key=2>必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">合同范本文章一级分类</span></td><td key=5></td></tr><tr key=0-2-4-3><td key=0><span style="padding-left: 40px"><span style="color: #8c8a8a">├─</span> create_time</span></td><td key=1><span>string</span></td><td key=2>必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">合同范本文章创建时间</span></td><td key=5></td></tr>
               </tbody>
              </table>

### 示例

```json
{
    "code": "200",
    "msg": "获取成功",
    "data": {
        "totalSize": 6,
        "currentPage": 1,
        "pageSize": 10,
        "totalPage": 1,
        "list": [
            {
                "id": 6,
                "title": "写字楼装修合同范本",
                "parent": "物业管理合同",
                "create_time": "2019-08-29"
            },
            {
                "id": 5,
                "title": "宅地基转让协议范本",
                "parent": "物业管理合同",
                "create_time": "2019-08-29"
            },
            {
                "id": 4,
                "title": "装饰装修合同三",
                "parent": "物业管理合同",
                "create_time": "2019-08-29"
            },
            {
                "id": 3,
                "title": "最新学校物业管理合同范本",
                "parent": "物业管理合同",
                "create_time": "2019-08-29"
            },
            {
                "id": 2,
                "title": "景观工程施工合同",
                "parent": "物业管理合同",
                "create_time": "2019-08-29"
            },
            {
                "id": 1,
                "title": "大厦物业管理合同范本",
                "parent": "物业管理合同",
                "create_time": "2019-08-29"
            }
        ]
    }
}
```

## 添加合同范本
<a id=添加合同范本> </a>
### 基本信息

**Path：** /contract/add

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
| tid | text  |  是 |    |  合同范本文章分类ID |
| title | text  |  是 |    |  合同范本文章主标题 |
| summary | text  |  是 |    |  合同范本文章简介 |
| picture_id | text  |  否 |    |  合同范本文章图片ID |
| content | text  |  是 |    |  合同正文 |



### 返回数据

<table>
  <thead class="ant-table-thead">
    <tr>
      <th key=name>名称</th><th key=type>类型</th><th key=required>是否必须</th><th key=default>默认值</th><th key=desc>备注</th><th key=sub>其他信息</th>
    </tr>
  </thead><tbody className="ant-table-tbody"><tr key=0-0><td key=0><span style="padding-left: 0px"><span style="color: #8c8a8a"></span> code</span></td><td key=1><span>string</span></td><td key=2>必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">返回码</span></td><td key=5></td></tr><tr key=0-1><td key=0><span style="padding-left: 0px"><span style="color: #8c8a8a"></span> msg</span></td><td key=1><span>string</span></td><td key=2>必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">返回信息</span></td><td key=5></td></tr>
               </tbody>
              </table>

### 示例

```json
{
    "code": "200",
    "msg": "添加合同范本成功"
}
```

## 编辑合同范本
<a id=编辑合同范本> </a>
### 基本信息

**Path：** /contract/edit

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
| id | text  |  是 |    |  合同范本文章ID |
| tid | text  |  是 |    |  合同范本文章分类ID |
| title | text  |  是 |    |  合同范本文章主标题 |
| summary | text  |  是 |    |  合同范本文章简介 |
| picture_id | text  |  否 |    |  合同范本文章图片 |
| content | text  |  是 |    |  合同正文 |



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
    "msg": "编辑合同范本成功"
}
```

## 删除合同范本
<a id=删除合同范本> </a>
### 基本信息

**Path：** /contract/delete

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
| id | 是  |   |  合同范本文章ID |

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
    "msg": "删除合同范本成功"
}
```

## 读取合同范本
<a id=读取合同范本> </a>
### 基本信息

**Path：** /contract/read

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
| id | 是  |   |  合同范本文章ID |

### 返回数据

<table>
  <thead class="ant-table-thead">
    <tr>
      <th key=name>名称</th><th key=type>类型</th><th key=required>是否必须</th><th key=default>默认值</th><th key=desc>备注</th><th key=sub>其他信息</th>
    </tr>
  </thead><tbody className="ant-table-tbody"><tr key=0-0><td key=0><span style="padding-left: 0px"><span style="color: #8c8a8a"></span> code</span></td><td key=1><span>string</span></td><td key=2>必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">返回码</span></td><td key=5></td></tr><tr key=0-1><td key=0><span style="padding-left: 0px"><span style="color: #8c8a8a"></span> msg</span></td><td key=1><span>string</span></td><td key=2>必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">返回码信息</span></td><td key=5></td></tr><tr key=0-2><td key=0><span style="padding-left: 0px"><span style="color: #8c8a8a"></span> data</span></td><td key=1><span>object</span></td><td key=2>必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">数据集</span></td><td key=5></td></tr><tr key=0-2-0><td key=0><span style="padding-left: 20px"><span style="color: #8c8a8a">├─</span> id</span></td><td key=1><span>number</span></td><td key=2>必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">合同范本文章ID</span></td><td key=5></td></tr><tr key=0-2-1><td key=0><span style="padding-left: 20px"><span style="color: #8c8a8a">├─</span> title</span></td><td key=1><span>string</span></td><td key=2>必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">合同范本文章主标题</span></td><td key=5></td></tr><tr key=0-2-2><td key=0><span style="padding-left: 20px"><span style="color: #8c8a8a">├─</span> summary</span></td><td key=1><span>string</span></td><td key=2>必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">合同范本文章简介</span></td><td key=5></td></tr><tr key=0-2-3><td key=0><span style="padding-left: 20px"><span style="color: #8c8a8a">├─</span> path</span></td><td key=1><span>string</span></td><td key=2>必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">合同范本文章路径</span></td><td key=5></td></tr><tr key=0-2-4><td key=0><span style="padding-left: 20px"><span style="color: #8c8a8a">├─</span> picture_id</span></td><td key=1><span>string</span></td><td key=2>必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">合同范本文章图片ID</span></td><td key=5></td></tr><tr key=0-2-5><td key=0><span style="padding-left: 20px"><span style="color: #8c8a8a">├─</span> content</span></td><td key=1><span>string</span></td><td key=2>必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">合同范本文章正文</span></td><td key=5></td></tr><tr key=0-2-6><td key=0><span style="padding-left: 20px"><span style="color: #8c8a8a">├─</span> tid</span></td><td key=1><span>string</span></td><td key=2>必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">合同范本文章分类ID</span></td><td key=5></td></tr>
               </tbody>
              </table>

### 示例

```json
{
    "code": "200",
    "msg": "获取成功",
    "data": {
        "id": 1,
        "title": "大厦物业管理合同范本",
        "summary": "大厦物业管理合同范本怎么写,书写大厦物业管理合同范本注意事项,标准大厦物业管理合同范本",
        "picture_id": 0,
        "path": null,
        "content": "甲方(委托方)：________________业主管理委员会\n\n地 址：________________邮码：____________电话：________\n\n法定代表人：________________职务：________\n\n乙方(受委托方)：____________ 物业管理公司\n\n地 址：________________邮码：____________电话：________\n\n法定代表人：________________职务：________\n\n为加强____________小区(大厦)的物业管理，保障房屋和公用设施的正常使用，为业主创造优美、整洁、安全、方便、舒适、文明的居住环境，根据____市物业管理方面的法规和政策，经双方友好协商，达成如下协议。 第一条 物业管理内容\n\n(一)甲方将位于____区____路的____范围内的物业委托给乙方实行统一管理，综合服务。\n\n(二)管理事项包括：\n\n1.房屋的使用、维修、养护;\n\n2.物业范围的公用设施、设备及场所(地)(消防、电梯、机电设备、路灯、走廊、自行车房、棚、园林绿化地、沟、渠、池、井、道路、停车场等)的使用、维修和管理;\n\n3.清洁卫生(不含垃圾运到中转站后的工作);\n\n4.公共生活秩序;\n\n5.文娱活动场所;\n\n6.便民服务网点及物业范围内所有营业场所;\n\n7.车辆行驶及停泊;\n\n8.物业档案管理;\n\n9.授权由物业管理公司管理的其他事项。\n\n第二条 委托物业管理形式\n\n承包经营、自负盈亏。\n\n第三条 物业管理期限\n\n委托管理期限为____年，自____年____月____日起到____年____月____日止。\n\n第四条 双方权利、义务\n\n(一)甲方权利、义务\n\n1.根据本合同规定甲方将住宅区委托乙方实施物业管理;\n\n2.监督乙方对公用设施专用基金的合理使用，并按公用设施专用基金管理办法拨付给乙方。\n\n3.按市政府规定的比例提供商业用房(总建设面积的0.5%)____平方米给乙方，按月租金____元租用，并负责办理使用手续;\n\n4.给乙方提供管理用房____平方米(其中办公用房____平方米，员工宿舍____平方米)，按月租金____元租用;\n\n5.负责向乙方提供本住宅区工程建设竣工资料一套并在乙方管理期满时予以收回;\n\n6.不得干涉乙方依法或依本合同规定内容所进行的管理和经营活动;\n\n7.对乙方的管理实施监督检查，每半年一次考核评定，如因乙方完不成第五条规定的目标和指标或管理不善造成重大经济损失，有权终止合同;\n\n8.负责确定本住宅区管理服务费收费标准;\n\n9.委托乙方对违反物业管理法规和规章制度以及业主公约的行为进行处理;包括予以罚款、责令停工、责令赔偿经济损失，以停水、停电等措施对无故不缴有关费用或拒不改正违章作业责任人进行催交、催改; 10.协助乙方做好宣传教育、文化活动，协调乙方与行政管理部门、业主间的关系;\n\n11.政策规定由甲方承担的其他责任。\n\n(二)乙方权利、义务：\n\n1.根据有关法律、法规，结合实际情况，制订本住宅区物业管理的各项规章制度;\n\n2.遵守各项管理法规和合同规定的要求，根据甲方授权，对本住宅区物业实施综合管理，确保实际管理目标、经济指标，并承担相应责任，自觉接受甲方检查监督;\n\n3.根据住宅区内大、中修的需要制订维修方案，报甲方审议通过后，从公用设施专用基金中领取所需的维修经费;\n\n4.接受甲方对经营管理过程中财务账目的监督并报告工作，每月向甲方和住宅区管理部门报送一次财务报表，每三个月向全体业主张榜公布一次管理费收支账目; 5.对住宅区的公用设施不得擅自占用和改变其使用功能，乙方如在住宅区内改扩建完善配套项目，须报甲方和有关部门批准后方可实施;\n\n6.乙方须本着高效、精干的原则在本住宅区设置管理机构和人员;\n\n7.建立本住宅区物业管理档案并负责及时记载有关变更情况;\n\n8.负责测算住宅区管理服务费收费标准并向甲方提供测算标准与依据，严格按照甲方审议通过的收费标准收取，不得擅自加价;\n\n9.有权依照甲方委托和业主公约的规定对违反业主公约和物业管理规章制度的行为进行处理;\n\n10.在管理期满时向甲方移交全部专用房屋及有关财产、全部物业管理档案及有关资料;\n\n11.开展卓有成效的社区文化活动和便民服务工作;\n\n12.有权选聘专营公司承担住宅区物业管理的专项业务并支付费用，但不得将住宅区物业管理的整体责任及利益转让给其他人或单位。\n\n第五条 物业管理目标和经济指标\n\n(一)各项管理指标执行物业行政主管部门规定的各项标准，要求住宅区在乙方接管后____年内达到____标准。\n\n(二)确保年完成各项收费指标____万元，合理支出____万元，乙方可提成所收取管理费的____%作为经营收入。\n\n第六条 风险抵押\n\n(一)乙方在合同签订之日起3日内向甲方一次性支付人民币____元，作为风险抵押金。\n\n(二)乙方完成合同规定的管理目标和经济指标，甲方在合同期满后3日内退还全部抵押金及银行活期存款利息。\n\n(三)如由于甲方过错致使本合同不能履行，由甲方双倍返还抵押金并赔偿乙方经济损失。\n\n(四)如由于乙方过错致使合同不能履行，乙方无权要求返还抵押金，并应赔偿甲方经济损失。\n\n第七条 奖罚措施\n\n(一)在各项管理目标、经济指标全面完成的前提下，管理费如有节余，甲方按节余额____%奖励乙方。\n\n(二)如该住宅区被评为全国、省、市文明住宅小区，甲方分别奖励乙方人民币____元(全国)、____元(省)、____元(市);获得上级部门单项奖或有关荣誉的奖金另订;如在乙方管理期间，由乙方获得的文明小区称号被上级部门取消，则乙方应全部返还上述奖金及银行活期存款利息。\n\n(三)如果甲方不完成应负的合同责任，由此而影响乙方的承包管理目标和经济指标，或给乙方造成直接经济损失，甲方应当给予补偿或承担相应责任。\n\n(四)如果乙方没有完成合同责任或管理目标和经济指标，甲方应当责成乙方限期改正，情节严重的处以人民币____至____元的罚款，直至终止合同，经济损失由乙方承担。 (五)由乙方管理不善或重大失误，造成住户经济损失或生活严重不便的，应当赔偿甲方或业主及使用人的经济损失。\n\n第八条 合同更改、补充与终止\n\n(一)经双方协商一致，可对本合同条款进行修订更改或补充，以书面合同为准。\n\n(二)合同规定的管理期满，本合同自然终止，各方如欲续订合同，须于期满前3个月向对方提出书面意见。\n\n(三)合同终止后，乙方可参加甲方的管理招标并在同等条件下优先承包管理。\n\n第九条 其他事项\n\n(一)本合同执行期间，如遇不可抗拒的自然灾害(台风、洪水、地震等)，造成经济损失的，双方应相互体谅，共同协商、合理分摊。\n\n(二)本合同自签订之日起生效;附件1、2、3、4……为合同的有效组成部分。 (三)本合同正本一式三份，甲、乙双方和物业管理部门各执一份，具有同等法律约束力。\n\n(四)双方如对合同发生争议，协商不成的，诉请人民法院解决。\n\n甲方：____________________\n\n代表人：________________\n\n____年____月____日\n\n乙方：____________________\n\n代表人：________________\n\n____年____月____日",
        "tid": 10
    }
}
```
