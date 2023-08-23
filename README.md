

Общее:
Программный пакет ReadWeldMonitoring включает в себя 3 составных микро сервиса: 
1.	web-интерфейс;
2.	приемник данных;
3.	генератор excel отчетов
При разработчике системы использовался модульный подход к проектированию. Такой подход позволяет корректно работать всей системе в целом в случаи неисправности одной из ее частей. Так же система ReadWeld проинформирует вас о неисправностях или иных сбоях.


Используемый стек технологий:
1.	Python 3.6.8 – основной язык программирования, используемых во всех микро сервисах.
2.	Falsk – web-фраемворк, использовался при разработки web-интерфеса и приемника данных
3.	Docker – для развертывания приложения на удаленном сервере


Приемник данных является независимой системы обработки данных с датчиков ReadWeld. Грамотно построенная архитектура микро сервиса позволяет в непрерывном режиме обслуживать до 40 устройств одновременно. Кроме приема значений с датчика, система также корректирует встроенные параметры устройства, такая возможность обратной связи позволяет получать наиболее точные и достоверные данные своевременно. 