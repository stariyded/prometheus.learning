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
