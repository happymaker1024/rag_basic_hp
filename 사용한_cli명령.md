powershell -ExecutionPolicy ByPass -c "irm https://astral.sh/uv/install.ps1 | iex"

# 파이썬 버전 고정 및 가상환경 만들기
```
uv --version
uv python pin 3.10
Get-Content .python-version
uv venv .venv --python 3.10 --prompt .venv
```
# powershell 보안 문제 해결
```
Set-ExecutionPolicy -Scope CurrentUser -ExecutionPolicy RemoteSigned
```

# 가상환경 활성화
```
.\.venv\Scripts\activate
```

# 라이브러리 설치
```
uv add -r .\requirements.txt
```