# README.md

## Цели проекта

Этот проект создан для упрощения процесса мониторинга и визуализации данных, предоставляя пользователям возможность:
- Быстро развернуть систему мониторинга без значительных затрат времени и усилий.
- Получать актуальные метрики в реальном времени через удобный интерфейс Grafana.
- Настраивать уведомления о возникновении проблем для быстрого реагирования.
Проект является отличной основой для дальнейшего расширения функционала и интеграции с другими инструментами в сфере DevOps.

## Описание проекта

Проект реализован с использованием Docker Compose и включает несколько сервисов для мониторинга и DNS-резолвинга. В состав проекта входят следующие компоненты:

- **CoreDNS**: DNS-сервер, предназначенный для управления доменными именами.
- **Prometheus**: Система для мониторинга и сбора метрик.
- **Node Exporter**: Экспортёр метрик, позволяющий отслеживать состояние серверов.
- **Grafana**: Платформа для визуализации данных и создания графиков.

## Структура проекта

- `/coredns`
- `/prometheus`
- `/grafana`
- `/docker-compose.yaml`
- `/README.md`

## Компоненты проекта

- **CoreDNS**: DNS-сервер для управления доменными именами.
- **Prometheus**: Инструмент для сбора и мониторинга метрик, обеспечивающий возможность отслеживания состояния ваших сервисов.
- **Grafana**: Платформа для визуализации данных, позволяющая создавать графики и дашборды на основе собранных метрик.
- **Docker**: Используется для контейнеризации приложений.
- **Docker Compose**: Инструмент для управления многоконтейнерными приложениями.

## Запуск проекта

1. Убедитесь, что Docker и Docker Compose установлены на вашем компьютере.
2. Склонируйте репозиторий или загрузите файлы проекта.
3. Перейдите в директорию, где расположен файл `docker-compose.yaml`.
4. Выполните команду:

   ```bash
   docker-compose up -d
   ```

## Порты

| Сервис       | Порт (хост) | Порт (контейнер) |
|--------------|-------------|-------------------|
| CoreDNS      | 5053        | 53                |
| Prometheus   | 9090        | 9090              |
| Grafana      | 3000        | 3000              |

## Завершение работы

Для остановки и удаления контейнеров выполните команду:

```bash
docker-compose down
``` 

Теперь ваш проект настроен и готов к использованию.