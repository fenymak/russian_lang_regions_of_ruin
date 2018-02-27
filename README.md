# Regions Of Ruin
Перевод для Regions Of Ruin (http://www.regionsofruin.com/)

Смотрите: https://github.com/fenymak/russian_lang_regions_of_ruin/

Спасибо всем, кто будет помогать в переводе!

Чтобы заменить вручную шрифт в игре на тот, что будет добавлен позже для поддержки русского языка, проделайте следующее:

1. Откройте программу UnityEX (здесь есть)
2. Откройте с помощью её архив игры sharedassets0.assets (советую сделать бекап)
3. Найдите оба шрифта по названию (здесь есть)
4. Извлеките их (без конвертации), выделив оба ПКМ и выбрав соответствующее действие
5. Далее разместите обновлённые шрифты в \Regions Of Ruin\Regions of Ruin_Data\Unity_Assets_Files\sharedassets0\ с заменой
6. Запакуйте архив в программе, нажав в верхней её части соответствующую кнопку

Если что-то не понятно, добро пожаловать в офф. канал по игре в Discord: https://discord.gg/656MPe5

# Рекомендации по переводу


	+===============================================+
	|		ОГРОМНОЕ СПАСИБО !!!		|
	|						|
	|	Перевод - это большая работа, и мы	|
	|	очень благодарны за вашу помощь.	|
	|						|
	+===============================================+



		-=-=-=-= КАК РАБОТАТЬ =-=-=-=-=-

Перевести нужно около 40,000 слов,
к счастью, сам процесс довольно прост.

В этом наборе локализации вы найдёте несколько файлов:

- English_dialog_messages.txt
- English_injury_messages.txt
- English_UI_messages.txt

и так далее...

Если вы откроете файл, вы увидите несколько строк, разделённых символом «%».

	- !!! НЕ УДАЛЯЙТЕ ИЛИ НЕ ПЕРЕМЕЩАЙТЕ % !!!
	
Всё, что находится между символами «%» - текст, который нужно
перевести. Если вам нужно использовать символ «%», используйте «$»
вместо него, который будет заменён в игре на «%».

Например, «Hello.%» нужно просто заменить на «Bonjour.%»
Всегда оставляйте символ «%» в конце сегмента.
А «Gain 10$ more.%» будет выглядеть в игре как «Gain 10% more.»

Вы можете найти несколько повторяющихся строк, пожалуйста, скопируйте и вставьте перевод
или обработайте их как обычные строки.

	- !!! НЕ УДАЛЯЙТЕ И НЕ ПЕРЕМЕЩАЙТЕ ПОВТОРЯЮЩИЕСЯ СТРОКИ !!! -
(Их немного и расположены они близко друг к другу.)

Если вы найдёте что-то подобное: [MappedKey:Submit] - НЕ УДАЛЯЙТЕ ЭТО.
Это будет автоматически заменено на текст привязки. Вместо этого переместите
[MappedKey] туда, где должна отображаться привязка клавиши.

Например, «Press the [MappedKey:Attack] button» может быть изменена на
«The [MappedKey:Attack] button is for attacking» и т.д., что в конечном итоге будет выглядеть как:
«The Right Trigger button is for attacking.»

Как долго вы закончили перевод текста в .txt файлах, смените
название «English_» на новый язык.

Например, «English_UI_messages.txt» вы можете изменить
на «French_UI_messages.txt»

		-=-=-=-= ГЕНЕРАЦИЯ ПРЕДМЕТОВ =-=-=-=-=-

Есть четыре отдельных файлы для генерации названия предмета:
	- English_item_prefixes.txt
	- English_item_materials.txt
	- English_item_types.txt
	- English_item_suffixes.txt
При генерации предмета в игре, он создаётся в таком порядке:
	prefix -> material -> type -> joiner -> suffix
Например, "Cursed Leather Cap of the monkey clan"

Вы можете изменить порядок генерации в English_item_order.txt
НЕ ИСПОЛЬЗУЙТЕ ЗАГЛАВНЫЕ БУКВЫ и ПРОБЕЛЫ.
Например, prefix+type+material+joiner+suffix

В суффиксах вы также найдёте две дополнительные ссылки, (« of the» и « of»)
(« Of the») будет использовать для первых 12 суффиксов, а (« of») для остальных 24.

		-=-=-=-= ГЕНЕРАЦИЯ ИМЁН =-=-=-=-=-

Есть также другие генерирующиеся имена: спутники и вознаграждения. Однако, они просты: name+suffix.

Есть много имён или описаний, которые не могут быть переведены, вы можете придумать свой собственный подходящий компромисс.

Если для перевода вам понадобится suffix+name, просто поменяйте строки местами.

Например, вместо:
- bob%
- fred%
- bill%
- The dumb%
- The silly%
- The idiot%

Вы можете изменить порядок на:

- The dumb%
- The silly%
- The idiot%
- bob%
- fred%
- bill%

(Убедитесь, что вы изменили порядок ВСЕХ имён и ВСЕХ суффиксов. И что они имеют одинаковое количество строк. Например, не заменяйте 5 суффиксов с 10 именами. Их соотношение должно быть 1:1)





















