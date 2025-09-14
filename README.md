# chiz.work.gd-k8s ☸️

[![Status](https://img.shields.io/badge/status-in%20development-yellow)](#)

> Infrastructure repository for managing Kubernetes clusters and application deployment.  
> Репозиторий находится в активной разработке.

---

## 📂 Структура репозитория

### `clusters/`
Хранит конфигурации Kubernetes-кластеров:
- `kind/` — локальные кластеры для разработки  
- `dev/`, `staging/`, `prod/` — конфиги для соответствующих окружений  

### `k8s/`
Kubernetes манифесты для приложений:
- `base/` — общие манифесты (Deployment, Service, ConfigMap, Secret)  
- `overlays/` — окруженчески-специфичные конфигурации  
- `helm/` — Helm charts для упрощённого деплоя и управления версиями  

### `terraform/`
Конфигурации Terraform для управления облачной инфраструктурой:  
виртуальные машины, сети, хранилища, балансировщики нагрузки  

### `ci/`
Скрипты и пайплайны CI/CD для автоматизации деплоя:  
- сборка Docker-образов  
- применение Kubernetes манифестов  
- тестирование и проверка окружений  

---

## ⚡ Использование

### Локальный кластер (kind)
```bash
# Развернуть локальный кластер
kind create cluster --name my-cluster --config clusters/kind/kind-config.yaml

📝 В разработке

⚠️ Этот проект пока в разработке. Структура и функционал могут изменяться.
