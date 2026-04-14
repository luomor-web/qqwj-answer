```shell
ssh-agent /bin/sh
https://wj.qq.com/docs/webhook/
腾讯问卷展示answer

你是一名资深开发，编写一个页面从接口读取数据，并转为html标签显示内容，数据主要为问答数据，接口请求为post请求，接口地址：http://xlab.ai-space.net/api/activity/getAnwserInfo/{id}，主要解析字段为answer，json数据示例：{             "id": "33cc555f-056f-4242-a97c-46f3e7d2016f",             "object": "Answer",             "action": "answer.create",             "created_at": "2021-01-26 14:00:00",             "payload": {                 "survey_id": 25721826,                 "survey_hash": "7446",                 "answer_id": 7,                 "respondent_id": 60000000001,                 "respondent_type": "",                 "openid": "",                 "started_at": "2020-02-09 11:55:30",                 "ended_at": "2020-02-09 11:58:39",                 "duration": 189,                 "country": "中国",                 "province": "广东省",                 "city": "深圳市",                 "ip": "127.0.0.1",                 "ua": "Mozilla/5.0 (iPhone; CPU iPhone OS 15_4_1 like Mac OS X) AppleWebKit/605.1.15 (KHTML, like Gecko) Mobile/15E148",                 "referrer": "https://wj.qq.com/xxx.html",                 "third_party_user": {                     "respondent_id": 60000000001,                     "openid": "abcdefg",                     "nickname": "张三"                 },                 "answer": [                     {                         "id": "p-1-abcd",                         "questions": [                             {                                 "id": "q-1-abcd",                                 "type": "radio",                                 "options": [                                     {                                         "id": "o-100-ABCD",                                         "checked": 1,                                         "text": "选项"                                     }                                 ],                                 "blanks": []                             }                         ]                     },                     {                         "id": "custom_args",                         "questions": [                             {                                 "id": "custom-arg-01",                                 "type": "text",                                 "text": "17695796264",                                 "title": "phone",                                 "description": "用户ID，传递用户身份信息"                             }                         ]                     }                 ]             }         }

可以从url参数中输入id，如?id=，并对页面进行美化

更新README.md，增加agent.md
将agent.md改为中文

irm https://trae.cn/trae-cli/install.ps1 | iex 
traecli
/login

traecli update
```