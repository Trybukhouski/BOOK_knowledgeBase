# BRANCHES

### BRANCHES >> About
- У репозитория может иметься несколько веток для разработки

### BRANCHES >> Syntax >> View
- Просмотр всех веток репозитория:

  ```
  git branch
  ```

### BRANCHES >> Syntax >> Creation
- Создание новой ветки:

  ```
  git branch <new-branch-name>
  ```
- Создание новой ветки и автоматический переход на нее:
  - от HEAD

  ```
  git checkout -b <new-branch-name>
  ```
  - от указанной ветки

  ```
  git checkout -b ＜new-branch-name＞ ＜existing-branch＞
  ```

### BRANCHES >> Syntax >> Modification
- Слияние изменений из другой ветки в текущую:

  ```
  git merge <merged-branche>
  ```
  - Объединяет ветки с сохранением истории коммитов интегрируемой ветки и создает результирующий коммит.
- Отмена слияния (возврат в pre-merge):

  ```
  git reset --hard HEAD
  ```
  - работает в случае, если merge не был закоммичен.
- Перебазирование изменений из текущей ветки в целевую:

  ```
  git rebase <branch-name>
  ```
  - Все коммиты из текущей ветки сжимаются в один «патч» и интегрируются в указанную ветку.
  - После перебазирования следует сделать `слияние перемоткой`.
- Удаление ветки

  ```
  git branch -d branch-name
  ```

### BRANCHES >> Syntax >> Moving
- Перемещение на конкретную существующую ветку:

  ```
  git checkout branch-name
  ```
  - в современных версиях команда позволяет переходить также и на ветки удаленного репозитория.