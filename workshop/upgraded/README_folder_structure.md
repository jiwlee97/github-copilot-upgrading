# upgraded 폴더 구조 설명

`upgraded` 폴더는 `legacy` 폴더의 전체 파일 및 디렉토리 구조를 그대로 복사한 폴더입니다. 각 파일과 폴더의 역할은 다음과 같습니다.

## 최상위 파일 및 폴더
- `MANIFEST.in`, `README.rst`, `distribute-0.6.10.tar.gz`, `distribute_setup.py`, `setup.py`: 패키지 메타데이터, 설치 스크립트, 설명 파일 등 Python 패키징 관련 파일입니다.
- `docs/`: 프로젝트 문서화 관련 파일 및 빌드 결과물이 포함된 폴더입니다.
- `guachi/`: 주요 Python 소스 코드와 테스트 코드가 포함된 폴더입니다.
- `guachi.egg-info/`: 패키지 빌드 시 생성되는 메타데이터 정보가 저장된 폴더입니다.

## docs/
- `build/`: Sphinx 등으로 빌드된 문서의 산출물이 저장됩니다.
  - `doctrees/`: 문서 빌드 중간 산출물
  - `html/`: HTML 문서 결과물 및 정적 파일
- `source/`: 문서의 원본 소스(rst, conf.py 등)
  - `_static/`: 커스텀 CSS 등 정적 리소스

## guachi/
- `__init__.py`, `config.py`, `database.py`: Python 모듈 소스 코드
- `tests/`: 각종 테스트 코드

## guachi.egg-info/
- 패키지 메타데이터 파일들

---

이 폴더는 기존 `legacy` 폴더의 구조와 동일하며, 향후 업그레이드/리팩토링 작업을 위한 베이스로 활용할 수 있습니다.
