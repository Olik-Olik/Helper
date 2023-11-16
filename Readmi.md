HEAD -- это голова.
Коммит -- это всему голова.
Статусы файлов:
<тут пустая строка!>

```mermaid
graph TD;
flowchart TD
A"Хочешь перенести свой проект на  GitHub?" --› B"Сделал новый проект на GitHub";
B -- Yes --› C"Скопируй SSH";
B -- No --› D "Do it!";
C ---- Yes --› F"Создаем директорию локально $ mkdir lesson";
F ------› E"Переходим в нее $ cd lesson";
E --------› G"Инициализируем гит $ git init";
G ----------› H"Создаем нужные нам файлы$ touch README.md";
H ------------› J"Добавляем все наши файлы $ git add . или выбранный $ git add README.md";
J --------------› K"Перый коммит с комментом git commit -m 'Добавить README'";
K ----------------› L"Добавляем все наши файлв в удаленный репозиторий git remote add origin ///далее ссылка SSH вашего репозитория на ГитХаб ";
L ------------------› M"Пушим $ git push -u origin main ";


```
```mermaid
graph LR;
  untracked -- "git add" --> staged;
  staged    -- "???"     --> tracked/comitted;

%% стрелка без текста для примера: 
  A --> B;
``` 
