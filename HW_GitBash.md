## HW_1. The first part 
## Linux terminal (GitBash) commands

1. Посмотреть где я 
`pwd`

2. Создать папку
`mkdir folder_1`

3. Зайти в папку
`cd folder_1`

4. Создать 3 папки 
`mkdir folder_2 folder_3 folder_4`

5. Зайти в любоую папку
`cd folder_2`

6. Создать 5 файлов (3 txt, 2 json)
`touch aa.txt ab.txt ac.txt ad.json ae.json`

7. Создать 3 папки
`mkdir folder5 folder6 folder7`

8. Вывести список содержимого папки
`ls -la` 

9. Открыть любой txt файл
`cat ab.txt`

10. Написать туда что-нибудь, любой текст
`vim ab.txt i hello world`

11. Сохранить и выйти
`esc :wq`

12. Выйти из папки на уровень выше
`cd ..`

13. Переместить любые 2 файла, которые вы создали, в любую другую папку
`mv aa.txt ab.txt folder5`

14. Скопировать любые 2 файла, которые вы создали, в любую другую папку 
`cp aa.txt ab.txt folder6`

15. Найти файл по имени
`find . -name "aa.txt"`

16. Просмотреть содержимое в реальном времени (команда grep) изучите как она работает
`tail -f ab.txt | grep a`

17. Вывести несколько первых строк из текстового файла
`head -n 2 ab.txt`

18. Вывести несколько последних строк из текстового файла
`tail -n 2 ab.txt`

19. Просмотреть содержимое длинного файла (команда less) изучите как она работает
`less ab.txt, q`

20. Вывести дату и время
`date "+%D %T"`

Задание *
1. Отправить http запрос на сервер

`curl http://162.55.220.72:5005/terminal-hw-request`

`curl 'http://162.55.220.72:5005/get_method?name=Sergey&age=26'`

2. Написать скрипт который выполнит автоматически пункты 3, 4, 5, 6, 7, 8, 13

        vim mysript_1.sh

        #!/bin/bash
        cd hw_2
        mkdir fl_2 fl_3 fl_4
        cd fl_2
        touch an.txt am.txt av.txt ac.json ax.json
        mkdir fl_5 fl_6 fl_7
        ls -la
        mv av.txt ac.json fl_6

        chmod +x mysript_1.sh