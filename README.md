# FAQ
```student_list``` - список всех студентов

``` all_grades ``` - функция возвращения всех оценок

``` average ``` - функция подсчета среднего арифметического числа

``` lecturer_grades ``` - функция добавления лекторам оценок

``` lecturer_list ``` - список всех лекторов

``` __lt__ ``` - функция сравнения лекторов и студентов по средней оценки за лекции

``` show_grades ``` - просмотр всех оценок у лекторов

``` rate_hw ``` - функция добавления студентам оценок

``` courses_average_students ``` - подсчет средней оценки за домашние задания по всем студентам в рамках конкретного курса

``` courses_average_lecturer ``` - подсчет средней оценки за лекции всех лекторов в рамках конкретного курса



## Задание № 1. Наследование
*класс **Mentor** должен стать родительским классом, а от него нужно реализовать наследование классов **Lecturer** (лекторы) и **Reviewer** (эксперты, проверяющие домашние задания). Очевидно, имя, фамилия и список закрепленных курсов логично реализовать на уровне родительского класса. А чем же будут специфичны дочерние классы? Об этом в следующих заданиях.*
## Задание № 2. Атрибуты и взаимодействие классов.
*В квизе к предыдущей лекции мы реализовали возможность выставлять студентам оценки за домашние задания. Теперь это могут делать только Reviewers (реализуйте такой метод)! А что могут делать лекторы? Получать оценки за лекции от студентов :) Реализуйте метод выставления оценок лекторам у класса Student (оценки по 10-балльной шкале, хранятся в атрибуте-списке). Лектор при этом должен быть закреплен за тем курсом, на который записан студент*
## Задание № 3. Полиморфизм и магические методы
>*Перегрузите магический метод ```__str__``` у всех классов*
> 
*Reviewer: ```экземпляр_класса.__str__()```*

*Lecturer: ```экземпляр_класса.__str__()```*

*Student: ```экземпляр_класса.__str__()```*

#### Реализуйте возможность сравнивать (через операторы сравнения) между собой лекторов по средней оценке за лекции и студентов по средней оценке за домашние задания.

*Lecturer: ```print(экземпляр_класса > экземпляр_класса)```*

*Student: ```print(экземпляр_класса < экземпляр_класса)```*

## Задание № 4. Полевые испытания

>для подсчета средней оценки за домашние задания по всем студентам в рамках конкретного курса (в качестве аргументов принимаем список студентов и название курса);

*Student: ```courses_average_students(Student.student_list, 'Курс')```*

>для подсчета средней оценки за лекции всех лекторов в рамках конкретного курса (в качестве аргументов принимаем список лекторов и название курса).

*Lecturer: ```courses_average_lecturer(Lecturer.lecturer_list, 'Курс')```*


