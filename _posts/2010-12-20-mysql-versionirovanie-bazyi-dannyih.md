---
layout: post
title: MySQL – версионирование базы данных

tags: [mysql, svn, sym, symlink, versioning]
---

Часто при создании больших сайтов, необходимо использовать системы версионирования, для того чтобы несколько человек могли совместно работать над созданием сайта.

С иходными кодами проекта все ясно, тут есть и SVN и GIT и им подобные системы, а вот как быть с базой данных?

Задача состоит в том чтобы перенести файлы базы в папку с проектом создаваемого сайта. Слава богу разработчкики MySQL позаботились о нас и ввели такое понятие как ссылки на базы.

Итак, что необходимо сделать:

1. Создать файл `my_data_base.sym` в папке `mysql/data`.
2. Прописать в этом файле полный путь к папке с базой, например вот так: `D:\xampp\htdocs\my_project\my_data_base`.

Теперь можно загонять базу в SVN.
