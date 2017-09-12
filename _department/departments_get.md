---
title: 获取所有部门
position: 4.1
type: get
right_code: |
  ~~~ json
  [
    {
        "name": "管理组",
        "uuid": "7684be70c34c554c8fdc062eba4382be",
        "superior_uuid": null,
        "charger_uuid": "fbfd8384fb43da1d979fd277473d7984"
    },
    {
        "name": "运营组",
        "uuid": "8674be70c34c554c8fdc062eba4382be",
        "superior_uuid": null,
        "charger_uuid": "fbfd8384fb43da1d979fd277473d7984"
    },
    {
        "name": "系统组",
        "uuid": "8689be70c34c554c8fdc062eba4382be",
        "superior_uuid": null,
        "charger_uuid": "fbfd8384fb43da1d979fd277473d7984"
    }
  ]
  ~~~
  {: title="Response" }
---
---

**GET** `/api/v2/departments`
{: .success }

### HTTP Parameters

参数       | 类型       | 默认值 | 必须 | 描述
-----------|------------|--------|------|----------------------------|
access_key | 字符串     |        | 是   | API Key
tonce      | 整型       |        | 是   | 以秒为单位的UNIX timestamp
signature  | 字符串     |        | 是   | 请求签名

### Response

JSON 格式的 [部门对象](#objectdepartment) 数组