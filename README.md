# DevOps L06: Ansible Roles & CI

## Часть 1: Ansible Roles
Роль `nginx-vhosts` для установки nginx с виртуальными хостами (etis.com, fizfak.com, mehmat.ru).

## Часть 2: GitHub Actions
- `devops_course_pipeline.yml` — тестовый пайплайн.
- `lint.yml` — проверка Ansible-кода линтером.

## Запуск
```bash
ansible-playbook ./playbook.yml -i ./inventory.ini

---

## 🐙 Шаг 2. Создание репозитория на GitHub

1. Зайдите на **GitHub** (в браузере на Windows или внутри VM).
2. Нажмите **+ → New repository**.
3. **Repository name:** `lab_ansible_roles` (или любое другое).
4. **Description:** `DevOps L06: Ansible Roles & CI`.
5. **Public** (или Private, если препод требует — тогда не забудьте добавить его в Collaborators).
6. ❌ **НЕ** ставьте галочки «Add README», «Add .gitignore» (у нас уже есть файлы).
7. Нажмите **Create repository**.

**📸 Скриншот:** страница создания репозитория (пустая, с инструкциями).

---

## 📤 Шаг 3. Инициализация Git и первый пуш (на VM1)

Выполните в терминале VM1 (в папке `~/devops5_nginx_vhosts`):

```bash
git init
git add .
git commit -m "Initial commit: Ansible role nginx-vhosts"
