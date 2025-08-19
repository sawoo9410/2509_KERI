# AI Course Environment Setup

이 리포지토리는 AI Course 프로젝트를 위한 가상환경 생성, 패키지 설치, Jupyter 커널 등록 및 사용법 안내를 제공합니다.

---

## 환경 생성 및 패키지 설치

### 1. Conda 가상환경 생성

아래 명령어로 Python 3.9 버전을 사용하는 Conda 가상환경 'AI-Course'를 만듭니다:

```bash
conda create -n AI-Course python=3.9 -y
```

### 2. 가상환경 활성화

```bash
conda activate AI-Course
```

### 3. 패키지 설치

requirements.txt 파일을 기준으로 PyTorch CUDA 11.8 버전용 휠을 포함하여 필요한 패키지들을 설치합니다:

```bash
pip install -r requirements.txt --extra-index-url https://download.pytorch.org/whl/cu118
```

### 4. Jupyter 커널 등록

가상환경을 Jupyter Notebook이나 JupyterLab에서 커널로 사용할 수 있도록 등록합니다:

```bash
python -m ipykernel install --user --name ai_course --display-name "AI Course (Python 3.9)"
```

---

## Jupyter에서 가상환경 사용하기

1. Jupyter Notebook 또는 JupyterLab을 실행합니다.

2. 새 노트북 생성시 'AI Course (Python 3.9)' 커널을 선택하여 해당 환경에서 코드를 실행할 수 있습니다.

---

## 기타

- 필요한 패키지나 환경 설정 변경 시, requirements.txt나 Conda 환경을 업데이트하세요.  
- CUDA 및 PyTorch 버전호환성을 신경써서 설치하시는 것을 권장합니다.

