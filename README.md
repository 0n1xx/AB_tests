### О репозитории:

В данном репозитории находяться проекты и учебные материалы по статистике и A/B тестам. В самх проектах показаны какие статистические критерии можно использовать в ходе проверки гипотез.

### Немного про условия по каждому проекту каждому проекту проекту:

##### Учебные:
____

- [A/A tests](https://github.com/0n1xx/AB_tests/blob/main/Studies/AA_tests/aa_studies.ipynb): 

  Задачи:
  1. Запустите A/A-тест;
  
  2. Посчитайте FPR на уровне альфа = 0.05 (ставьте подвыборки без возвращения объемом 1000). Вы увидите, что FPR > альфа! Нам нужно наоборот – чтобы было меньше;
  
  3. Найдите причины поломки сплит-системы, ориентируясь на результаты эксперимента (подсказка: найдите аномалию в версии приложения);
  
  4. Напишите выводы, которые можно сделать на основе анализа результатов A/A-теста.


- [A/B tests](https://github.com/0n1xx/AB_tests/blob/main/Studies/AB_tests/ab_studies.ipynb): в данном проекте я генерировал и проверял различные гипотезы при помощи таких статистических критериев как:Манна-Уитни, Шапиро-Уилка, а также использовал Bootstrap.

  Задачи:

  1. Проверьте, есть ли различия в размерах оттока клиентов в разных городах (churn, city);
  
  2. Есть ли разница в активности в первые 30 дней с момента регистрации между водителями из разных городов? (city, trips_in_first_30_days);
  
  3. Может ли отток быть связан с активностью в первые 30 дней после регистрации? (churn, trips_in_first_30_days)
  Перед проведением тестов проверьте распределения переменных, а также удовлетворяются ли параметрические условия.


- [Bootstrap](https://github.com/0n1xx/AB_tests/blob/main/Studies/Intro_boostrap/bootstrap_studies.ipynb):

  Задачи:
  1. Сравните результат между тестом и контролем по двум кейсам:
    Примените бутстрап (с np.mean) и критерий mann-whitney, а потом сравните p-value
    Примените бутстрап (с np.median) и критерий mann-whitney, а потом сравните p-value.
    
  2. Напишите выводы, которые можно сделать на основе анализа примененных критериев


#### Проекты:
____

- [A/B тест и retention](https://github.com/0n1xx/AB_tests/blob/main/Projects/AB_retention/retention_ab_test.ipynb):

  Представьте, что вы работаете в компании, которая разрабатывает мобильные игры. К вам пришел менеджер с рядом задач по исследованию нескольких аспектов мобильного приложения:

  1. В первую очередь, его интересует показатель retention. Напишите функцию для его подсчета;
  
  2. Помимо этого, в компании провели A/B тестирование наборов акционных предложений. На основе имеющихся данных определите, какой набор можно считать лучшим и на основе каких метрик стоит принять правильное решение;
  
  3. Предложите метрики для оценки результатов последнего прошедшего тематического события в игре.


- [A/B тест](https://github.com/0n1xx/AB_tests/blob/main/Projects/AB_test/ab_test.ipyn):

  Представьте, что вы работаете в крупном дейтинговом приложении.

  Помимо базовых функций, в приложении также имеется премиум-подписка, которая дает доступ к ряду важных дополнительных возможностей. Был проведен A/B тест, в рамках которого для новых пользователей из нескольких стран была изменена стоимость премиум-подписки* при покупке через две новые платежные системы. При этом стоимость пробного периода оставалась прежней.

  Проверьте:

  1. Был ли эксперимент успешен в целом;
  
  2. Проанализируйте, имеет ли нововведение смысл среди каких-либо конкретных групп пользователей.
