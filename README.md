#Лифт в здании
Необходимо написать приложение без UI(консольное), или с минимальным UI.
- Использовать ООП и придерживаться принципов SOLID, DRY и ETC.
- Здание состоит из n-ое количества этажей, где n - случайное число генерируемое
при старте программы в диапазоне 5 <= n <= 20.
- На каждом этаже k количество пассажиров, где k - случайное число генерируемое
при старте программы в диапазоне 0 <= k <= 10.
- Каждый пассажир хочет приехать на определённый этаж отличный от того на
котором он находиться.
- На каждом этаже есть две кнопки для вызова лифта "Вверх" и "Вниз". исключение
составляют нижний и верхний этаж.
- Лифт имеет ограничение по вместимости: максимум 5 человек.
Первый раз лифт загружается людьми с первого этажа, и едет от
первого(текущего) до наибольшего из тех на которые нужно пассажирам.
По дороге лифт останавливается на тех этажах на которых нужно пассажирам
высаживая их и подбирая людей которым нужно в том же направлении в котором
движется лифт.
- Также если лифт загружен не полностью он может остановиться на этаже на
котором есть люди, которым необходимо в том же направлении.
При посадки новых пассажиров максимальный этаж пересчитывается.


Неоднозначные моменты:
-
- Если на этаже вышли все, но больше на этом этаже пассажиров нет, лифт едет дальше по направлению пока не достигнет последнего этажа где потом поменяет направление
- Установленно ограничение на количество итераций(100) во избежания бесконечного цикла