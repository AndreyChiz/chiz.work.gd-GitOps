# chiz.work.gd-k8s ☸️

[![Status](https://img.shields.io/badge/status-in%20development-yellow)](#)

> Инфрасттруктурный репозиорий сервера

## Доступные URLs

- http://chiz.work.gd - фронтенд
- http://chiz.work.gd/api - RESTfull api
- http://chiz.work.gd/api/docs - RESTfull api swagger documentation
- http://reg.chiz.work.gd - приватный docker репозиторрий
- http://reg.chiz.work.gd/ui - веб интерфейс приватного репозитория
- http://kub.chiz.work.gd - kube-apiserver




---

## 📂 Структура репозитория

### `clusters/`
Хранит конфигурации Kubernetes-кластеров:
-`staging/` — конфиги для соответствующих окружений  

### 'ext_env/' 
Конфиги для cluster-extanded окружений (внешний прокси, тунель...)
---

## ⚡ Использование

### Локальный кластер (kind)
```bash
# Развернуть локальный кластер
sudo kubectl create cluster  --config=clusters/dev/cluster-config.yaml

📝 В разработке

⚠️ Этот проект пока в разработке. Структура и функционал могут изменяться.
