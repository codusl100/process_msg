# 💬 GPT 메세지 전처리 패키지
### 1. process-msg 패키지 다운로드
```shell
pip install process-msg==0.0.2
```
[최신 버전 (0.0.2)](https://pypi.org/project/process-msg/0.0.2/) (latest updated 23.11.27)

<br>

### 2. 패키지 파라미터
```python
def process_message(api_key, content, name="quality manager",
                    instructions="You are a quality manager. Classify types of faults and deduct possible causes.",
                    require_content="를 문제를 표현하는 부분만 나타내도록 한국어로 최대한 간결하게 압축해줘.")
```
- api_key = GPT Openai secret key
- content = 요약 핵심 텍스트 
- instructions = assistant 설명 (default = "You are a quality manager. Classify types of faults and deduct possible causes.")
- require_content = 요구사항 텍스트 (default = "를 문제를 표현하는 부분만 나타내도록 한국어로 최대한 간결하게 압축해줘.")


<br>

### 3. 패키지 사용 예시
```python
import process-msg

process_msg("open ai key", "틸트호스 크랙으로 오일누유 발생")
```
