# Dark world
Платформа: Windows

Язык: Русский

Технологии: C#, Monogame.

Сеттинг: Тёмный мир.

Длительность: На пару вечеров ~30-60 минут
## Сюжет
учёный участвовавший в эксперименте случайно попадает в другое измерение, которое заполнено монстрами и полностю поглащено тьмою. У учёного чудом оказался ссобой фонарик и пара батареек, но спасёт ли его это или убъёт? Сможет он продержаться до открытия портала вновь, или портал до его возвращения?
## Игровой мир
Мир полностью тёмный, монстры отакуют любой светящийся объет. Для монстров свет вреден и является для них угрозой. В этом мире никогда не было видимого для человека света. Он чужеродный и монстры не приспособленны к нему. Тепло рассеивающеся с человека, может приманивать, некоторых монстров.
## ГейМплей
### Механики:
У игрока есть слабый фонарик.
Фонарик: в форме элипса из двух окружностей Из 
Область освещения является сектор с центром на игроке и направлением биссектрисы на курсор игрока.
При включении фонарика Монстры находящиеся радом с игроком (растояние 15-20 метров, Условие между игроком и монстром нет препятсвий) начинают двигатсья в сторону игрока. 
Фонарик светит 100 секунд, после требуется поменять батарейки.(Игровая условность, у игрока бесконечное количество батареек)

Смена батареек: занимет 10 секунд, есть вероятность события "уронил батарейки" 50% что время увеличится на 10 секунд, не может возникнуть больше одного раза за смену батареек.

Уровень агресии: у монстров 3 уровня агресии 
     0-й монстры двигаются в случайном направлении или в направлнеии, где ранее был замечен ими игрок.
     1-й монстры двигаются с обычной скоростью в направлении игрока.
     2-й Монстры Действуют согласно своему поведению
## Объекты:
###статичные обЪекты:
####Не активные:
Стена
пол
####Активные:
портал
###Динамические объекты:
####игрок:
не имеет здоровья (Любой монстр при соприкосновении хитбоксов мгновенно убивает игрока)
#### Монстры:
1)Тёмная псина (на 1-ом уровне агресии скорость Х1.3 от скорости бега игрока, на 2-ом уровне агресии убегает от игрока (второй уровень агресии длится 10 секунлд))

2)Тёмный жнец (на 2-ом уровне агрессии скорость равная скорости бега игрока, в 1-ом уровне агресии движется со скоростью равной шагу игрока)

3)Тёмный титан (на всех уровнях агресии скорость Х0.5 от скорости бега игрока, если игрок находится на растоянии близком к Тёмному титану, то последний переходит на первый уровень агресии)
##Взаимодествия:
