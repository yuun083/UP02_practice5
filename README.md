## Отчёт по практической работе №5
##### Тема: «Основы работы с системами контроля версий
##### Цель работы: научиться использовать систему контроля версий git при работке с программным кодом
1. Создаём аккаунт на https://github.com.
2. Нажимаем на "+" в шапке сайта и выбираем "New repository". В нвовом окне вводим имя репозитория и убираем добавление README.md.
3. Создаём на компьютере новый каталог(папку).
4. Выполняем команды:
   
   a. git init
   
      ```
      $ git init
      Initialized empty Git repository in C:/Users/yuun083/Desktop/UP02_PR5/.git/
      ```
      
  b. Создаём файл .gitignore и вводим туда текст, данный в практической работе. 
  
  c. git config user.name, git config user. email
  
      ```
      $ git config user.name "ataran"
      $ git config user.email jjjaa9099@gmail.com
      ```
   d. Отключение проверки сертификата
   
      ```
      $ git config --global http.sslVerify false
      ```
   e. git add
   
      ```
      $ git add .
      ```
   f. git commit
   
      ```
      $ git commit -m "Initial commit"
      [master (root-commit) 64768e7] Initial commit
      1 file changed, 9 insertions(+)
      create mode 100644 .gitignore
      ```
   g. git remote add
   
      ```
      $ git remote add origin https://github.com/yuun083/UP02_practice5.git
      ```
   h. git push -u
   
      ```
      $ git push -u origin master
      Enumerating objects: 3, done.
      Counting objects: 100% (3/3), done.
      Delta compression using up to 12 threads
      Compressing objects: 100% (2/2), done.
      Writing objects: 100% (3/3), 367 bytes | 183.00 KiB/s, done.
      Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
      To https://github.com/yuun083/UP02_practice5.git
       * [new branch]      master -> master
      branch 'master' set up to track 'origin/master'.
      ```
   i. Удаление credential manager
   
      ```
      $ git config --system --unset credential.helper
      ```
   j. Для GOGS
      ```
      $ git config --global http.postBuffer 157286400
      ```
5. Создаём в репозитории README.md и записываем команды с возвращаемым результатом.
