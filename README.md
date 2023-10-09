# Домашнее задание к занятию «Система мониторинга Zabbix. Часть 2»

 ---

### Задание 1
Создайте свой шаблон, в котором будут элементы данных, мониторящие загрузку CPU и RAM хоста.

#### Процесс выполнения
1. Выполняя ДЗ сверяйтесь с процессом отражённым в записи лекции.
2. В веб-интерфейсе Zabbix Servera в разделе Templates создайте новый шаблон
3. Создайте Item который будет собирать информацию об загрузке CPU в процентах
4. Создайте Item который будет собирать информацию об загрузке RAM в процентах

#### Требования к результату
- [ ] Прикрепите в файл README.md скриншот страницы шаблона с названием «Задание 1»

  *Скриншоты задания №1*
  
![Commit Task1](https://github.com/AndrewZnamenskiy/Zabbix_learning_2/blob/main/img/task1p1.png)

![Commit Task1](https://github.com/AndrewZnamenskiy/Zabbix_learning_2/blob/main/img/task1p2.png)

![Commit Task1](https://github.com/AndrewZnamenskiy/Zabbix_learning_2/blob/main/img/task1p3.png)

![Commit Task1](https://github.com/AndrewZnamenskiy/Zabbix_learning_2/blob/main/img/task1p4.png)

 ---

### Задание 2
Добавьте в Zabbix два хоста и задайте им имена <фамилия и инициалы-1> и <фамилия и инициалы-2>. Например: ivanovii-1 и ivanovii-2.

#### Процесс выполнения
1. Выполняя ДЗ сверяйтесь с процессом отражённым в записи лекции.
2. Установите Zabbix Agent на 2 виртмашины, одной из них может быть ваш Zabbix Server
3. Добавьте Zabbix Server в список разрешенных серверов ваших Zabbix Agentов
4. Добавьте Zabbix Agentов в раздел Configuration > Hosts вашего Zabbix Servera
5. Прикрепите за каждым хостом шаблон Linux by Zabbix Agent
6. Проверьте что в разделе Latest Data начали появляться данные с добавленных агентов

#### Требования к результату
- [ ] Результат данного задания сдавайте вместе с заданием 3

 ---

### Задание 3
Привяжите созданный шаблон к двум хостам. Также привяжите к обоим хостам шаблон Linux by Zabbix Agent.

#### Процесс выполнения
1. Выполняя ДЗ сверяйтесь с процессом отражённым в записи лекции.
2. Зайдите в настройки каждого хоста и в разделе Templates прикрепите к этому хосту ваш шаблон
3. Так же к каждому хосту привяжите шаблон Linux by Zabbix Agent
4. Проверьте что в раздел Latest Data начали поступать необходимые данные из вашего шаблона

#### Требования к результату
- [ ] Прикрепите в файл README.md скриншот страницы хостов, где будут видны привязки шаблонов с названиями «Задание 2-3». Хосты должны иметь зелёный статус подключения

  *Скриншоты задания №2-3*
  
![Commit Task2-3](https://github.com/AndrewZnamenskiy/Zabbix_learning_2/blob/main/img/task3p1.png)

![Commit Task2-3](https://github.com/AndrewZnamenskiy/Zabbix_learning_2/blob/main/img/task3p2.png)

![Commit Task2-3](https://github.com/AndrewZnamenskiy/Zabbix_learning_2/blob/main/img/task3p3.png)

![Commit Task2-3](https://github.com/AndrewZnamenskiy/Zabbix_learning_2/blob/main/img/task3p4.png)


 ---

### Задание 4
Создайте свой кастомный дашборд.

#### Процесс выполнения
1. Выполняя ДЗ сверяйтесь с процессом отражённым в записи лекции.
2. В разделе Dashboards создайте новый дашборд
3. Разместите на нём несколько графиков на ваше усмотрение.

#### Требования к результату
- [ ] Прикрепите в файл README.md скриншот дашборда с названием «Задание 4»

  *Скриншоты задания №4*
  
![Commit Task4](https://github.com/AndrewZnamenskiy/Zabbix_learning_2/blob/main/img/task4p1.png)

 ---

### Задание 5* со звёздочкой
Создайте карту и расположите на ней два своих хоста.

#### Процесс выполнения
1. Настройте между хостами линк.
2. Привяжите к линку триггер, связанный с agent.ping одного из хостов, и установите индикатором сработавшего триггера красную пунктирную линию.
3. Выключите хост, чей триггер добавлен в линк. Дождитесь срабатывания триггера.

#### Требования к результату
- [ ] Прикрепите в файл README.md скриншот карты, где видно, что триггер сработал, с названием «Задание 5» 

  *Скриншоты задания №5*
  
![Commit Task5](https://github.com/AndrewZnamenskiy/Zabbix_learning_2/blob/main/img/task5p1.png)

![Commit Task5](https://github.com/AndrewZnamenskiy/Zabbix_learning_2/blob/main/img/task5p2.png)

![Commit Task5](https://github.com/AndrewZnamenskiy/Zabbix_learning_2/blob/main/img/task5p3.png)

 ---

### Задание 6* со звёздочкой
Создайте UserParameter на bash и прикрепите его к созданному вами ранее шаблону. Он должен вызывать скрипт, который:
- при получении 1 будет возвращать ваши ФИО,
- при получении 2 будет возвращать текущую дату.

#### Требования к результату
- [ ] Прикрепите в файл README.md код скрипта, а также скриншот Latest data с результатом работы скрипта на bash, чтобы был виден результат работы скрипта при отправке в него 1 и 2
 
   *Скриншоты задания №6*
  
![Commit Task6](https://github.com/AndrewZnamenskiy/Zabbix_learning_2/blob/main/img/task6p1.png)

![Commit Task6](https://github.com/AndrewZnamenskiy/Zabbix_learning_2/blob/main/img/task6p2.png)

![Commit Task6](https://github.com/AndrewZnamenskiy/Zabbix_learning_2/blob/main/img/task6p3.png)

 
 ---

### Задание 7* со звёздочкой
Доработайте Python-скрипт из лекции, создайте для него UserParameter и прикрепите его к созданному вами ранее шаблону. 
Скрипт должен:
- при получении 1 возвращать ваши ФИО,
- при получении 2 возвращать текущую дату,
- делать всё, что делал скрипт из лекции.

- [ ] Прикрепите в файл README.md код скрипта в Git. Приложите в Git скриншот Latest data с результатом работы скрипта на Python, чтобы были видны результаты работы скрипта при отправке в него 1, 2, -ping, а также -simple_print.*
 
 ---

### Задание 8* со звёздочкой

Настройте автообнаружение и прикрепление к хостам созданного вами ранее шаблона.

#### Требования к результату
- [ ] Прикрепите в файл README.md скриншот правила обнаружения, а также скриншот страницы Discover, где видны оба хоста.*

   *Скриншоты задания №8*
  
![Commit Task8](https://github.com/AndrewZnamenskiy/Zabbix_learning_2/blob/main/img/task8p1.png)

![Commit Task8](https://github.com/AndrewZnamenskiy/Zabbix_learning_2/blob/main/img/task8p2.png)

![Commit Task8](https://github.com/AndrewZnamenskiy/Zabbix_learning_2/blob/main/img/task8p3.png)

![Commit Task8](https://github.com/AndrewZnamenskiy/Zabbix_learning_2/blob/main/img/task8p4.png)

![Commit Task8](https://github.com/AndrewZnamenskiy/Zabbix_learning_2/blob/main/img/task8p5.png)

 ---

### Задание 9* со звёздочкой

Доработайте скрипты Vagrant для 2-х агентов, чтобы они были готовы к автообнаружению сервером, а также имели на борту разработанные вами ранее параметры пользователей.

- [ ] Приложите в GitHub файлы Vagrantfile и zabbix-agent.sh.*

## Критерии оценки

1. Выполнено минимум 4 обязательных задания
2. Прикреплены требуемые скриншоты, код и файлы 
3. Задание оформлено в шаблоне с решением и опубликовано на GitHub

