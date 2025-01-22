# Custom Components and Integrations for Home Assistant

[![](https://img.shields.io/github/license/coichedid/coichedid-custom-component?style=for-the-badge)](LICENSE)
[![](https://img.shields.io/github/actions/workflow/status/coichedid/coichedid-custom-component/pythonpackage.yaml?branch=main)](https://github.com/coichedid/coichedid-custom-component/actions)

## About

This repo contains a several custom components and integrations for [Home Assistant](https://www.home-assistant.io) that was created to abstract some unsupported Tuya devices.

Thanks for tutorial series
on [aarongodfrey.dev](https://aarongodfrey.dev/home%20automation/building_a_home_assistant_custom_component_part_1/).

Under folder [custom_components](https://github.com/coichedid/coichedid-custom-component/custom_components) it's possible to find those components.

## What It Is

Under construction.

## Running Tests

To run the test suite create a virtualenv (I recommend checking out [pyenv](https://github.com/pyenv/pyenv) and [pyenv-virtualenv](https://github.com/pyenv/pyenv-virtualenv) for this) and install the test requirements.

```bash
$ pip install -r requirements.test.txt
```

After the test dependencies are installed you can simply invoke `pytest` to run
the test suite.

```bash
$ pytest
Test session starts (platform: linux, Python 3.7.5, pytest 5.4.3, pytest-sugar 0.9.3)
rootdir: /home/dev/projects/github-custom, inifile: setup.cfg, testpaths: tests
plugins: cov-2.9.0, aiohttp-0.3.0, requests-mock-1.8.0, homeassistant-0.1.1, timeout-1.3.4, sugar-0.9.3
collecting ...
 tests/test_sensor.py ✓✓✓✓✓✓✓                                                                                                                                                  100% ██████████

----------- coverage: platform linux, python 3.7.5-final-0 -----------
Name                                          Stmts   Miss  Cover   Missing
---------------------------------------------------------------------------
custom_components/__init__.py                     0      0   100%
custom_components/github_custom/__init__.py       0      0   100%
custom_components/github_custom/const.py         17      0   100%
custom_components/github_custom/sensor.py       110      7    94%   92-95, 113, 118, 127
---------------------------------------------------------------------------
TOTAL                                           127      7    94%


Results (0.14s):
       7 passed
```