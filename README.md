# prometheus.learning
STEP 1
1. Установлено приложение Prometheus на базе Debian 11
2. Настроен запуск Prometheus как системного демона через /etc/systemd
3. Установлены экспортеры для целевой машины:
   * blackbox_exporter https://github.com/prometheus/blackbox_exporter/
   * node_exporter https://github.com/prometheus/node_exporter
   * mysql_exporter https://github.com/prometheus/mysqld_exporter
   * php-fpm_exporter https://github.com/bakins/php-fpm-exporter
   * nginx_exporter https://github.com/sysulq/nginx-vts-exporter
4. Собран конфигурационный файл prometheus.yml
5. Пуш проекта в гитхаб

STEP2
1. Установлена система долговременного хранения метрик Victoria Metrics (конфиг сервиса victoriametrics.service)
2. Настроен экспорт метрик на Victoria Metrics (обновлен файл конфига prometheus.yml)

STEP3
1. Добавлена конфигурация Alertmanager
   * alertmanager.yml
   * prometheus.rules.yml
   * отредактирован prometheus.yml для работы с Alertmanager
2. Добавлены systemd файлы сервисов

STEP4
1. Установлена Grafana
2. Настроены дашборды доступности сервисов и параметрох хостовой системы
   ![image](https://github.com/user-attachments/assets/e7982845-8679-496c-8a88-0ca970f0dfb8)
   ![image](https://github.com/user-attachments/assets/7c183314-c69b-47a2-ae29-cd58d17fc764)

