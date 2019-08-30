# 法律文书

## 法律文书列表
<a id=法律文书列表> </a>
### 基本信息

**Path：** /instrument/list

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
  </thead><tbody className="ant-table-tbody"><tr key=0-0><td key=0><span style="padding-left: 0px"><span style="color: #8c8a8a"></span> code</span></td><td key=1><span>string</span></td><td key=2>必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">返回码</span></td><td key=5></td></tr><tr key=0-1><td key=0><span style="padding-left: 0px"><span style="color: #8c8a8a"></span> msg</span></td><td key=1><span>string</span></td><td key=2>必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">返回码信息</span></td><td key=5></td></tr><tr key=0-2><td key=0><span style="padding-left: 0px"><span style="color: #8c8a8a"></span> data</span></td><td key=1><span>object</span></td><td key=2>必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">数据集</span></td><td key=5></td></tr><tr key=0-2-0><td key=0><span style="padding-left: 20px"><span style="color: #8c8a8a">├─</span> totalSize</span></td><td key=1><span>number</span></td><td key=2>必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">总条数</span></td><td key=5></td></tr><tr key=0-2-1><td key=0><span style="padding-left: 20px"><span style="color: #8c8a8a">├─</span> currentPage</span></td><td key=1><span>number</span></td><td key=2>必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">当前页码</span></td><td key=5></td></tr><tr key=0-2-2><td key=0><span style="padding-left: 20px"><span style="color: #8c8a8a">├─</span> pageSize</span></td><td key=1><span>number</span></td><td key=2>必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">每页显示条数</span></td><td key=5></td></tr><tr key=0-2-3><td key=0><span style="padding-left: 20px"><span style="color: #8c8a8a">├─</span> totalPage</span></td><td key=1><span>number</span></td><td key=2>必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">总页码</span></td><td key=5></td></tr><tr key=0-2-4><td key=0><span style="padding-left: 20px"><span style="color: #8c8a8a">├─</span> list</span></td><td key=1><span>object []</span></td><td key=2>必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">列表集</span></td><td key=5><p key=3><span style="font-weight: '700'">item 类型: </span><span>object</span></p></td></tr><tr key=0-2-4-0><td key=0><span style="padding-left: 40px"><span style="color: #8c8a8a">├─</span> id</span></td><td key=1><span>number</span></td><td key=2>必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">法律文书文章ID</span></td><td key=5></td></tr><tr key=0-2-4-1><td key=0><span style="padding-left: 40px"><span style="color: #8c8a8a">├─</span> title</span></td><td key=1><span>string</span></td><td key=2>必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">法律文书文章主标题</span></td><td key=5></td></tr><tr key=0-2-4-2><td key=0><span style="padding-left: 40px"><span style="color: #8c8a8a">├─</span> parent</span></td><td key=1><span>string</span></td><td key=2>必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">法律文书文章分类ID</span></td><td key=5></td></tr><tr key=0-2-4-3><td key=0><span style="padding-left: 40px"><span style="color: #8c8a8a">├─</span> create_time</span></td><td key=1><span>string</span></td><td key=2>必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">法律文书文章创建时间</span></td><td key=5></td></tr>
               </tbody>
              </table>

### 示例

```json
{
    "code": "200",
    "msg": "获取成功",
    "data": {
        "totalSize": 7,
        "currentPage": 1,
        "pageSize": 10,
        "totalPage": 1,
        "list": [
            {
                "id": 7,
                "title": "取保候审申请书",
                "parent": "民事诉讼",
                "create_time": "2019-08-29"
            },
            {
                "id": 6,
                "title": "股权转让协议",
                "parent": "民事诉讼",
                "create_time": "2019-08-29"
            },
            {
                "id": 5,
                "title": "民间借贷纠纷起诉状范文",
                "parent": "民事诉讼",
                "create_time": "2019-08-29"
            },
            {
                "id": 4,
                "title": "征收补偿费用二审民事判决书",
                "parent": "民事诉讼",
                "create_time": "2019-08-29"
            },
            {
                "id": 3,
                "title": "民事再审申请书",
                "parent": "民事诉讼",
                "create_time": "2019-08-29"
            },
            {
                "id": 2,
                "title": "机动车交通事故责任纠纷二审民事判决书",
                "parent": "民事诉讼",
                "create_time": "2019-08-29"
            },
            {
                "id": 1,
                "title": "买卖合同纠纷一审民事判决书",
                "parent": "民事诉讼",
                "create_time": "2019-08-29"
            }
        ]
    }
}
```

## 添加法律文书
<a id=添加法律文书> </a>
### 基本信息

**Path：** /instrument/add

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
| tid | text  |  是 |    |  法律文书分类ID |
| title | text  |  是 |    |  法律文书主标题 |
| content | text  |  是 |    |  法律文书文本内容 |



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
    "msg": "添加法律文书成功"
}
```

## 编辑法律文书
<a id=编辑法律文书> </a>
### 基本信息

**Path：** /instrument/edit

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
| id | text  |  是 |    |  法律文书文章ID |
| tid | text  |  是 |    |  法律文书分类ID |
| title | text  |  是 |    |  法律文书文章主标题 |
| content | text  |  是 |    |  法律文书文章正文内容 |



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
    "msg": "编辑法律文书成功"
}
```

## 删除法律文书
<a id=删除法律文书> </a>
### 基本信息

**Path：** /instrument/delete

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
| id | 是  |   |  法律文书文章ID |

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
    "msg": "删除法律文书成功"
}
```

## 读取法律文书
<a id=读取法律文书> </a>
### 基本信息

**Path：** /instrument/read

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
| id | 是  |   |  法律文书文章ID |

### 返回数据

<table>
  <thead class="ant-table-thead">
    <tr>
      <th key=name>名称</th><th key=type>类型</th><th key=required>是否必须</th><th key=default>默认值</th><th key=desc>备注</th><th key=sub>其他信息</th>
    </tr>
  </thead><tbody className="ant-table-tbody"><tr key=0-0><td key=0><span style="padding-left: 0px"><span style="color: #8c8a8a"></span> code</span></td><td key=1><span>string</span></td><td key=2>必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">返回码</span></td><td key=5></td></tr><tr key=0-1><td key=0><span style="padding-left: 0px"><span style="color: #8c8a8a"></span> msg</span></td><td key=1><span>string</span></td><td key=2>必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">返回码信息</span></td><td key=5></td></tr><tr key=0-2><td key=0><span style="padding-left: 0px"><span style="color: #8c8a8a"></span> data</span></td><td key=1><span>object</span></td><td key=2>必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">数据集</span></td><td key=5></td></tr><tr key=0-2-0><td key=0><span style="padding-left: 20px"><span style="color: #8c8a8a">├─</span> id</span></td><td key=1><span>number</span></td><td key=2>必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">法律文书文章ID</span></td><td key=5></td></tr><tr key=0-2-1><td key=0><span style="padding-left: 20px"><span style="color: #8c8a8a">├─</span> title</span></td><td key=1><span>string</span></td><td key=2>必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">法律文书文章主标题</span></td><td key=5></td></tr><tr key=0-2-2><td key=0><span style="padding-left: 20px"><span style="color: #8c8a8a">├─</span> content</span></td><td key=1><span>string</span></td><td key=2>必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">法律文书正文内容</span></td><td key=5></td></tr><tr key=0-2-3><td key=0><span style="padding-left: 20px"><span style="color: #8c8a8a">├─</span> tid</span></td><td key=1><span>string</span></td><td key=2>必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">法律文书分类ID</span></td><td key=5></td></tr>
               </tbody>
              </table>

### 示例

```json
{
    "code": "200",
    "msg": "获取成功",
    "data": {
        "id": "1",
        "title": "买卖合同纠纷一审民事判决书",
        "content": "当事人信息(均为化名)\n\n原告彭逢阳，男，汉族，1946年2月16日出生，住北京市宣武区。\n\n委托代理人秦舰，四川精伦律师事务所律师。\n\n被告费顶发，男，汉族，1966年7月28日出生，住四川省双流县。\n\n委托代理人萧国辉，四川中业律师事务所律师。\n\n审理经过\n\n原告彭逢阳诉被告费顶发买卖合同纠纷一案，本院于2015年2月2日立案受理后，依法由代理审判员易炜适用简易程序公开开庭进行了审理。原告彭逢阳及其委托代理人秦舰、被告费顶发及其委托代理人萧国辉均到庭参加诉讼。本案现已审理终结。\n\n原告诉称\n\n原告彭逢阳诉称，2009年9月，被告向原告购买工程车两台，议定总价为96万元，双方约定2009年底付款46万元，余款2010年底前付清，但被告至2010年10月才累计付款30万元，其后4年，原告一直向被告追讨，但被告均以种种理由不给。2014年1月29日，在原告的一再催收下，被告同意把欠款尽快付清，被告要求原告将以前的付款收据拿来清理，趁原告不备在原来的收据上涂抹，并单方面给原告写了一张40万元的欠条，被告在欠条上明确最晚2014年4月30日付清，原告没有同意其将66万元的欠款改成40万元，被告也未按其承诺支付这40万元，并继续以各种理由推脱原告的催收，故原告要求被告支付从2014年4月30日起未支付欠款的违约金共计5万元。为维护原告的合法权益，特起诉请求：1、判令被告向原告归还660000元及利息(按中国人民银行贷款利息计算自2011年1月1日起至本金付清之日止);2、判令被告支付原告违约金50000元。\n\n被告辩称\n\n被告费顶发辩称，被告向原告购买了两台车是事实，但是双方没有说好价格，原告出售给被告的两台车价值没有96万元这么多，被告多次要求对车子进行评估以确定一个合理的价格，但是原告不予配合。原告出具的收据仅能证明被告向其支付了30万元货款，但不能证明两车的价款是96万元，收据一直是由原告在保管，收据上的字除了被告的签名外，其他字都是原告写的，总价96万元当时没有，是原告后来自己加上去的，被告也没有对收据进行过涂改。原告收到被告出具的欠条，并未表示反对，表明其已经接受了被告只欠其40万元的意思表示，如果原告对此不予认可，则此案已过了诉讼时效。双方没有约定违约金，故原告要求被告支付违约金没有依据。\n\n本院查明\n\n经审理查明，被告于2009年向原告购买了16吨和50吨吊车各一台，16吨吊车于当年7月交付给被告，50吨吊车于当年9月交付给被告，双方未签订书面合同。收车后，被告于2010年3月3日向原告支付了100000元、于2010年7月27日支付了100000元、于2010年10月9日支付了100000元，原告分别出具了三张收款收据，被告在该收据上签字认可付款金额，此后未再向原告付款。2014年1月29日，被告向原告出具了欠条一张，载明：“今欠至彭逢阳吊车(两台)余款400000元(以前所有票据已作废)，分三次付清，最晚4月30日前付清”，并将原告于2010年7月27日、2010年10月9日出具的收据进行涂抹。此后，被告仍然未向原告付款，原告起诉来院。\n\n以上事实，有原、被告的身份信息、收据、欠条和原、被告的一致陈述在卷佐证。\n\n本院认为\n\n本院认为，原、被告虽然未签订书面合同，但双方均认可被告向原告购买了两台吊车的事实存在，结合原告出具的收款收据，应当认为双方的买卖合同已经成立。原、被告双方虽对吊车总价款各执一词，但被告于2014年1月29日向原告出具的欠购车余款40万元的欠条，原告持欠条主张权利，应视为双方对购车总价款及余款的付款期限达成的一致意见，原、被告均应受此协议约束。现被告未按期付款，应当承担法律责任，被告应以欠条确定的未付货款400000元为本金，按中国人民银行同期贷款利率向原告支付资金占用利息。双方未约定违约金，原告要求被告向其支付50000元违约金的请求没有依据，不予支持。\n\n据此，根据《中华人民共和国合同法》第一百零九条、第一百一十二条、第一百五十九条、第一百六十一条，《最高人民法院关于审理买卖合同纠纷案件适用法律若干问题的解释》第一条之规定，判决如下：\n\n裁判结果\n\n被告费顶发于本判决生效之日起三日内向原告彭逢阳支付货款400000元及利息(利息计算方法为：以400000元为本金，按中国人民银行同期贷款利率计算利息，从2014年5月1日起至其付清该款之日止)。\n\n如果未按判决指定的期间履行给付金钱义务，应当依照《中华人民共和国民事诉讼法》第二百五十三条之规定，加倍支付迟延履行期间的债务利息。\n\n案件受理费5450元，由被告费顶发负担。\n\n如不服本判决，可在本判决送达之日起十五日内向本院递交上诉状，并按对方当事人的人数提出副本，上诉于四川省成都市中级人民法院。\n\n审判人员\n\n代理审判员易炜\n\n裁判日期\n\n二〇一五年四月二十一日\n\n书记员\n\n书记员夏东",
        "tid": 9
    }
}
```
