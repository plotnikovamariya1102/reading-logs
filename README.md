**Задача:**

В приложении BonusService содержется ошибка, которую можно найти с использованием команды в Maven: mvn clean compile spotbugs:check

Прочитать логи, устранить ошибку.

**Решение:** 

На основе представленных файлов создан Maven проект, применена команда: mvn clean compile spotbugs:check, получена ошибка: Return value of method without side effect is ignored.

Изменен код: 

ДО: 

**service.calculate(amount, registered)**

ПОСЛЕ:

**System.out.println(service.calculate(amount, registered))**
