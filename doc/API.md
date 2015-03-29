#User类
###Function:注册/找回密码，发送验证码
IN

    phone:"18731245087"

OUT(json示例)

    {
    "state": 1,
    "msg": "请求频率超限"
    }

###Function:验证码校验
IN  

    phone:"18731245087"
    checknum:"223214"

OUT(json示例)  

    {
      "state": 1,
      "msg": "请求频率超限",
      "key": "aaf298fd195470b7f0f44d7f05753339",
      "openid": "aaf298fd195470b7f0f44d7f05753339"
    }

###Function:登入（数据加密）
IN  

    phone
    password 

OUT(json示例)

    {
      "state": 1,
      "msg": "'请求频率超限'",
      "key": "'aaf298fd195470b7f0f44d7f05753339'",
      "openid": "'aaf298fd195470b7f0f44d7f05753339'",
      "type": 2
    }

###Function:初始化/修改用户信息
IN

	key
	openid
	type/device(不同用户类型，字段不同)

OUT(json示例)

	{
	  "state": 1,
	  "msg": "'请求频率超限'"
	}

###Function:查看用户信息
IN

	key
	begin PC端查看多个数据
	end 
	openid APP查看单一数据
	search 搜索选项,json数据

OUT(json示例)

	{
	  "state": 1,
	  "msg": "'请求频率超限'",
	  "openid": "'aaf298fd195470b7f0f44d7f05753339'",
	  "phone": "'18733212239'",//仅APP请求返回
	  "device": [
	    "'00:1c:42:00:00:08'",
	    "'00:1c:42:00:00:08'"
	  ]
	}

###Function:删除用户
IN

	key
	openid

OUT(json示例)

	{
	  "state": 1,
	  "msg": "'请求频率超限'"
	}

###Function:登出
IN

	key

OUT(json示例)

	{
	  "state": 1,
	  "msg": "'请求频率超限'"
	}

###Function:绑定设备
IN

	key
	device两边都要请求
	openid

OUT(json示例)

	{
	  "state": 1,
	  "msg": "'请求频率超限'"
	}

###Function:解绑设备
IN

	key
	device

OUT(json示例)

	{
	  "state": 1,
	  "msg": "'请求频率超限'"
	}
