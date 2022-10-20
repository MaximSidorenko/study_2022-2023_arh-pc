**РОССИЙСКИЙ УНИВЕРСИТЕТ ДРУЖБЫ НАРОДОВ** 

**Факультет физико-математических и естественных наук Кафедра прикладной информатики и теории вероятностей** 

**ОТЧЕТ**  

**ПО ЛАБОРАТОРНОЙ РАБОТЕ № 2** 

*дисциплина: Архитектура Вычислительных Систем* 

Студент: Сидоренко Максим Алексеевич         Группа:    НБИбд-02-22         

**МОСКВА** 2022  г. 

**Цель работы:** Целью работы является изучить идеологию и применение средств контроля версий. Приобрести практические навыки по работе с системой git. 

**Лабораторная работа** 

**Ход работы:**  

1) **Настройка github 2.4.1.** 
- Существует несколько доступных серверов репозиториев с возможностью бесплатного размещения данных. Например, http://bitbucket.org/, https://gith ub.com/ и https://gitflic.ru. Для выполнения лабораторных работ предлагается использовать Github. Создадим учётную запись на сайте https://github.com/ и заполним основные данные.

![](/home/masidorenko/work/study/2022-2023/Архитектура%20компьютера/arch-pc/labs/lab02/report/image/1.png)

![](/home/masidorenko/work/study/2022-2023/Архитектура%20компьютера/arch-pc/labs/lab02/report/image/2.jpeg)

![](/home/masidorenko/work/study/2022-2023/Архитектура%20компьютера/arch-pc/labs/lab02/report/image/3.png)

2) **Базовая настройка git 2.4.2** 
- Сначала сделаем предварительную конфигурацию git. Откроем терминал и введём следующие команды, указав имя и email владельца репозитория:

![](/home/masidorenko/work/study/2022-2023/Архитектура%20компьютера/arch-pc/labs/lab02/report/image/4.png)

- Настроим utf-8 в выводе сообщений git:

![](/home/masidorenko/work/study/2022-2023/Архитектура%20компьютера/arch-pc/labs/lab02/report/image/5.png)

- Зададим имя начальной ветки (будем называть её master):![](/home/masidorenko/work/study/2022-2023/Архитектура%20компьютера/arch-pc/labs/lab02/report/image/6.png)
- Параметр autocrlf:![](/home/masidorenko/work/study/2022-2023/Архитектура%20компьютера/arch-pc/labs/lab02/report/image/7.png)
- Параметр safecrlf:

![](/home/masidorenko/work/study/2022-2023/Архитектура%20компьютера/arch-pc/labs/lab02/report/image/8.png)

3) **Создание SSH ключа 2.4.3** 
- Для последующей идентификации пользователя на сервере репозиториев необходимо сгенерировать пару ключей (приватный и открытый): 

![](/home/masidorenko/work/study/2022-2023/Архитектура%20компьютера/arch-pc/labs/lab02/report/image/9.jpeg)

- Ключи сохраняться в каталоге ~/.ssh/. Далее необходимо загрузить сгенерённый открытый ключ. Для этого зайдём на сайт http://github.org/ под своей учётной записью и перейти в меню Setting . После этого выберем в боковом меню SSH and GPG keys и нажмем кнопку New SSH key . Скопировав из локальной консоли ключ в буфер обмена

![](/home/masidorenko/work/study/2022-2023/Архитектура%20компьютера/arch-pc/labs/lab02/report/image/10.jpeg)

![](/home/masidorenko/work/study/2022-2023/Архитектура%20компьютера/arch-pc/labs/lab02/report/image/11.png)

- вставляем ключ в появившееся на сайте поле и указываем для ключа имя (Title).

![](/home/masidorenko/work/study/2022-2023/Архитектура%20компьютера/arch-pc/labs/lab02/report/image/12.jpeg)

4) **Сознание рабочего пространства и репозитория курса на основе шаблона** 
- При выполнении лабораторных работ следует придерживаться структуры рабочего пространства. Рабочее пространство по предмету располагается в следующей иерархии:

![](/home/masidorenko/work/study/2022-2023/Архитектура%20компьютера/arch-pc/labs/lab02/report/image/13.png)

- Каталог для лабораторных работ имеет вид labs 
- Каталоги для лабораторных работ имеют вид lab<номер>, например: lab01, lab02 и т.д. 
- Название проекта на хостинге git имеет вид: study\_<учебный год>\_<код предмета> Например, для 2022–2023 учебного года и предмета «Архитектура компьютера» (код предмета arch-pc) название проекта примет следующий вид: study\_2022–2023\_arch-pc  
- Откроем терминал и создадим каталог для предмета «Архитектура компьютера»: 

![](/home/masidorenko/work/study/2022-2023/Архитектура%20компьютера/arch-pc/labs/lab02/report/image/14.png)

5) **Сознание репозитория курса на основе шаблона 2.4.5** 
- Репозиторий на основе шаблона можно создать через web- интерфейс github. Перейдём на станицу репозитория с шаблоном курса https://github.com/yam adharma/course-directory-student- template. Далее выберем Use this template.

![](/home/masidorenko/work/study/2022-2023/Архитектура%20компьютера/arch-pc/labs/lab02/report/image/15.jpeg)

- В открывшемся окне зададим имя репозитория (Repository name) study\_2022–2023\_arh-pc и создадим репозиторий (кнопка Create repository from template).

![](/home/masidorenko/work/study/2022-2023/Архитектура%20компьютера/arch-pc/labs/lab02/report/image/16.jpeg)

![](/home/masidorenko/work/study/2022-2023/Архитектура%20компьютера/arch-pc/labs/lab02/report/image/17.jpeg)

- Откройте терминал и перейдите в каталог курса:

![](/home/masidorenko/work/study/2022-2023/Архитектура%20компьютера/arch-pc/labs/lab02/report/image/18.png)

- Клонируем созданный репозиторий:

![](/home/masidorenko/work/study/2022-2023/Архитектура%20компьютера/arch-pc/labs/lab02/report/image/19.png)

- Ссылку для клонирования можно скопировать на странице созданного репозитория Code -> SSH:

![](/home/masidorenko/work/study/2022-2023/Архитектура%20компьютера/arch-pc/labs/lab02/report/image/20.png)

6) **Настройка каталога курса 2.4.6** 
- Перейдем в каталог курса:

![](/home/masidorenko/work/study/2022-2023/Архитектура%20компьютера/arch-pc/labs/lab02/report/image/21.png)

- Удалим лишние файлы:

![](/home/masidorenko/work/study/2022-2023/Архитектура%20компьютера/arch-pc/labs/lab02/report/image/22.png)

- Создадим необходимые каталоги:

![](/home/masidorenko/work/study/2022-2023/Архитектура%20компьютера/arch-pc/labs/lab02/report/image/23.png)

- Отправим файлы на сервер: 

![](/home/masidorenko/work/study/2022-2023/Архитектура%20компьютера/arch-pc/labs/lab02/report/image/24.jpeg)

![](/home/masidorenko/work/study/2022-2023/Архитектура%20компьютера/arch-pc/labs/lab02/report/image/25.png)

![](/home/masidorenko/work/study/2022-2023/Архитектура%20компьютера/arch-pc/labs/lab02/report/image/26.jpeg)

7) **Самостоятельная работа 2.5** 

**Ход работы:**

1. **Cоздадим отчет по выполнению лабораторной работы в соответствующем каталоге рабочего пространства (labs>lab02>report).**

![](/home/masidorenko/work/study/2022-2023/Архитектура%20компьютера/arch-pc/labs/lab02/report/image/27.jpeg)

2. **Скопируем отчеты по выполнению предыдущих лабораторных работ в соответствующие каталоги созданного рабочего пространства.**

![](/home/masidorenko/work/study/2022-2023/Архитектура%20компьютера/arch-pc/labs/lab02/report/image/28.png)

3. **Загрузим файлы на guthib**

![](/home/masidorenko/work/study/2022-2023/Архитектура%20компьютера/arch-pc/labs/lab02/report/image/29.jpeg)

![](/home/masidorenko/work/study/2022-2023/Архитектура%20компьютера/arch-pc/labs/lab02/report/image/30.jpeg)

![](/home/masidorenko/work/study/2022-2023/Архитектура%20компьютера/arch-pc/labs/lab02/report/image/31.jpeg)

![](/home/masidorenko/work/study/2022-2023/Архитектура%20компьютера/arch-pc/labs/lab02/report/image/32.jpeg)

**Вывод:** Мы изучили идеолгию и применение средств контроля версий. Приобрели практические навыки по работе с системой git 

**(ссылка на github)  (https://github.com/MaximSidorenko/study\_2022-2023\_arh-pc)** 
