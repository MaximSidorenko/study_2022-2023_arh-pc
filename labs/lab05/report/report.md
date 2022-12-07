**РОССИЙСКИЙ УНИВЕРСИТЕТ ДРУЖБЫ НАРОДОВ** 

**Факультет физико-математических и естественных наук Кафедра прикладной информатики и теории вероятностей** 

**ОТЧЕТ** 

**ПО ЛАБОРАТОРНОЙ РАБОТЕ** № **5** 

*дисциплина:  Архитектура Вычислительных Систем* 

Студент: Сидоренко Максим Алексеевич Группа:  НБИбд-02-22 

**МОСКВА** 2022  г. 

**Цель работы: Приобретение практических навыков работы в Midnight Commander. Освоение инструкций языка ассемблера mov и int.** 

**Ход работы:** 

- **5.3.** 

  Откроем midnight commander 

![](/home/masidorenko/work/study/2022-2023/Архитектура%20компьютера/arch-pc/labs/lab05/report/image/1.png)

![](/home/masidorenko/work/study/2022-2023/Архитектура%20компьютера/arch-pc/labs/lab05/report/image/2.jpeg)

- Пользуясь клавишами “вверх вниз и ENTER” перейдем в каталог ~/work/arch-pc 

![](/home/masidorenko/work/study/2022-2023/Архитектура%20компьютера/arch-pc/labs/lab05/report/image/3.jpeg)

- С помощью функциональной клавиши f7 создадим папку lab05 и перейдем в созданный каталог 

![](/home/masidorenko/work/study/2022-2023/Архитектура%20компьютера/arch-pc/labs/lab05/report/image/4.jpeg)

- Пользуясь строкой ввода и командой touch создадим файл lab5-1.asm 

![](/home/masidorenko/work/study/2022-2023/Архитектура%20компьютера/arch-pc/labs/lab05/report/image/5.jpeg)

- С помощью функциональной клавиши F4 откроем файл lab5- 1.asm для редактирования во встроенном редакторе. Как правило в качестве встроенного редактора Midnight Commander используется редактор nano  

![](/home/masidorenko/work/study/2022-2023/Архитектура%20компьютера/arch-pc/labs/lab05/report/image/6.jpeg)

![](/home/masidorenko/work/study/2022-2023/Архитектура%20компьютера/arch-pc/labs/lab05/report/image/7.jpeg)

- Введем текст программы из листинга 6.1, сохраним изменения и закроем файл  

![](/home/masidorenko/work/study/2022-2023/Архитектура%20компьютера/arch-pc/labs/lab05/report/image/8.jpeg)

![](/home/masidorenko/work/study/2022-2023/Архитектура%20компьютера/arch-pc/labs/lab05/report/image/7.jpeg)

- С помощью функциональной клавиши F3 откроем файл lab5- 1.asm для просмотра, убедимся, что файл содержит текст 

программы ![](/home/masidorenko/work/study/2022-2023/Архитектура%20компьютера/arch-pc/labs/lab05/report/image/9.jpeg)

- Оттранслируем текст программы lab5-1.asm в объектный файл. Выполнили компоновку объектного файла и запустили получившийся исполняемый файл. Программа выводит стороку ‘Введите строку’ и ожидает ввода с клавиатуру, На запрос введем ФИО

![](/home/masidorenko/work/study/2022-2023/Архитектура%20компьютера/arch-pc/labs/lab05/report/image/10.png)

![](/home/masidorenko/work/study/2022-2023/Архитектура%20компьютера/arch-pc/labs/lab05/report/image/11.png)

![](/home/masidorenko/work/study/2022-2023/Архитектура%20компьютера/arch-pc/labs/lab05/report/image/12.png)

![](/home/masidorenko/work/study/2022-2023/Архитектура%20компьютера/arch-pc/labs/lab05/report/image/13.jpeg)

- **5.3.1. Подключение внешнего файла in\_out.asm** 
- Скачаем файл in\_out.asm со страницы курса ТУИС 

![](/home/masidorenko/work/study/2022-2023/Архитектура%20компьютера/arch-pc/labs/lab05/report/image/14.jpeg)

- Подключаемый файл in\_out.asm должен лежать в том же каталоге, что и файл с программой, в которой он используется. В одной из панелей mc откроем каталог с файлом lab5-1.asm. В другой панели каталог с in\_out.asm. Скопируем файл in\_out.asm в каталог с файлом lab5-1.asm  

![](/home/masidorenko/work/study/2022-2023/Архитектура%20компьютера/arch-pc/labs/lab05/report/image/15.jpeg)

- С помощью функциональной клавиши F6 создадим копию файла lab5-1.asm с именем lab5-2.asm. Выделим файл lab5- 1.asm, нажмем на клавишу F6, введем имя файла lab5-2.asm и нажмем на ENTER 

![](/home/masidorenko/work/study/2022-2023/Архитектура%20компьютера/arch-pc/labs/lab05/report/image/16.jpeg)

![](/home/masidorenko/work/study/2022-2023/Архитектура%20компьютера/arch-pc/labs/lab05/report/image/17.jpeg)

- Исправим  текст  программы  в  файле  lab5-2.asm  с использованием  подпрограммы  из  внешнего  файла in\_out.asm(используем подпрограммы sprintLF, sread и quit) в соответствии  с  листингом  6.2. Создим  исполняемый  файл и проверим  его  работу ![](/home/masidorenko/work/study/2022-2023/Архитектура%20компьютера/arch-pc/labs/lab05/report/image/18.jpeg)![](/home/masidorenko/work/study/2022-2023/Архитектура%20компьютера/arch-pc/labs/lab05/report/image/19.jpeg)

![](/home/masidorenko/work/study/2022-2023/Архитектура%20компьютера/arch-pc/labs/lab05/report/image/20.png)

![](/home/masidorenko/work/study/2022-2023/Архитектура%20компьютера/arch-pc/labs/lab05/report/image/21.png)

![](/home/masidorenko/work/study/2022-2023/Архитектура%20компьютера/arch-pc/labs/lab05/report/image/22.jpeg)

![](/home/masidorenko/work/study/2022-2023/Архитектура%20компьютера/arch-pc/labs/lab05/report/image/23.jpeg)

- В файле lab5-2.asm заменим подпрограмму sprintLF на sprint. Создадим исполняемый файл и проверим его работу.  

Между ними видна разница в том, что sprintLF строку для ввода переносит вниз, а sprint на той же строке, где и указание ‘Введите строку’

![](/home/masidorenko/work/study/2022-2023/Архитектура%20компьютера/arch-pc/labs/lab05/report/image/24.jpeg)

![](/home/masidorenko/work/study/2022-2023/Архитектура%20компьютера/arch-pc/labs/lab05/report/image/25.jpeg)

- 5.4. Самостоятельная работа
- Создайте  копию  файла  lab6-1.asm.  Внесите  изменения  в программу  (без  использования  внешнего  файла  in\_out.asm), так чтобы она работала по следующему алгоритму: 
- вывести приглашение типа “Введите строку:”;
- ввести строку с клавиатуры; 
- вывести  введённую  строку  на  экран.

![](/home/masidorenko/work/study/2022-2023/Архитектура%20компьютера/arch-pc/labs/lab05/report/image/26.jpeg)

![](/home/masidorenko/work/study/2022-2023/Архитектура%20компьютера/arch-pc/labs/lab05/report/image/27.jpeg)

- Получим  исполняемый  файл  и  проверим  его  работу.  На приглашение введем строку своё имя и фамилию 

![](/home/masidorenko/work/study/2022-2023/Архитектура%20компьютера/arch-pc/labs/lab05/report/image/28.jpeg)

![](/home/masidorenko/work/study/2022-2023/Архитектура%20компьютера/arch-pc/labs/lab05/report/image/29.jpeg)

![](/home/masidorenko/work/study/2022-2023/Архитектура%20компьютера/arch-pc/labs/lab05/report/image/30.jpeg)

- Создим копию файла lab6-2.asm. Исправим текст программы с использованием подпрограмм из внешнего файла in\_out.asm, так чтобы она работала по следующему алгоритму: 
- вывести приглашение типа “Введите строку:”; 
- ввести строку с клавиатуры; 
- вывести введённую строку на экран. 

![](/home/masidorenko/work/study/2022-2023/Архитектура%20компьютера/arch-pc/labs/lab05/report/image/31.jpeg)

![](/home/masidorenko/work/study/2022-2023/Архитектура%20компьютера/arch-pc/labs/lab05/report/image/32.jpeg)

- Создадим  исполняемый  файл  и  проверим  его  работу

![](/home/masidorenko/work/study/2022-2023/Архитектура%20компьютера/arch-pc/labs/lab05/report/image/33.jpeg)

![](/home/masidorenko/work/study/2022-2023/Архитектура%20компьютера/arch-pc/labs/lab05/report/image/34.jpeg)

![](/home/masidorenko/work/study/2022-2023/Архитектура%20компьютера/arch-pc/labs/lab05/report/image/35.png)

- **Вывод:  после  проделанной  работы,  я приобрел  практические  навыки  работы  в Midnight  commander.  Освоил  инструкции языка ассемблера mov и int** 

**Cсылка на гитхаб  [https://github.com/MaximSidorenko/study_2022- 2023_arh-pc** ](https://github.com/MaximSidorenko/study_2022-2023_arh-pc)**
