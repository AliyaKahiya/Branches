1. На локальном репозитории сделать ветки для:
- Postman
- Jmeter
- CheckLists
- Bag Reports
- SQL
- Charles
- Mobile testing

   a) Создать внешний репозиторий c названием Branches.

   b) Перейти в GitBash

    $ mkdir BRANCHES
   
    $ cd BRANCHES
   
    $ git clone https://github.com/AliyaKahiya/Branches.git
   
    $ cd Branches
   
    $ git branch Postman; git branch Jmeter; git branch CheckLists; git branch Bag_Reports; git branch SQL; git branch Charles; git branch Mobile_Testing
   
2. Запушить все ветки на внешний репозиторий

    $ git push -u origin Postman Jmeter CheckLists Bag_Reports SQL Charles Mobile_Testing

3. В ветке Bag Reports сделать текстовый документ со структурой баг репорта

   a) Перейти на ветку Bag_Reports
   
    $ git checkout Bag_Reports
      
   b) Создать текстовый файл с атрибутами баг-репорта
   
    $ cat >> structure_of_bag_report.txt
      
	   1. Summary
	
	   2. Description
	
	   3. Actual_result
	
	   4. Expected_result
	
	   5. Attachments
	
	   6. Priority
	
	   7. Severity
	
	   8. Status
	
	   Ctrl+C
     
4. Запушить структуру багрепорта на внешний репозиторий

    $ git add structure_of_bag_report.txt && git commit -m "Add new file with bag report attributes" && git push

5. Вмержить ветку Bag Reports в Main

   a) Перейти на ветку main
   
    $ git checkout main
      
   b) Вмержить ветку Bag_Reports в main

    $ git merge Bag_Reports

6. Запушить main на внешний репозиторий.

    $ git push -u origin main

7. В ветке CheckLists набросать структуру чек листа.
   
  a) Перейти на ветку CheckLists
     
    $ git checkout CheckLists

  b) Набросать структуру чек листа.
   
	  $ cat >> structure_of_check_list.txt
  
     1. Functional_testing
	
	   2. Integration_testing
	
	   3. Security_testing
	
	   4. Localization_testing
	
	   5. Globalization_testing
	
	   6. Usability_testing
	
	   7. Cross_platform_testing

8. Запушить структуру на внешний репозиторий

    $ git add structure_of_check_list.txt && git commit -m "Add new file with structure of check list" && git push

9. На внешнем репозитории сделать Pull Request ветки CheckLists в main

   a) На внешнем репозитории перейти на ветку CheckLists.
   
   b) Нажать Pull Requests
   
   c) Нажать Compare&pull request
   
   d) Нажать Create pull request
   
   e) Нажать merge pull request 

10. Синхронизировать Внешнюю и Локальную ветки Main

    $ git pull
    
