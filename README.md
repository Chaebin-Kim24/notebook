# 주피터 노트북

![Github Actions Status](https://github.com/jupyter/notebook/workflows/Build/badge.svg)
[![Documentation Status](https://readthedocs.org/projects/jupyter-notebook/badge/?version=latest)](https://jupyter-notebook.readthedocs.io/en/latest/?badge=latest)
[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/jupyter/notebook/main?urlpath=tree)
[![Gitpod](https://img.shields.io/badge/gitpod_editor-open-blue.svg)](https://gitpod.io/#https://github.com/jupyter/notebook)

주피터 노트북은 대화형 컴퓨팅을 위한 웹 기반 노트북 환경입니다.

![Jupyter notebook example](docs/resources/running_code_med.png '주피터 노트북 화면')

## 소프트웨어 버전

우리는 **주피터 노트북의 최신 버전**인 클래식 노트북 v6와 노트북 v7만 관리합니다
노트북 v5는 더이상 관리되지 않습니다.
모든 노트북 v5 유저들은 최대한 빨리 클래식 노트북 v6로 업그레이드 할 것이 권장됩니다.

노트북 v7으로 업그레이드 하는 것은, 확장 코드를 쓰고 있는 경우 추가 작업이 필요한데, 그 이유는
노트북 v5나 클래식 노트북 v6에서 동작하는 코드가 노트북 v7에서는 호환되지 않기 때문입니다.

### 노트북 v7

새로운 버전의 노트북의 구성요소는:

- 프론트엔드를 위한 주피터랩 구성요소
- 파이썬 서버를 위한 주피터 서버

입니다. 이는 `주피터/노트북` 코드에 상당히 많은 변화가 있을을 뜻합니다.

노트북 v7: https://jupyter.org/enhancement-proposals/79-notebook-v7/notebook-v7.html

### 클래식 노트북 v6

유지보수 및 보안 관련 이슈는 [한정적으로](https://github.com/jupyter/notebook-team-compass/issues/5#issuecomment-1085254000) [`6.5.x`](https://github.com/jupyter/notebook/tree/6.5.x) 버전에서만 처리되고 있습니다.
이 버전은 [`nbclassic`](https://github.com/jupyter/nbclassic)에서 HTML/JavaScript/CSS 관련 자원을 가져옵니다.

새로운 기능과 지속적인 개선은 노트북 v7에 집중합니다(윗 섹션을 보세요). 

새로운 기능을 개발해서 본 깃허브 저장소에 코드 기여 신청을 했거나 신청할 예정이라면, 주피터 서버와 주비터랩 구조로 전환하고, 주피터 서버 확장팩 / 주피터랩 확장팩으로 배포할 것을 권장합니다. 이 방법을 쓰면 새로운 노트북 v7과도 개발된 기능이 호환될 수 있습니다. 

## 주피터 노트북, 프로그래밍 언어에 무관하게 진화된 IPython 노트북

주피터 노트북은 프로젝트 주피터의 프로그래밍 언어에 무관한 HTML 노트북 애플리케션 입니다.
2015년, 주피터 노트북은 IPython 코드의 Big Split™의 일부로 출시됐습니다. 
IPython 3가 프로그래밍 언어에 무관한 코드인 _IPython 노트북_ 과 프로그램 특이적 코드인
_IPython 파이썬 커널_ 이 같이 들어있는 마지막 버전이었습니다. 다양한 프로그래밍 언어가 사용됨에 따라, 
프로젝트 주피터는 프로그래밍 언어에 무관한 **주피터 노트북**을 본 저장소에서 계속 개발해 나갈 것이며, 
프로그래밍 언어에 특이적인 커널은 커뮤니티 구성원들의 도움을 받아 각자의 저장소에서 개발됩니다. 

- [Big Split™ 공지](https://blog.jupyter.org/the-big-split-9d7b88a031a7)
- [주피터의 비상 블로그 포스트](https://blog.jupyter.org/jupyter-ascending-1bf5b362d97e)

## 설치

설치 관련 문서는
[주피터 플랫폼, ReadTheDocs 블로그](https://jupyter.readthedocs.io/en/latest/install.html)에서 찾아볼 수 있습니다.
주피터 노트북의 고급 사용법에 대한 문서는 
[여기](https://jupyter-notebook.readthedocs.io/en/latest/)에 있습니다.

설치를 하기 전 먼저
[pip 설치](https://pip.readthedocs.io/en/stable/installing/)가 되었는지 확인하고 명령 프롬프트에서 다음 명령어를 실행합니다:

```bash
pip install notebook
```

## 사용법 - 주피터 노트북 실행하기

### 일반 설치를 했을 때

명렁 프롬프트에서 다음 명령어를 실행합니다:

```bash
jupyter notebook
```

### 원격 설치를 했을 때

주피터 노트북을 원격으로 실행하기 위해서는 추가 설정이 필요합니다. See [노트](https://jupyter-server.readthedocs.io/en/latest/operators/public-server.html).

## Development Installation

See [`CONTRIBUTING.md`](CONTRIBUTING.md) for how to set up a local development installation.

## Contributing

If you are interested in contributing to the project, see [`CONTRIBUTING.md`](CONTRIBUTING.md).

## Community Guidelines and Code of Conduct

This repository is a Jupyter project and follows the Jupyter
[Community Guides and Code of Conduct](https://jupyter.readthedocs.io/en/latest/community/content-community.html).

## Resources

- [Project Jupyter website](https://jupyter.org)
- [Online Demo at jupyter.org/try](https://jupyter.org/try)
- [Documentation for Jupyter notebook](https://jupyter-notebook.readthedocs.io/en/latest/)
- [Korean Version of Installation](https://github.com/ChungJooHo/Jupyter_Kor_doc/)
- [Documentation for Project Jupyter](https://jupyter.readthedocs.io/en/latest/index.html)
- [Issues](https://github.com/jupyter/notebook/issues)
- [Technical support - Jupyter Google Group](https://discourse.jupyter.org/)

## About the Jupyter Development Team

The Jupyter Development Team is the set of all contributors to the Jupyter project.
This includes all of the Jupyter subprojects.

The core team that coordinates development on GitHub can be found here:
https://github.com/jupyter/.

## Our Copyright Policy

Jupyter uses a shared copyright model. Each contributor maintains copyright
over their contributions to Jupyter. But, it is important to note that these
contributions are typically only changes to the repositories. Thus, the Jupyter
source code, in its entirety is not the copyright of any single person or
institution. Instead, it is the collective copyright of the entire Jupyter
Development Team. If individual contributors want to maintain a record of what
changes/contributions they have specific copyright on, they should indicate
their copyright in the commit message of the change, when they commit the
change to one of the Jupyter repositories.

With this in mind, the following banner should be used in any source code file
to indicate the copyright and license terms:

```
# Copyright (c) Jupyter Development Team.
# Distributed under the terms of the Modified BSD License.
```
