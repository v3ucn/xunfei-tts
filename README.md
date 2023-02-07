# xunfei-tts

pip install -r requirements.txt

```
if __name__ == "__main__":
    # 测试时候在此处正确填写相关信息即可运行
    ifly = Ifly(APPID='', APISecret='',
                       APIKey='',
                       Text="你好这是一个语音合成示例")
    websocket.enableTrace(False)
    wsUrl = ifly.create_url()
    print(wsUrl)
    ws = websocket.WebSocketApp(wsUrl, on_message=on_message,on_close=on_close)
    print(ws)
    ws.on_open = on_open
    ws.run_forever(sslopt={"cert_reqs": ssl.CERT_NONE})
```
