# homeworkForLesson5
### Сборщики мусора ###
##### Домашнее задание ###

* Определение нужного размера хипа. 
* Запустите его с размером хипа 256 Мб и посмотрите в логе время выполнения. 
* Нужно проанализировать производительность в зависимости от объема памяти и также попробовать оптимизировать код.
* Также необходимо оптимизировать код, не меняя логику и определить самый эффективный хип для него.

---

***Integer:***

* 256:  spend msec:17151, sec:17  spend msec:17139, sec:17  spend msec:16960, sec:16  spend msec:17381, sec:17  spend msec:17726, sec:17
* 512:  spend msec:12028, sec:12  spend msec:12083, sec:12  spend msec:12187, sec:12  spend msec:12082, sec:12  spend msec:12199, sec:12
* 1024: spend msec:10868, sec:10  spend msec:10924, sec:10  spend msec:10872, sec:10  spend msec:10807, sec:10  spend msec:10682, sec:10
* 2048: spend msec:9964, sec:9    spend msec:9857, sec:9    spend msec:9983, sec:9    spend msec:9988, sec:9    spend msec:10025, sec:10
* 4096: spend msec:10445, sec:10  spend msec:10328, sec:10  spend msec:10314, sec:10  spend msec:10275, sec:10  spend msec:10381, sec:10
* 10192:spend msec:21080, sec:21  spend msec:18862, sec:18  spend msec:16586, sec:16  spend msec:19965, sec:19  spend msec:15329, sec:15

***Integer заменен на int:***

* 256:   spend msec:3142, sec:3  spend msec:2852, sec:2  spend msec:2499, sec:2  spend msec:2435, sec:2  spend msec:2477, sec:2
* 512:   spend msec:2242, sec:2  spend msec:1891, sec:1  spend msec:1905, sec:1  spend msec:1842, sec:1  spend msec:1965, sec:1
* 1024:  spend msec:1811, sec:1  spend msec:1793, sec:1  spend msec:1800, sec:1  spend msec:1784, sec:1  spend msec:1754, sec:1
* 2048:  spend msec:1881, sec:1  spend msec:1996, sec:1  spend msec:1869, sec:1  spend msec:1842, sec:1  spend msec:1869, sec:1
* 4096:  spend msec:1807, sec:1  spend msec:1841, sec:1  spend msec:1868, sec:1  spend msec:1895, sec:1  spend msec:1899, sec:1
* 10192: spend msec:1951, sec:1  spend msec:2118, sec:2  spend msec:1905, sec:1  spend msec:1864, sec:1  spend msec:1830, sec:1


***Вывод:***

При Integer дольше всего работает на 256. Оптимальная работа - на 2048.

Integer меняем на int. Дольше всего работает на 256. Оптимальная работа - на 1024.   
