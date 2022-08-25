[![MIT Licensed][icon-mit]][license]
[![Awesome][icon-awesome]][awesome]
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
[![Telegram][icon-chat]][chat]

# Git та GitHub

Ознайомтеся з Git і GitHub.

1.  Прослухайте тижні 1 і 2 курсу [Introduction to Git and GitHub](https://www.coursera.org/learn/introduction-git-github)

Для того, щоб проходити курс безкоштовно, треба натиснути кнопку "Enroll for free" і потім на лінк внизу "Audit course"

![git_intro_CC_audit](../img/coursera_audit.png)

Ви можете вдатися до автоматично перекладених субтитрів, зокрема, якщо ви відчуваєте що
це допоможе вам краще засвоїти відеокурс.

![git_intro-CC-guide](../img/git_intro.png)

2.  Пройдіть наступні рівні тут [learngitbranching.js.org](https://learngitbranching.js.org/):

    - Основи: Introduction Sequence, Ramping Up
    - Віддалені репозиторії: Push & Pull -- віддалені репозиторії в Git!

1.  Створіть репозиторій та назвіть його `kottans-frontend`.

1.  Створіть `README.md` для репозиторію.

1.  Опишіть свої враження від вивченого матеріалу.

1.  Надішліть pull-request сюди [Kottans/mock-repo][mock-repo] пропонуючи зміни.

    **Як зробити pull-request**

    - Форкніть цей репозиторій [Kottans/mock-repo][mock-repo]
    - Клонуйте свій форк локально на свій комп'ютер: `git clone https://github.com/YOUR_USERNAME/mock-repo.git`
    - Додайте цей репозиторій [Kottans/mock-repo][mock-repo] як upstream: `git remote add upstream https://github.com/kottans/mock-repo.git`
    - `git checkout master` і потім створіть нову гілку, ім'я на ваш роздум (aka feature branch): `git checkout -b BRANCH_NAME`.
    - Внесіть деякі зміни до свого локального сховища. Це може бути що завгодно, насправді. Якщо ви знайшли помилку в README - чудово!
      Подбайте про те, щоб дати своєму PR значуще (осмислене) ім’я та опис.
    - Внесіть зміни до новоствореної гілки (Сommit)
    - Перейдіть до гілки master: `git checkout master`
    - Витягніть останні зміни з гілки upstream master: `git pull upstream master`
    - Об’єднайте головну гілку зі своєю гілкою: `git checkout BRANCH_NAME && git merge master`
    - Вирішіть будь-які конфлікти мержу, якщо такі є (Resolve merge conflicts)
    - Надішліть гілку до вашого віддаленого сховища: `git push --set-upstream origin BRANCH_NAME`
    - Зробіть pull-request з вашого репозиторію до [цього][mock-repo] репозиторію через GitHub web-interface
    - Якщо вас попросять виправити merge конфлікт, зверніться до додаткових матеріалів для отримання відповідної інформації

    **Зауважте, що ваш PR можуть не розглянути швидко.**

    Чудова робота! Якщо ваш PR вже продивились ментори, узгодили та **вмерджили** (його статус змінено на `merged` з фіолетовою іконкою), то прийшов час ділитись своїми досягненнями з іншими –
    опублікуйте повідомлення в [course channel][chat]:
    `Git Basics — #done` (або `Git Basics — #p2p_done` якщо ви студент курсу p2p) і додайте посилання до свого репо. **Цей крок важливий, оскільки він допомагає наставникам відстежувати ваш прогрес!**

1.  Вивчіть додаткові матеріали нижче, щоб покращити свої навички.
    Якщо ви вважаєте, що це вплине на вашу загальну ефективність курсу, подумайте над тим, щоб
    повернутись до них пізніше, наприклад коли ви виконаєте всі обов’язкові завдання.

Коли ви закінчите це завдання, ви можете приступити до наступного.

## Додаткові матеріали

- [Лекція по Git від Олексія Руденка](https://www.youtube.com/playlist?list=PLS8sEUxbfFY9MnPIFPTNlaS5xX7P5Ge-5)

- [Git за 30 хвилин](https://codeguida.com/post/453)

- [Git tips](http://sixrevisions.com/web-development/git-tips/) — закріпити свої знання про Git

- [About Merge Conflicts](https://docs.github.com/en/free-pro-team@latest/github/collaborating-with-issues-and-pull-requests/about-merge-conflicts)

- [Resoilving a Merge Conflict](https://docs.github.com/en/free-pro-team@latest/github/collaborating-with-issues-and-pull-requests/resolving-a-merge-conflict-using-the-command-line)

- [Communicating using Markdown](https://lab.github.com/githubtraining/communicating-using-markdown)

- [Learn anything front-end](https://learn-anything.xyz/web-development/front-end)

- [TypingClub](https://www.typingclub.com/) — покращити швидкість набору на клавіатурі

- [How to Learn and Cope with Negative Thoughts](https://guides.hexlet.io/learning/)

## Готово?

➡️ Ідіть далі [Linux, Command Line, HTTP Tools](linux-cli-http.md)

⤴️ Повернутися до змісту курсу: [Contents](../contents.md)

[icon-chat]: https://img.shields.io/badge/chat-on%20telegram-blue.svg
[icon-mit]: https://img.shields.io/badge/license-MIT-blue.svg
[icon-awesome]: https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg
[license]: https://github.com/Kottans/web/blob/master/LICENSE.md
[awesome]: https://github.com/sindresorhus/awesome#front-end-development
[chat]: https://t.me/joinchat/CX8EF1JmLm9IM6J6oy2U7Q
[mock-repo]: https://github.com/Kottans/mock-repo
