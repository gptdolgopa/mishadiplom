1. В директории ***experiments ***хранятся результаты моей дипломной работы (описание задачи в  ***README.md*** , код и другие полезные материалы). код drive_portfolio_optimization.ipynb не работает как нужно, но поверхностно содержит примерное решение.
2. Необходимо написать на основе этих результатов диплом на русском языке.
3. Шаблон диплома в латехе есть в директории ***Bachelor-Thesis-Template***
4. Изучи требования к диплому в файле ***diploma_requirements.md***
5. Прочитай презентацию `НИС_ДИПЛОМ_Зятьков.pptx-2.pdf` с рассказом диплома. В ней нет ответов на следующие вопросы:

   1. Какими метриками сравнивалось качество catboost и BNN в случае предсказания апостериорного распределения?
   2. Был ли в экономическом эффекте учтены выплаты по SLA?
   3. про функцию выживаемости. более глобально зачем теория выживания в данной работе?
6. Напиши диплом в соседней директории ***diploma ***по шаблону
7. Декомпозируй эту задачу на подзадачи, например:

   1. обзор существующих решений с байесовским подходом и фронтом паретто.
   2. обучение классификатора catboost с использованием VirtEnsembles для оценки апостериорной вероятности
   3. построение экономической модели доходов для политики замены дисков. Учет выплат по SLA, количества дисков на складе.
   4. оптимизация pymoo с подбором пороговых вероятностей для построения фронта паретто оптимальных решений для закупки дисков
   5. сравнение моделей catboost, bayesian neural network, baseline weibull MLE
8. Если каких-то ресурсов или данных для шаблона не хватает, не нужно ничего придумывать, просто оставь пустые секции



Важные комментарии по докладам, как их можно улучшить.

1. Начинать доклад следует с постановки какую именно вы решали задачу и что являлось критерием успеха, что именно вы улучшали. Сделать технологию - это не результат. Результат - это определенные характеристики и выполнение критериев. То есть не "сделали технологии", а "сделали технологию, которая обладает уникальными характеристиками - выполнение вот этих критериев"
2. Излагайте в формате "пирамиды Минто", поищите что это означает. Если коротко, то
   Пирамида Минто строится сверху вниз:
   Главный вывод (тезис) – на вершине.
   Аргументы – уровнем ниже, логически обосновывают вывод.
   Поддержка (факты, данные) – в основании.
   Каждый уровень отвечает на вопрос предыдущего.
   Принцип: От общего – к частному, от идеи – к доказательствам.

Коротко: «Иерархия мыслей: вывод → аргументы → факты».

3. Стиль. Представляйте, что ваш рассказ - это написание научной например математической книги. Не допустимы "что-то", "как-то", частые местоимения "я", "мое", жаргонизмы, шуточки, веселые словечки ит .п.

Например
"ну я как-то это проверил" -> "была выполнена проверка по разработанной методике".
"bnn-ка" -> "Байесовская нейронная сеть, для укорачивания я буду пользоваться далее термином БНН"
"апишка" -> "эй пи ай" или "программный интерфейс"

Еще совет - не читайте со слайдов. Слайды - это поддержка вашего рассказал. Рассказ главное, а на слайдах сопутсвующий и помогающий материал. Слайды с большим объемом текста лучше заменить на схему или визуальное описание этого текста, а текст вы скажите вслух.

не используйте приемы манипуляции аудиторией вообще, они неуместны.
Например, "что такое отладка все знают, сосредотачиваться на этом не будем". Либо это вообще не надо говорить, либо все-таки описать, что это такое.

По результатам пред-защиты буквально у всех одно и то же очень серьезное замечание - лучше описать результат. Он не должен быть в абстрактных понятиях "улучшили", "отмасштабировали", "упростили" - все должно подтверждаться метриками. И это самое главное, гораздо важнее, чем описание технологии.
