# llm-playground


## 가상환경 설정
- 현 프로젝트를 위한 환경이 외부 환경과 독립되도록 가상환경을 먼저 설정합니다
```shell
# 가상환경 생성
python3.12 -m venv venv
# 가상환경 활성화
source ./venv/bin/activate

# 프로젝트 필요 패키지 설치
pip install -r requirements.txt

# 비활성화
# deactivate
```

### Configure
> No python interpreter figured for the module

1. Project Settings (File > Project Structure)
2. Project > SDK > add python interpreter from disk > Existing Environment > interpreter
3. `현재 경로/venv/bin/python` 로 연동


## Directory 구성

```shell
- multiturn # 채팅 맥락 유지 플레이그라운드
```

### 실행 방법
- 원하는 playground directory 들어가서 아래 명령어 실행
```shell
streamlit run app.py 

#또는 root 에서 
#streamlit run multiturn/app.py 
```