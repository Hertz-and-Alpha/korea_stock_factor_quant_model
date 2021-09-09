# 설치 준비사항
> 2021 4월 25일에 새로운 zipline 버전 업데이트: The [new Zipline version](https://github.com/stefan-jansen/zipline-reloaded) 도커 사용없이 원도우, 맥, 리눅스 다 설치해서 사용가능
> 기존에 퀀토피안에서 포기했던 zipline을 stefan jansen이 최근 파이썬 환경에서도 돌아가게 수정 해놓은 버전

> 여기서 US 기준으로 되어있는 zipline을 모두 KOREA에 맞게 수정한 파일을 windows 폴더 안에 넣어 놓았다.
> 여기 코드들은 파이썬 3.8 버전을 사용합니다. 


# mamba 설치
> 윈도우키를 누르고 Anaconda Powershell Prompt를 실행시킵니다.
```shell
conda install -n base -c conda-forge mamba
```
> mamba를 사용하는 이유는 기존의 anaconda를 이용해서 설치하는 것 보다 mamba를 이용하는 것이 속도가 훨씬 더 빠르다.
> mamba 설치 후 아래 명령어를 실행 시킵니다.

```shell
mamba env create -f installation/windows/ml4t_korea.yml
```

# 아나콘다 가상환경 실행

```shell
conda activate ml4t_korea
```

```shell
pip install installation/windows/trading_calendars_korea-0.0.1-py3-none-any.whl
```

```shell
pip install installation/windows/zipline_reloaded_korea-0.0.3-cp38-cp38-win_amd64.whl
```


