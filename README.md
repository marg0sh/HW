## [HW_1](#1)
## [HW_3](#2)
  
======  
  
## HW_1.<a name="1"></a>
#### 1) Посмотреть где я
```
pwd
```

#### 2) Создать папку
```
mkdir p1
```

#### 3) Зайти в папку
```
cd p1
```

#### 4) Создать 3 папки
```
mkdir p2 p3 p4
```

#### 5) Зайти в любоую папку
```
cd p2
```

#### 6) Создать 5 файлов (3 txt, 2 json)
```
touch t1.txt t2.txt t3.txt j1.json j2.json
```

#### 7) Создать 3 папки
```
mkdir p5 p6 p7
```

#### 8) Вывести список содержимого папки
```
ls -la
```

#### 9) + Открыть любой txt файл
```
vim t1.txt
```

#### 10) + написать туда что-нибудь, любой текст.
*режим редактирования нажатием i*
```
123 
456
789
 
```

#### 11) + сохранить и выйти.
*нажатием Esc : w q Enter*

#### 12) Выйти из папки на уровень выше
```
cd ..
```

#### 13) переместить любые 2 файла, которые вы создали, в любую другую папку.
```
mv /c/Users/user/QA/p1/p2/{t1.txt,t2.txt} /c/Users/user/QA/p1/p3
```
*или*
```
mv p2/{t1.txt,t2.txt} p3
```
*или*
```
mv t1.txt t2.txt p3 
```

#### 14) скопировать любые 2 файла, которые вы создали, в любую другую папку.
```
cp /c/Users/user/QA/p1/p3/{t2.txt,t1.txt} /c/Users/user/QA/p1/p4
```
*или*
```
cp p3/{t2.txt,t1.txt} p4
```
*или*
```
cp t2.txt t1 txt p4
```

#### 15) Найти файл по имени
```
find . -name t1.txt
```

#### 16) просмотреть содержимое в реальном времени (команда grep) изучите как она работает.
```
tail -f p4/t1.txt |grep 'err'
```
*отслеживание только строк с 'err', выход по Ctrl+C*

#### 17) вывести несколько первых строк из текстового файла
```
head -n 3 p4/t1.txt
```

#### 18) вывести несколько последних строк из текстового файла
```
tail -n 3 p4/t1.txt
```

#### 19) просмотреть содержимое длинного файла (команда less) изучите как она работает.
```
less p4/t1.txt
```
*выход Q*

#### 20) вывести дату и время
```
date +%x" "%X
```
*или*
```
date +"%D %R"
```

 
  -----


## Задание *
#### 1) Отправить http запрос на сервер. http://162.55.220.72:5005/terminal-hw-request
```
curl ‘http://162.55.220.72:5005/terminal-hw-request’
```
*После получения ответа сервера, отправить повторный запрос*
```
curl ‘http://162.55.220.72:5005/get_method?name=Marg0shik&age=34’
```

#### 2) Написать скрипт который выполнит автоматически пункты 3, 4, 5, 6, 7, 8, 13
##### 1.Создать файл:
```
touch script.sh
```

##### 2.Изменить содержимое файла:
```
cat >script.sh 
#!/bin/bash 
cd p1 
mkdir p2 p3 p4 
cd p2 
touch t1.txt t2.txt t3.txt j1.json j2.json 
mkdir p5 p6 p7 
ls -la 
mv /c/Users/user/QA/p1/p2/{t1.txt,t2.txt} /c/Users/user/QA/p1/p3/

```

##### 3.Сохранить изменения и выйти из режима редактирования:
*выйти из режима редактирования нажатием Ctrl+C*

##### 4.Сделать файл "скриптом" исполняемым:
```
chmod +x ./script.sh 
```

##### 5.Запустить скрипт
```
./script.sh
```
=====  
  
## HW_2. Termial.  <a name="2"></a>
  
#### 1. Сделать папку dir_1  
```
mkdir_1
```
  
#### 2. Зайти в папку dir_1  
```
cd dir_1
```
  
#### 3. Создать папку inner_dir_1  
```
mkdir inner_dir_1
```

#### 4. Посмотреть где ты находишься  
```
pwd
```
*ответ терминала /c/Users/user/bash/dir_1*  
    
#### 5. Находясь в папке dir_1 создать пустой текстовый файл tf_1.txt  
```
touch tf_1.txt
```
  
#### 6. Находясь в папке dir_1 через команду cat создать текстовый файл tf_2.txt со следующими строками:  
- the first 1  
- the second 2  
- the third 3  
```
cat >> tf_2.txt
- the first 1
- the second 2
- the third 3
  
```
*выйти из режима редактирования Ctrl+C*  
  
#### 7. Зайти в папку inner_dir_1  
```
cd inner_dir_1
```
  
#### 8. Через cat сделать текстовый файл tf_3.txt  c любыми строками  
```
cat >> tf_3.txt
- one
- two
- three
- four
- five
- six
- seven
- eight
- nine
- ten

```
*выйти из режима редактирования Ctrl+C*  
  
#### 9. Через cat добавить в текстовый файл tf_3.txt строку “the second 2”  
```
cat >> tf_3.txt
the second 2

```
*выйти из режима редактирования Ctrl+C*  
  
#### 10. Через cat добавить в текстовый файл tf_3.txt строку “the sec 2”  
```
cat >> tf_3.txt
the sec 2

```
*выйти из режима редактирования Ctrl+C*  
  
#### 11. Через cat добавить в текстовый файл tf_2.txt строку “the sec 3”  
```
cat >> tf_3.txt
the sec 3

```
*выйти из режима редактирования Ctrl+C*  
  
#### 12. Через cat добавить в текстовый файл tf_3.txt строку “the SeCoNd 2”  
```
cat >> tf_3.txt
the SeCoNd 2

```
*выйти из режима редактирования Ctrl+C*  
  
#### 13. Через cat добавить в текстовый файл tf_2.txt строку “the seConD 2”  
```
cat >> tf_3.txt
the sEcOnD 2

```
*выйти из режима редактирования Ctrl+C*  
  
#### 14. Сделать текстовый файл tf_4.txt в котором будет 15 строк.  
```
cat >> tf_4.txt
111
222
333
444
555
666
777
888
999
101010
111111
121212
131313
141414
151515

```
*выйти из режима редактирования Ctrl+C*  
  
#### 15. Сделать текстовый файл tF_5.txt в котором будет 13 строк.  
```
cat >> tf_5.txt
111
222
333
444
555
666
777
888
999
101010
111111
121212
131313

```
*выйти из режима редактирования Ctrl+C*  
  
#### 16. Вывести список всех файлов в папке.  
```
ls -la
```
*ответ терминала:*  
```
total 3
drwxr-xr-x 1 user 197121   0 May 27 17:49 ./
drwxr-xr-x 1 user 197121   0 May 27 17:33 ../
-rw-r--r-- 1 user 197121 128 May 27 17:47 tf_3.txt
-rw-r--r-- 1 user 197121  78 May 27 17:48 tf_4.txt
-rw-r--r-- 1 user 197121 134 May 27 17:50 tf_5.txt
```
  
#### 17. Выйти из папки inner_dir_1  
```
cd ..
```
  
#### 18. Вывести содержимое файла tf_3.txt в терминал.  
```
cat /c/Users/user/bash/dir_1/inner_dir_1/tf_3.txt
```
*ответ терминала:*  
```
- one
- two
- three
- four
- five
- six
- seven
- eight
- nine
- ten
the second 2
the sec 2
the sec 3
the SeCoNd 2
the sEcOnD 2
```
  
#### 19. Найти путь к файлу tf_4.txt  
```
realpath tf_4.txt
```
*ответ терминала*  
```
/c/Users/user/bash/dir_1/tf_4.txt
```
  
#### 20. Отчистить файл tf_4.txt от содержимого без удаления самого файла.  
```
echo -n > /c/Users/user/bash/dir_1/inner_dir_1/tf_4.txt
```
  
#### 21. Найти путь к файлам у которых есть  “tf” в названии.  
```
find -name "*tf*"
```
*ответ терминала:*  
```
./inner_dir_1/tf_3.txt
./inner_dir_1/tf_4.txt
./inner_dir_1/tf_5.txt
./tf_1.txt
./tf_2.txt
```
  
#### 22. Найти путь к файлам у которых есть  “tf” в названии и буквы в любом регистре.  
```
find -iname "*tf*"
```
*ответ терминала:*  
```
./inner_dir_1/tf_3.txt
./inner_dir_1/tf_4.txt
./inner_dir_1/tf_5.txt
./tf_1.txt
./tf_2.txt
```
  
#### 23. Найти строки в файлах где есть комбинация букв “sec” в текущей папке  
```
find . 
```
  
#### 24. Найти строки в файлах где есть комбинация букв “sec” в любом регистре в текущей папке
#### 25. Найти строки в файлах где есть только комбинация букв “sec” в текущей папке
#### 26. Найти строки в файлах где есть только комбинация букв “sec” в любом регистре в текущей папке
#### 27. Найти строки в файлах где есть комбинация букв “second” в текущей папке
#### 28. Найти строки в файлах где есть комбинация букв “second” в любом регистре в текущей папке
#### 29. Найти строки в файлах где есть комбинация букв “second” во всех папках ниже уровнем
#### 30. Найти только путь и название файла в строках которых есть комбинация букв “second” в текущей папке
#### 31. Найти все строки во всех файлах где нет комбинации “second”
#### 32. Найти только название и путь к файлам где нет комбинации “second”
#### 33. Вывести в терминал 4 последних строк любого текстового файла
#### 34. Вывести в терминал 4 первые строки любого текстового файла.
#### 35. Команда в одну строку. Создать папку и создать текстовый файл с содержиммым.
#### 36. Команда в одну строку. Переместить в любую одну папку текстовые файлы у которых в содержимом есть слово “sec”
#### 37. Команда в одну строку. Скопировать в любую одну папку текстовые файлы у которых в содержимом есть слово “sec”
#### 38. Команда в одну строку. Найти все строки c “sec” во всех текстовых файлах, скопировать и вставить эти строки в один новый созданный текстовый файл.
#### 39. Команда в одну строку. Удалить текстовые файлы у которых в содержимом есть слово “sec”
#### 40. Просто вывести в терминал строку “Good job!!”
