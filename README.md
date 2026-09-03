<img src="./metal-slug-fio-by-specterwhite.png" width = "337" height = "477" alt="Fio" align=right />
<div align="center">

<!-- thanks for:https://github.com/NolanHo/NolanHo -->
<!-- thanks for:https://github.com/Xbodwf/Xbodwf -->
> <p align="left"><em>
>     用代码表达言语的魅力，用代码书写山河的壮丽。
> </em></p>
> <p align="right">
>     &mdash;&mdash;&mdash; 一言「一言开发者中心」
> </p>
<p align="left">
  <div align="left">

  ```python
import requests
import time

def receive_messages(api_url, token):
    last_id = 0
    while True:
        try:
            response = requests.get(f"{api_url}/messages?since={last_id}")
            messages = response.json().get("messages", [])
            for msg in messages:
                print(f"收到消息: {msg['sender']}: {msg['content']}")
                last_id = max(last_id, msg['id'])
            time.sleep(2)

API_URL = "http://voce.bugcode.cc/api"
receive_messages(API_URL, TOKEN)
  ```
  <br>
  有点难绷
  </div>
</p>
</div>

<details>
  <summary>🖨️ 站点详细</summary><br>

  | 介绍 | 链接 |
  | ---- | ---- |
  | 主要站点 | https://bugcode.cc |
  | 备用站点 | https://411912.xyz |
  | 灾备站点 | https://bugji.github.io |
  | 加入我的QQ群 | [http://qun.qq.com/invite?group_id=835382474](https://qm.qq.com/cgi-bin/qm/qr?k=BixrGd63CrHhe5oawoEGtXQSSSn8sJcT&jump_from=webapi&authKey=rIqkvqkIBOgiN4tqh9n6mRW3MyJn4P/cYp+Q11D9aYJj54BbLsXW0QlMTYuK+Uan) |


</details>
