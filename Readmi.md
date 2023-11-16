
```mermaid
graph TD;
  Хочешь_перенести_на_GitHub -- "Скопируй SSH?" --> ready;
  ready -- "Создаем директорию локально $ mkdir lesson"     --> ready_dir;
  ready_dir -- "Переходим в нее $ cd lesson" --> ready_changedir;

  ready_changedir  -- "Инициализируем гит $ git init" --> ready_gitinit;
  ready_gitinit -- "Создаем нужные нам файлы$ touch README.md"--> ready_createfile;
  ready_createfile -- "Добавляем все наши файлы $ git add . или выбранный $ git add README.md" --> readyadd;
  readyadd -- "Перый коммит с комментом git commit -m 'Добавить README'"  --> readycommit;
  readycommit -- "Добавляем все наши файлв в удаленный репозиторий git remote add origin ///далее ссылка SSH вашего репозитория на ГитХаб " --> readygitremote;
  readygitremote -- "Пушим $ git push -u origin main " -->readypush;

