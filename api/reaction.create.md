# reaction.create

创建消息 Reaction

## 请求方式

```
POST {base_url}/reaction.create
```

## 请求参数

**需要登录**

| 参数名称 | 参数类型 | 参数是否必须？ | 说明 | 样例 |
|:--------:|:--------:|:--------------:|------|------|
| `vchannel_id` | `string` | 是 | 消息所在的频道 | =bw52O |
| `key` | `string` | 是 | 想要加 sticker 的 message 的 key | 1540460114044.0100 |
| `reaction` | `string` | 是 | 想要添加的 reaction 名 | :smile: |

## 响应

### 200

```javascript
{
  "id": "=bw52Q",
  "team_id": "=bw52R",
  "uid": "=bw52S",
  "message_id": "=bw52Q",
  "message_key": "1540460114044.0100",
  "reaction": ":smile:"
  "created_ts": 1540461431018,
  "created": "2018-10-25T09:57:11.000+0000",
  "updated": "2018-10-25T09:57:11.000+0000"
}
```
### 错误响应

```javascript
{
  "code": // error code,
  "error": "unexpected error"
}
```

<!-- generated by gen_doc.js -->
