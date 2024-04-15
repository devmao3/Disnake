# 1강 / 코딩하기
----

## 준비물 : Vscode ( 비쥬얼 스튜디오 코드 ) , Python

----

✅ 출처 : https://disnake.dev/

----

1. 먼저 폴더를 만들고 거기 안에 main.py 파일을 생성한다.
2. 파일 탐색기 에서 위 위치를 눌러서 cmd를 입력한다.
3. ![image](https://github.com/devmao3/Disnake/assets/167006209/ea73af13-d954-457d-b0e2-b49aeff226b8)
 이렇게 뜨면 위아 같이 ```code . ``` 를 입력해준다.
4. 그러면 창이 뜰텐데 옆에 있는 main.py를 눌러준다 ![image](https://github.com/devmao3/Disnake/assets/167006209/aa1fc896-221c-4f4d-8ee2-c61474eb30b2)
5. 거기다가 이렇게 붙여 넣어 준다.
```
import disnake
from disnake.ext import commands

bot = commands.Bot()

@bot.event
async def on_ready():
    print("봇이 준비 됬습니다")

bot.run("발급받은 봇 토큰")
```
6. 그리고 발급받은 봇 토큰을 저기다가 넣어준다.
7. 또 방금 cmd 에서 ```pip install disnake``` 입력 해주고
8. cmd 에다가 ```py main.py``` 입력해주면 봇 실행은 끝
