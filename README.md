# MockingBird-colab

1.安装pyngrok 
```
!pip install pyngrok 
```
2.注册pyngrok 并配置Authtoken
```
!ngrok authtoken  <your token>
```
3.启动pyngrok
```
from pyngrok import ngrok

# Setup a tunnel to the streamlit port 2023
ngrok.kill()

public_url = ngrok.connect(2023)
print(public_url)
```
4.修改端口号为2023并启动streamlit，然后访问上一步pyngrok的地址就可以使用了
