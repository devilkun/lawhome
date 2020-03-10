# 法律文档类型（法规，罪名库，文书，合同范本）

## 类型列表
<a id=类型列表> </a>
### 基本信息

**Path：** /type/list

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
| pid | 是  |   |  父级ID |

### 返回数据

<table>
  <thead class="ant-table-thead">
    <tr>
      <th key=name>名称</th><th key=type>类型</th><th key=required>是否必须</th><th key=default>默认值</th><th key=desc>备注</th><th key=sub>其他信息</th>
    </tr>
  </thead><tbody className="ant-table-tbody"><tr key=0-0><td key=0><span style="padding-left: 0px"><span style="color: #8c8a8a"></span> code</span></td><td key=1><span>string</span></td><td key=2>必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">返回码</span></td><td key=5></td></tr><tr key=0-1><td key=0><span style="padding-left: 0px"><span style="color: #8c8a8a"></span> msg</span></td><td key=1><span>string</span></td><td key=2>必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">返回码信息</span></td><td key=5></td></tr><tr key=0-2><td key=0><span style="padding-left: 0px"><span style="color: #8c8a8a"></span> data</span></td><td key=1><span>object</span></td><td key=2>必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">数据集</span></td><td key=5></td></tr><tr key=0-2-0><td key=0><span style="padding-left: 20px"><span style="color: #8c8a8a">├─</span> totalSize</span></td><td key=1><span>number</span></td><td key=2>必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">总条数</span></td><td key=5></td></tr><tr key=0-2-1><td key=0><span style="padding-left: 20px"><span style="color: #8c8a8a">├─</span> currentPage</span></td><td key=1><span>number</span></td><td key=2>必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">当前页码</span></td><td key=5></td></tr><tr key=0-2-2><td key=0><span style="padding-left: 20px"><span style="color: #8c8a8a">├─</span> pageSize</span></td><td key=1><span>number</span></td><td key=2>必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">每页条数</span></td><td key=5></td></tr><tr key=0-2-3><td key=0><span style="padding-left: 20px"><span style="color: #8c8a8a">├─</span> totalPage</span></td><td key=1><span>number</span></td><td key=2>必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">总页码</span></td><td key=5></td></tr><tr key=0-2-4><td key=0><span style="padding-left: 20px"><span style="color: #8c8a8a">├─</span> list</span></td><td key=1><span>object []</span></td><td key=2>必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap"></span></td><td key=5><p key=3><span style="font-weight: '700'">item 类型: </span><span>object</span></p></td></tr><tr key=0-2-4-0><td key=0><span style="padding-left: 40px"><span style="color: #8c8a8a">├─</span> id</span></td><td key=1><span>number</span></td><td key=2>必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">类型ID</span></td><td key=5></td></tr><tr key=0-2-4-1><td key=0><span style="padding-left: 40px"><span style="color: #8c8a8a">├─</span> name</span></td><td key=1><span>string</span></td><td key=2>必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">类型名称</span></td><td key=5></td></tr><tr key=0-2-4-2><td key=0><span style="padding-left: 40px"><span style="color: #8c8a8a">├─</span> create_time</span></td><td key=1><span>string</span></td><td key=2>必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">创建时间</span></td><td key=5></td></tr>
               </tbody>
              </table>
              
### 示例

```json
{
    "code": "200",
    "msg": "获取成功",
    "data": {
        "totalSize": 3,
        "currentPage": 1,
        "pageSize": 10,
        "totalPage": 1,
        "list": [
            {
                "id": 7,
                "name": "行政法类",
                "create_time": "2019-08-29"
            },
            {
                "id": 6,
                "name": "民商法类",
                "create_time": "2019-08-29"
            },
            {
                "id": 5,
                "name": "宪法类",
                "create_time": "2019-08-29"
            }
        ]
    }
}
```

## 添加类型
<a id=添加类型> </a>
### 基本信息

**Path：** /type/add

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
| name | text  |  是 |    |  类型名称 |
| level | text  |  否 |    |  类型级别（默认为一级分类，如需要添加二级分类，此处应添加参数为second） |
| pid | number  |  否 |    |  父级ID（添加二级类型时是为必需项） |



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
    "msg": "添加类型成功"
}
```

## 编辑类型
<a id=编辑类型> </a>
### 基本信息

**Path：** /type/edit

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
| id | number  |  是 |    |  类型ID |
| name | text  |  是 |    |  类型名称 |



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
    "msg": "编辑类型成功"
}
```

## 删除类型
<a id=删除类型> </a>
### 基本信息

**Path：** /type/delete

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
| id | 是  |   |  类型ID |

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
    "msg": "删除类型成功"
}
```

## 获取类型
<a id=获取类型> </a>
### 基本信息

**Path：** /type/read

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
| id | 是  |   |  类型ID |

### 返回数据

<table>
  <thead class="ant-table-thead">
    <tr>
      <th key=name>名称</th><th key=type>类型</th><th key=required>是否必须</th><th key=default>默认值</th><th key=desc>备注</th><th key=sub>其他信息</th>
    </tr>
  </thead><tbody className="ant-table-tbody"><tr key=0-0><td key=0><span style="padding-left: 0px"><span style="color: #8c8a8a"></span> code</span></td><td key=1><span>string</span></td><td key=2>必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">返回码</span></td><td key=5></td></tr><tr key=0-1><td key=0><span style="padding-left: 0px"><span style="color: #8c8a8a"></span> msg</span></td><td key=1><span>string</span></td><td key=2>必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">返回码信息</span></td><td key=5></td></tr><tr key=0-2><td key=0><span style="padding-left: 0px"><span style="color: #8c8a8a"></span> data</span></td><td key=1><span>object</span></td><td key=2>必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap"></span></td><td key=5></td></tr><tr key=0-2-0><td key=0><span style="padding-left: 20px"><span style="color: #8c8a8a">├─</span> id</span></td><td key=1><span>number</span></td><td key=2>必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">类型ID</span></td><td key=5></td></tr><tr key=0-2-1><td key=0><span style="padding-left: 20px"><span style="color: #8c8a8a">├─</span> name</span></td><td key=1><span>string</span></td><td key=2>必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">类型名称</span></td><td key=5></td></tr>
               </tbody>
              </table>

### 示例

```json
{
    "code": "200",
    "msg": "获取成功",
    "data": {
        "id": 5,
        "name": "宪法类"
    }
}
```

## 获取类型下拉列表数据
<a id=获取类型下拉列表数据> </a>
### 基本信息

**Path：** /type/select

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
| pid | 是  |   |  父级分类ID |

### 返回数据

<table>
  <thead class="ant-table-thead">
    <tr>
      <th key=name>名称</th><th key=type>类型</th><th key=required>是否必须</th><th key=default>默认值</th><th key=desc>备注</th><th key=sub>其他信息</th>
    </tr>
  </thead><tbody className="ant-table-tbody"><tr key=0-0><td key=0><span style="padding-left: 0px"><span style="color: #8c8a8a"></span> code</span></td><td key=1><span>string</span></td><td key=2>必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">返回码</span></td><td key=5></td></tr><tr key=0-1><td key=0><span style="padding-left: 0px"><span style="color: #8c8a8a"></span> msg</span></td><td key=1><span>string</span></td><td key=2>必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">返回码信息</span></td><td key=5></td></tr><tr key=0-2><td key=0><span style="padding-left: 0px"><span style="color: #8c8a8a"></span> data</span></td><td key=1><span>object []</span></td><td key=2>必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">数据集</span></td><td key=5><p key=3><span style="font-weight: '700'">item 类型: </span><span>object</span></p></td></tr><tr key=0-2-0><td key=0><span style="padding-left: 20px"><span style="color: #8c8a8a">├─</span> id</span></td><td key=1><span>number</span></td><td key=2>必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">分类ID</span></td><td key=5></td></tr><tr key=0-2-1><td key=0><span style="padding-left: 20px"><span style="color: #8c8a8a">├─</span> name</span></td><td key=1><span>string</span></td><td key=2>必须</td><td key=3></td><td key=4><span style="white-space: pre-wrap">分类名称</span></td><td key=5></td></tr>
               </tbody>
              </table>

### 示例

```json
{
    "code": "200",
    "msg": "获取成功",
    "data": [
        {
            "id": 5,
            "name": "宪法类"
        },
        {
            "id": 6,
            "name": "民商法类"
        },
        {
            "id": 7,
            "name": "行政法类"
        }
    ]
}
```
