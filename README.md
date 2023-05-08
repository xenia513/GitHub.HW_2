# GitHub.HW_2

## Homework to the second GIT lesson 

### 1. На локальном репозитории сделать ветки для:
- Postman
- Jmeter
- CheckLists
- BugReports
- SQL
- Charles
- Mobile testing

    $ git branch Postman
    $ git branch Jmeter
    $ git branch CheckLists
    $ git branch BugReports
    $ git branch SQL
    $ git branch Charles
    $ git branch MobileTesting

### 2. Запушить все ветки на внешний репозиторий

    $ git push --all

### 3. В ветке BugReports сделать текстовый документ со структурой баг репорта

    $ touch BugReport.txt
    $ vim BugReport.txt
  
Эта команда открывает встроенный редактор текста, для начала редактирования необходимо нажать `i` и ввести текст:

    ID -
    Severity - 
    Environment - 
    Title - 
    Precondition -
    Steps - 
      1:
      2:
      3:
      4:
      5:
      6:
      7: 
    Postcondition -
    Expected Result - 
    Actual Result -  
    Attachment - 
    Author - 

После завершения редактирования нажимаем `Esc` и `:wq` для сохранения внесенных изменений и выхода из режима редактора.

### 4. Запушить структуру багрепорта на внешний репозиторий

    $ git add .
    $ git commit -m "created BugReport.txt"
    $ git push

### 5. Вмержить ветку Bag Reports в Main

    $ git checkout main
    $ git merge BugReports

### 6. Запушить main на внешний репозиторий

    $ git push

### 7. В ветке CheckLists набросать структуру чек листа

    $ git checkout CheckLists
    $ cat > checkList.txt
    1. ID
    2. Название
    3. Предусловия
    4. Название проверки 
    5. Тестовые данные (при необходимости)
    6. Ожидаемый результат
    7. Имя тестировщика
    8. Дата и время прохождения чек-листа
    9. Статус проверки
    10. Комментарий
Для завершения редактирования нажимаем `Enter` и `Ctrl+C`

### 8. Запушить структуру на внешний репозиторий

    $ git add .
    $ git commit -m "created checkList.txt"
    $ git push

### 9. На внешнем репозитории сделать Pull Request ветки CheckLists в main

    Repositories >> GitHub.HW_2 >> Pull Requests >> New pull request >> choose branches to be merged >> Create pull request

### 10. Синхронизировать Внешнюю и Локальную ветки Main

    $ git pull
