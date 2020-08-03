# jv-salary-info

Реализуйте метод `getSalaryInfo(String[] names, String[] data, String dateFrom, String dateTo)` вычисляющий зарплату сотрудников. На вход методу подаётся 2 массива и 2 даты, определяющие период за который надо вычислить зарплату, первый массив содержит имена сотрудников организации, второй массив информацию о рабочих часах и ставке. Формат данных второго массива следующий: дата, имя сотрудника, количество отработанных часов, ставка за 1 час. Создать пакет exception и в нём класс-ошибку IllegalDateParametersException, она должен быть unchecked. Сделать так, чтобы метод getSalaryInfo выбрасывал IllegalDateParametersException, если dateFrom > dateTo, с сообщнием "Wrong parameters". Метод должен вернуть отчёт за период, который передали в метод (обе даты включительно) составленный по следующей форме: 
   Отчёт за период #дата_1# - #дата_2#
   Имя сотрудника - сумма заработанных средств за этот период

   Пример ввода:
   date from = `01.04.2019 `
   date to = `30.04.2019` 

   names:

   ```Java
   Сергей
   Андрей
   София
   ```

   data:

   ```java
  26.04.2019 Сергей 4 50
  05.04.2019 Андрей 3 200
  10.04.2019 Сергей 7 100
  22.04.2019 София 9 100
  25.06.2019 Сергей 11 50
  26.04.2019 Андрей 3 150
  13.02.2019 Сергей 7 100
  26.04.2019 София 9 100
   ```

   Пример вывода:

   ```java
   Отчёт за период 01.04.2019  - 30.04.2019  
   Сергей - 900
   Андрей - 1050
   София - 1800
   ```
