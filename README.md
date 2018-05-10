# Первые шаги по освоению HTML

## Инструкция по запуску проекта

1. Скачиваем и устанавливаем Vagrant и VirtualBox
1. Клонируем репозиторий в удобную нам папку с помощью команды:

        git clone git@github.com:test-qeep/html-first-steps.git
    
1. Переходим в папку **html-first-steps**: `cd html-first-steps`
1. Запускаем виртуальную машину: `vagrant up`
1. Заходим в командную строку виртуальной машины по SSH-протоколу: `vagrant ssh`

## Инструкция по базовой работе с Git

1. `git add` — добавляет файл в индекс
1. `git commit` — создает коммит из всех файлов в индексе
1. `git commit -m "Comment"` — позволяет добавить комментарий к коммиту в командной строке
1. `git push` — залить (запушить) изменения в удаленный репозиторий
1. `git pull` — принять (запуллить) изменения с удаленного репозитория
1. `git clone git@github.com:user/repo-name.git` — склонировать удаленный репозиторий

## Работа с HTML

### Подключение скриптов и стилей

* Скрипты можно подключить с помощью тега `<script>`:
    
        <script type="text/javascript">
            // Объявляем переменную j и присваиваем ей значение 10
            var j = 10;
            console.log(j);
        </script>
        
* Стили создаются с помощью тега `<style>`:

        <style>
            h1, h2, h3, h4, h5, h6 {
                background: red;
            }
            .class {
                color: #ba0;
            }
        </style>
        
### Подключение файлов

* Чтобы подключить файл со скриптом,
необходимо прописать тег `<script>` с атрибутом `src`:

        <script src="/index.js" type="text/javascript"></script> 
         
* Для подключения файла со стилями прописываем
тег `<link>` с аттрибутом `rel="stylesheet"`:

        <link rel="stylesheet" href="index.css">