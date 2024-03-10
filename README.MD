# 비트코인 GPT 인공지능 AI 업비트 자동매매 시스템 만들기

- GPT API를 활용하여 투자를 자동화 합니다. by 유튜버 조코딩

## 관련 링크

- [수업 자료](https://jocoding.net/bitcoin)

## 로컬 환경 설정

pip install -r requirements.txt
[업비트 API 홈페이지](https://upbit.com/mypage/open_api_management)

### 기본 세팅

- 한국 기준으로 서버 시간 설정: sudo ln -sf /usr/share/zoneinfo/Asia/Seoul /etc/localtime
- 한국 기준으로 서버 시간 설정

```
sudo ln -sf /usr/share/zoneinfo/Asia/Seoul /etc/localtime
```

- 패키지 목록 업데이트

```
sudo apt update
sudo apt upgrade
sudo apt install python3-pip
```

### 레포지토리 가져오기

```
git clone https://github.com/youtube-jocoding/gpt-bitcoin.git
```

### 서버에서 라이브러리 설치

```
pip3 install -r requirements.txt
```

### .env 파일 만들고 API KEY 넣기

```
vim .env
```

### 명령어

- 현재 경로 상세 출력

```
ls -al
```

- 경로 이동

```
cd 경로
```

- vim 에디터로 파일 열기

```
vim autotrade.py
```

- vim 에디터 입력: i
- vim 에디터 저장: :wq!
- vim 에디터 저장: ESC + wq!

### 실행하기
- 그냥 실행
```
python3 autotrade.py
```
- 백그라운드 실행
```
nohup python3 -u autotrade.py > output.log 2>&1 &
```
- 로그 보기
```
cat output.log
tail -f output.log
```
- 실행 확인
```
ps ax | grep .py
```
- 종료하기
```
kill -9 PID
ex. kill -9 13586
```

## 추후 계획

- 빗썸, 바이낸스, 코인베이스, OKX, 바이비트도 가능하면 다루겠음
