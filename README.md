1. На локальном репозитории сделать ветки для:
 
 * Postman - git branch Postman
 
 * Jmeter - git branch Jmeter
 
 * CheckLists - git branch CheckLists
 
 * Bug Reports - git branch Bug_Reports
 
 * SQL -  git branch SQL
 
 * Charles - git branch Charles
 
 * Mobile testing - git branch Mobile_testing

 2. Запушить все ветки на внешний репозиторий
 
 * git push -u origin --all
 
 3. В ветке Bug Reports сделать текстовый документ со структурой баг репорта
  
 * git checkout Bug_Reports (перейти на ветку)

 * cat > bug_report.txt
  ID
  Summary
  Pre-conditions
  Steps to reproduce
  Actual result
  Expected result
  Attachment
  Severity
  Reporter
  Notes
  
  Ctrl+C

 4. Запушить структуру багрепорта на внешний репозиторий
 
 * git add bug_report.txt
 * git commit -m "add bug_report_1.txt"
 * git push

 5. Вмержить ветку Bag Reports в Main
 
 * git checkout main
 * git merge Bug_Reports

 6. Запушить main на внешний репозиторий.
 
 *git add .
 *git commit -m "merge 1 branch"
 *git push

 7. В ветке CheckLists набросать структуру чек листа.
 
 *git checkout CheckLists
 
 *cat > check_list.txt
  ID
  Title
  Precondition
  Module
  Steps_to_reproduce
  Expected_result
  Status
 
  Ctrl+C
 
 8. Запушить структуру на внешний репозиторий
 
 *git add check_list.txt
 *git commit -m "add  check_list_1.txt"
 *git push
 
 9. На внешнем репозитории сделать Pull Request ветки CheckLists в main
 *Открываем внешний репозиторий и нажимаем кнопку Compare & pull request
 *Оставляем комментарий в графе Write : add a lot of lines
 *Нажимаем кнопку Create pull request
 *Нажимаем кнопку Merge pull request
 *Нажимаем кнопку Confirm merge
 
 10. Синхронизировать Внешнюю и Локальную ветки Main
 *Переходим на локальный репозиторий
 *git checkout main
 *git pull
