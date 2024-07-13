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

New features and continuous improvement is now focused on Notebook v7 (see section above).

If you have an open pull request with a new feature or if you were planning to open one, we encourage switching over to the Jupyter Server and JupyterLab architecture, and distribute it as a server extension and / or JupyterLab prebuilt extension. That way your new feature will also be compatible with the new Notebook v7.

## Jupyter notebook, the language-agnostic evolution of IPython notebook

Jupyter notebook is a language-agnostic HTML notebook application for
Project Jupyter. In 2015, Jupyter notebook was released as a part of
The Big Split™ of the IPython codebase. IPython 3 was the last major monolithic
release containing both language-agnostic code, such as the _IPython notebook_,
and language specific code, such as the _IPython kernel for Python_. As
computing spans across many languages, Project Jupyter will continue to develop the
language-agnostic **Jupyter notebook** in this repo and with the help of the
community develop language specific kernels which are found in their own
discrete repos.

- [The Big Split™ announcement](https://blog.jupyter.org/the-big-split-9d7b88a031a7)
- [Jupyter Ascending blog post](https://blog.jupyter.org/jupyter-ascending-1bf5b362d97e)

## Installation

You can find the installation documentation for the
[Jupyter platform, on ReadTheDocs](https://jupyter.readthedocs.io/en/latest/install.html).
The documentation for advanced usage of Jupyter notebook can be found
[here](https://jupyter-notebook.readthedocs.io/en/latest/).

For a local installation, make sure you have
[pip installed](https://pip.readthedocs.io/en/stable/installing/) and run:

```bash
pip install notebook
```

## Usage - Running Jupyter notebook

### Running in a local installation

Launch with:

```bash
jupyter notebook
```

### Running in a remote installation

You need some configuration before starting Jupyter notebook remotely. See [Running a notebook server](https://jupyter-server.readthedocs.io/en/latest/operators/public-server.html).

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
