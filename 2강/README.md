# 2강 / 명령어와 버튼 제작하기!
----

## 준비물 : Vscode ( 비쥬얼 스튜디오 코드 ) , Python, 1강의 main.py

----

✅ 출처 : https://disnake.dev/
⚙️ 1강때 사용했던 폴더가 필요합니다!
----

1. 저번과 같이 Vscode ( 비쥬얼 스튜디오 코드 ) 를 ```code . ``` 명령어를 사용해서 사용 해주세요.
2. 먼저 명령어 부터 만들겠습니다! 저희는 슬러쉬 커맨드를 사용 하겠습니다.
```
import disnake
from disnake.ext import commands

bot = commands.Bot()

@bot.event
async def on_ready():
    print("봇이 준비 됬습니다")

bot.run("발급받은 봇 토큰")
```
3. 저번에 했던 코드 입니다. 아래 코드를 추가 해주면 명령어가 정상 작동 합니다.
```
@bot.slash_command(name="명령어 이름")
async def 명령어이름(inter):
    await inter.response.send_message("테스트")
```
4. 이 코드는 ```@bot.event
async def on_ready():
    print("봇이 준비 됬습니다")``` 이거 아래로 해주세요.