# 📙 1. Conda 기본 정보 확인

Conda가 정상 설치되었는지, 어떤 환경이 구성되어 있는지 확인할 때 사용합니다.

```
    conda --version          # Conda 버전 확인
    conda info               # Conda 환경, 설정 정보 확인
    conda init               # Shell 초기화
    conda env list           # 전체 가상환경 목록 확인
```

---

# 📘 2. Conda 가상환경 관리

## ▶  가상환경 활성화 / 비활성화

```
    conda activate [가상환경이름]
    conda deactivate
```

## ▶  가상환경 생성

```
    conda create -n [가상환경이름] python=버전
```

## ▶  가상환경 패키지 목록 확인

```
    conda list
```

---

# 📗 3. Jupyter Notebook 설치 & 커널 등록

## ▶  Jupyter Notebook 설치

```
    pip install jupyter notebook
```

## ▶  Conda 환경을 주피터 커널로 등록

```
    python -m ipykernel install --user --name 가상환경이름 --display-name "커널출력이름"
```

---

# 📕 4. 환경 및 커널 삭제

## ▶ 🗑 Jupyter 커널 삭제

```
    jupyter kernelspec uninstall test
```

## ▶ 🗑 Conda 가상환경 삭제

```
    conda remove --name 가상환경이름 --all
```

---

# 📘 5. Jupyter Notebook 실행

## ▶ 🔹 해당 커널을 사용할 가상환경 활성화 후 실행

```
    conda activate 커널출력이름
    jupyter notebook
```

