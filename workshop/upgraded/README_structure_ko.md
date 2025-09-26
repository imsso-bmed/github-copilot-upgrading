# upgraded 폴더 구조 설명

`upgraded` 폴더는 레거시(`legacy`) 폴더의 전체 파일과 디렉터리 구조를 복사한 것으로, Python 프로젝트의 업그레이드 실습을 위한 베이스입니다.

## 주요 파일 및 폴더

- **MANIFEST.in**: 패키징 시 포함할 파일 목록을 지정하는 설정 파일
- **README.rst**: 프로젝트 설명서
- **distribute-0.6.10.tar.gz**: 예전 Python 패키징 도구인 distribute의 소스 아카이브
- **distribute_setup.py**: distribute 설치 스크립트
- **setup.py**: Python 패키지 설치 및 배포를 위한 스크립트
- **docs/**: Sphinx 기반 문서 소스 및 빌드 결과물
  - **build/**: 빌드된 문서(HTML, doctree 등)
  - **source/**: 문서 원본(rst, conf.py 등)
- **guachi/**: 실제 Python 패키지 소스 코드
  - **__init__.py, config.py, database.py**: 패키지 모듈
  - **tests/**: 단위 테스트 및 통합 테스트 코드
- **guachi.egg-info/**: setuptools로 패키징 시 생성되는 메타데이터

## 활용 목적

이 구조는 레거시 Python 프로젝트를 최신 개발 환경에 맞게 업그레이드하는 실습의 출발점으로 사용됩니다. 각 파일과 폴더는 실제 업그레이드 작업(문법 변환, 패키징 방식 변경, 테스트 개선 등)에 활용됩니다.
