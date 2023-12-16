# git

Git is a version control system that makes easier for members of a team to collaborate with one another.

## Task 1

##### Creating, cloning, pushing and pulling repositories  
```git

1. Создать свой репозиторий в таким же именем, как и имя пользователя
$ curl -u 'buksha-evgenia' https://api.github.com/user/repos -d '{"name":"buksha-evgenia"}'

2. Склонировать его на свой компьютер в отдельную папку
$ git clone git@github.com:buksha-evgenia/buksha-evgenia.git

3. Склонировать себе следующий репозиторий в отдельную папку https://github.com/testrusau/testrusau
$ git clone git@github.com:testrusau/testrusau.git

4. Скопировать данные из склонированного репозитория и вставить их в ваш репозиторий из шага 2
cd testrusau 
git push git@github.com:osukhorukova/testrusau.git main:main

5. Открыть файл README.md и поочередно заменить каждый блок на вашу информацию. Каждое изменений блока делайте через отдельный коммит.
git commit -m "buksha-evgenia/adding info"
git push
```

## Task 2

##### Creating, adding remote repositories  
```git
1. Создание локального репозитория и объявление его удаленным
git init web_testing
git remote add web_testing https://github.com/buksha-evgenia/web_testing.git 

2. Добавление в файл README.md нового блока Testing Artefacts 
README.md (manual edit)   

3. Внесение изменений в удаленный репозиторий                              
git commit -m "Update README.md"                 
git push                                                    
```
