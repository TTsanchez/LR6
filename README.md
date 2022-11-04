# LR6
Лабораторная работа №6

Первым шагом мы создаем копию репозитория в личное хранилище репозиторий: https://github.com/Kurtyanik/LR6/

![1](https://github.com/TTsanchez/LR6/blob/master/imgs/1.jpg)

Далее используем команды git config --global user.name и git config --global user.email для настройки клиента Git и вводим свои данные от GitHub.

![2](https://github.com/TTsanchez/LR6/blob/master/imgs/2.jpg)

Клонируем удаленный репозиторий, используя команду git clone.

![3](https://github.com/TTsanchez/LR6/blob/master/imgs/3.jpg)

Добавим файл через интерфейс GitHub. Далее переходим в директорию LR6 командой cd LR6 для дальнейшей работы с файлами.

![4](https://github.com/TTsanchez/LR6/blob/master/imgs/4.jpg)

Подтянем изменения из веб-интерфейса GitHub для клиента Git. Для этого используем команду git pull.
 
![5](https://github.com/TTsanchez/LR6/blob/master/imgs/5.jpg)

Посмотрим коммиты ветки master, используя команду git log.
  
 ![6](https://github.com/TTsanchez/LR6/blob/master/imgs/6.jpg)
  
Просмотрим существующие ветки в текщем репозитории командой git branch.
  
![7](https://github.com/TTsanchez/LR6/blob/master/imgs/7.jpg)
  
Перейдем в ветку branch1 командой git checkout branch1.

![8](https://github.com/TTsanchez/LR6/blob/master/imgs/8.jpg)

Посмотрим коммиты ветки branch1 с помощью команды git log.

![9](https://github.com/TTsanchez/LR6/blob/master/imgs/9.jpg)

Используем команду git log -p, чтобы рассмотреть коммиты.

![10](https://github.com/TTsanchez/LR6/blob/master/imgs/10.jpg)
![11](https://github.com/TTsanchez/LR6/blob/master/imgs/11.jpg)

Вернемся в ветку master.

![12](https://github.com/TTsanchez/LR6/blob/master/imgs/12.jpg)

Выполним слияние в ветку master. Слияние производится при помощи команды git merge branch1.

![13](https://github.com/TTsanchez/LR6/blob/master/imgs/13.jpg)

Произошел конфликт. Скорее всего из-за того, что файл mergefile.txt не отслеживается. Используем команду git status.

![14](https://github.com/TTsanchez/LR6/blob/master/imgs/14.jpg)

Теория оказалась верна. Добавим файл для отслеживания командой git add mergefile.txt.

![15](https://github.com/TTsanchez/LR6/blob/master/imgs/15.jpg)

Проверим еще раз, отслеживается ли файл.

![16](https://github.com/TTsanchez/LR6/blob/master/imgs/16.jpg)

Конфликт разрешен, оставляем коммит при помощи команды git commit -m "Branches".

![17](https://github.com/TTsanchez/LR6/blob/master/imgs/17.jpg)

Удаляем побочную ветку после успешного слияния при помощи команды git branch -d branch1

![18](https://github.com/TTsanchez/LR6/blob/master/imgs/18.jpg)

Создадим изменения и комментарии для них. Создавать будем текстовые файлы прямо в терминале. Для создания текстовика используем команду echo hello > change1.txt, зафиксируем его git add change1.txt. Оставим комментарий git commit -m "Change1.txt". Повторем все то же самое еще раз, только название указываем другое - change2.txt.

![19](https://github.com/TTsanchez/LR6/blob/master/imgs/19.jpg)

Посмотрим комментарии.

![20](https://github.com/TTsanchez/LR6/blob/master/imgs/20.jpg)

Теперь сделаем "хард" откат коммита. Вводим команду git reset --hard HEAD~1

![21](https://github.com/TTsanchez/LR6/blob/master/imgs/21.jpg)

Создадим ветку для отчета и перейдем в неё git branch report.

![22](https://github.com/TTsanchez/LR6/blob/master/imgs/22.jpg)

Получим итоговую историю операций

![23](https://github.com/TTsanchez/LR6/blob/master/imgs/23.jpg)

После редактирования отчета, его нужно будет сохранить и произвести команды git add и git commit. В конце работы необходимо будет отправить все локальные изменения в сетевое хранилище GitHub командой git push.


