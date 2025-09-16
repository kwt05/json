// config.json
[
  {
    "tenant_name": "学校名称",
    "account": "账号",
    "password": "密码",
    "study": true, // 是否学习课程，默认开启
    "study_time": 15, // 每节课学习时间，单位（秒），默认 15 秒
    "restudy_time": 0, // 每节课重新学习时间，单位（秒），默认不开启，有学习时长的要求可以设置
    "exam": true, // 是否考试，默认开启
    "exam_use_time": 250 // 考试总时间，单位（秒），会平均到每到题上，默认 250 秒
  },
  // 或者
  {
    "tenant_name": "学校名称", // 与 user 字段的二选一，优先使用 user 字段的
    "user": {
      "userId": "可以从浏览器F12->存储->Local Storage->user->userId 中找到",
      "token": "可以从浏览器F12->存储->Local Storage->user->token 中找到",
      "tenantName": "" // 二选一，会优先使用这个
    }
  }
]
