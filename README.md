### Hexlet tests and linter status:
[![Actions Status](https://github.com/bahtiyar0/frontend-project-46/actions/workflows/hexlet-check.yml/badge.svg)](https://github.com/bahtiyar0/frontend-project-46/actions)

[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)


[![Maintainability](https://api.codeclimate.com/v1/badges/7cfd79ce778f0eaa874b/maintainability)](https://codeclimate.com/github/bahtiyar0/frontend-project-46/maintainability)


Вычислитель отличий – программа, определяющая разницу между двумя структурами данных. Это популярная задача, для решения которой существует множество онлайн сервисов, например http://www.jsondiff.com/. Подобный механизм используется при выводе тестов или при автоматическом отслеживании изменений в конфигурационных файлах.
https://ru.hexlet.io/programs/frontend/projects/46


Возможности утилиты:

Поддержка разных входных форматов: yaml, json
Генерация отчета в виде plain text, stylish и json

Требования:
Требуется node.js версия 13.2.0 и выше (проверить версию установленной node возможно командой в терминале node -v)

Установка:
1. Клонируйте данный репозиторий командой: git clone git@github.com:bahtiyar0/frontend-project-46.git
2. Выполните установку командой: npm link


Аргументы и опции

node bin/gendiff -h 

<a href="https://asciinema.org/a/8BQw2FWHxu7RSkXtoQ05hbL3b" target="_blank"><img src="https://asciinema.org/a/8BQw2FWHxu7RSkXtoQ05hbL3b.svg" /></a>


Рекурсивное сравнение

bin/gendiff.js __fixtures__/filepath1.json __fixtures__/filepath2.json


<a href="https://asciinema.org/a/yB3AXFG5By3UsVN0V4M640vqz" target="_blank"><img src="https://asciinema.org/a/yB3AXFG5By3UsVN0V4M640vqz.svg" /></a>



Сравнение плоских файлов (JSON)

bin/gendiff.js __fixtures__/filepath1.json __fixtures__/filepath2.json

<a href="https://asciinema.org/a/0DD0N2mJB055iZFlsP4Fzv5pJ" target="_blank"><img src="https://asciinema.org/a/0DD0N2mJB055iZFlsP4Fzv5pJ.svg" /></a>


Сравнение плоских файлов (yaml)

bin/gendiff.js __fixtures__/filepath1.yaml __fixtures__/filepath2.yaml

[![asciicast](https://asciinema.org/a/HTtHuGUVpuWtvAcylL6w5clcn.svg)](https://asciinema.org/a/HTtHuGUVpuWtvAcylL6w5clcn)


Плоский формат

node bin/gendiff -f plain  __fixtures__/filepath1.yaml __fixtures__/filepath2.yaml

[![asciicast](https://asciinema.org/a/P5nBH2xOpJyIurzwD8CiYaUGF.svg)](https://asciinema.org/a/P5nBH2xOpJyIurzwD8CiYaUGF)


Вывод в json

bin/gendiff.js --format json __fixtures__/filepath1.json __fixtures__/filepath2.json

[![asciicast](https://asciinema.org/a/EzbQuDx0sxcUURFp4Eo8NJYKo.svg)](https://asciinema.org/a/EzbQuDx0sxcUURFp4Eo8NJYKo)
