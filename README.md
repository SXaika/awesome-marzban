
# Awesome Marzban

## Содержание
1. [Основное](#Основное)
2. [Бекап](#Бекап)
   - [Бекап панели](#Бекап-панели)
   - [Бекап логов](#Бекап-логов)
3. [Миграция](#Миграция)
4. [Ограничение пользователей](#Ограничение-пользователей)
5. [Шаблоны подписок](#Шаблоны-подписок)
6. [Сканеры SNI](#Сканеры-SNI)
7. [Скрипты теста скорости, проверки доступности](#Скрипты-теста-скорости-проверки-доступности)
8. [API](#API)
9. [Коммерция/боты](#Коммерцияботы)
10. [Управление пользователями](#Управление-пользователями)
11. [Аналитика/мониторинг](#Аналитикамониторинг)
12. [Генераторы inbound'ов](#Генераторы-inboundов)
13. [Автоматизация](#Автоматизация)
14. [Другие утилиты](#Другие-утилиты)

## Основное
- [Блок о прокси](https://marzban.dev/)
- [GitHub Marzban](https://github.com/Gozargah/Marzban)
- [Документация Marzban на русском](https://marzban-docs.sm1ky.com)
- [Группа Marzban в Telegram](https://t.me/gozargah_marzban)

## Бекап
### Бекап панели
- [Backuper](https://github.com/erfjab/Backuper)
- [Marzban backup (Telegram)](https://github.com/jomertix/marzban-tools/tree/master/backup/marzban)
- [Marzban backup (rclone)](https://github.com/ElitraProject/marzban-backup)
- [Marzban backup (Telegram, Discord)](https://github.com/M03ED/Marzban_Backup)
- [AC-Lover](https://github.com/AC-Lover/backup)
- [Marzban backup (логи + панель)](https://github.com/terbyn/Marzban_logs_backupTG)

### Бекап логов
- [Logs backup (Telegram)](https://github.com/jomertix/marzban-tools/tree/master/backup/logs)
- [Marzban backup (логи + панель)](https://github.com/terbyn/Marzban_logs_backupTG)

## Миграция
- [X-UI -> Marzban](https://github.com/ItsAML/X-Ui-to-Marzban)
- [Hiddify -> Marzban](https://github.com/ItsAML/Hiddify-To-Marzban)
- [SQLite -> MySQL](https://github.com/mobinalipour/marzban-to-mysql)

## Ограничение пользователей
- [V2IpLimit](https://github.com/houshmand-2005/V2IpLimit) - при достижении лимита подключений блокируется аккаунт
- [luIP-marzban (UFW)](https://github.com/sm1ky/luIP-marzban) - при достижении лимита блокируются только новые подключения
- [luIP-marzban (iptables)](https://github.com/mmdzov/luIP-marzban) - при достижении лимита блокируются только новые подключения. Устаревший проект, не рекомендуется к использованию на проде

## Шаблоны подписок
- [Minimalistic Sub Page](https://github.com/jomertix/marzban-tools/tree/master/subscription)
- [Marzbanify Template](https://github.com/dermv/marzbanify-template)
- [x0sina sub](https://github.com/x0sina/marzban-sub)
- [marzban-sub-ru](https://github.com/DigneZzZ/marzban-sub-ru)
- [Clash](https://github.com/mahanmi/iran-clash-example)
- [Sing-box](https://github.com/oXIIIo/marzban-template)
- [marzban-custom-home](https://github.com/LibernetDigital/marzban-custom-home)
- [confluence-marzban-home](https://github.com/sm1ky/confluence-marzban-home)
- [marzban-sub](https://github.com/sm1ky/marzban-sub)

## Сканеры SNI
- [RealiTLScanner](https://github.com/XTLS/RealiTLScanner)
- [SNI-Finder (TLS 1.3, HTTP/2 with TLS Ping)](https://github.com/v-kamerdinerov/SNI-Finder)
- [SNI-Checker (TLS 1.3, HTTP/2)](https://github.com/jomertix/SNI-Checker)
- [SNI-Checker (only TLS 1.3)](https://github.com/ElitraProject/SNI-Checker)

## Скрипты теста скорости, проверки доступности
Тест доступности сервисов на сервере:
```bash
bash <(curl -L -s https://bench.openode.xyz/checker.sh)
```
Тест для проверки Instagram:
```bash
bash <(curl -L -s https://bench.openode.xyz/checker_inst.sh)
```
Бенчмарк скорости:
```bash
wget -qO - bench.sh | bash
```
Бенчмарк скорости (регионы России):
```bash
wget -qO- https://raw.githubusercontent.com/jomertix/server-scripts/refs/heads/master/speedtest/countries/speedtest_ru.sh | bash
```
Тест доступности сервисов (Stream Platforms & Game Regions):
```bash
bash <(curl -L -s https://git.io/JRw8R) -E en -M 4
```
Проверка блокировки IP зарубежными сервисами
```bash
bash <(curl -Ls IP.Check.Place) -l en
```

### Другие скрипты
Смена ядра Xray:
```bash
bash <(wget -qO- https://raw.githubusercontent.com/DigneZzZ/marzban_core_change/main/core.sh)
```
Проверка системы на совместимость с Xanmod BBR3:
```bash
wget -qO- https://cdn.sm1ky.pl/s/9qFbTF3MKr9W2o3/download | awk -f -
```
Автоматическая установка Xanmod BBR3:
```bash
bash <(curl -fsSL https://cdn.sm1ky.pl/s/FGdCjrpHbQ5Rq3b/download)
```

Другие скрипты смотрите [здесь](https://github.com/Gozargah/Marzban-scripts/)

## API
- [marzpy](https://github.com/mewhrzad/marzpy)
- [marzban-api-client](https://github.com/oXIIIo/marzban-api-client)
- [marzban](https://github.com/sm1ky/marzban_api)
- [aiomarzban](https://github.com/P1nk-L0rD/aiomarzban)
- [MarzJS](https://github.com/maniwrld/marzjs)
- [marzban-sdk](https://www.npmjs.com/package/marzban-sdk?activeTab=readme) (TypeScript)

## Коммерция/боты
- [marzban-shop](https://github.com/gunsh1p/marzban-shop)
- [SHM](https://github.com/danuk/shm)
- [botmirzapanel](https://github.com/mahdiMGF2/botmirzapanel)

## Управление пользователями
- [MarzbanExpiredUserRemover](https://github.com/ItsAML/MarzbanExpiredUserRemover)
- [Marzban_Inbound_Updater](https://github.com/M03ED/Marzban_Inbound_Updater)
- [Marzban_Flow_Select](https://github.com/M03ED/Marzban_Flow_Select)
- [holderbot](https://github.com/erfjab/holderbot)

## Аналитика/мониторинг
- [xray-checker](https://github.com/kutovoys/xray-checker)
- [marzban-node-monitor](https://github.com/sm1ky/marzban-node-monitor)
- [marzban_sqlite_streamlit](https://github.com/lifeindarkside/marzban_sqlite_streamlit)
- [marzban-grafana-pannel](https://github.com/lifeindarkside/marzban-grafana-pannel)
- [marzban-exporter](https://github.com/kutovoys/marzban-exporter)
- [xray-logger](https://github.com/likstanov/xray-logger)

## Генераторы inbound'ов
- [MarzbanInboundGenerator](https://azavaxhuman.github.io/MarzbanInboundGenerator/v2)
- [Marzban-Reality-Generator](https://azavaxhuman.github.io/Marzban-Reality-Generator)

## Автоматизация
- [marzban-haproxy-ansible](https://github.com/v-kamerdinerov/marzban-haproxy-ansible) - набор Ansible ролей для автоматической настройки Marzban.

## Другие утилиты
- [xray-torrent-blocker](https://github.com/kutovoys/xray-torrent-blocker)
