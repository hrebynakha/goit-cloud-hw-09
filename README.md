1. Створення застосунку в Elastic Beanstalk

Відкрити AWS Elastic Beanstalk → Applications.

![eba](images/eba.png)

2. Налаштування середовища

Відкрити Elastic Beanstalk → Configuration → Capacity

- Тип середовища: Web server environment
- EC2 Instance type: t3.micro

![cap](images/cap.png) 

3. Моніторинг і логування

Відкрити Elastic Beanstalk → Monitoring, відображаються метрики:

- CPUUtilization
- RequestCount
- Target response time
![metrics](images/metrics.png)

4. Налаштування масштабування

Відкрити Elastic Beanstalk → Configuration → Scaling

- Min instances: 1
- Max instances: 3
- Scaling trigger: CPUUtilization > 70%

![scale](images/scale.png)

5. Перевірку доступу до застосунку

Відкрити згенерований Elastic Beanstalk URL у браузері.

![url](images/url.png)

6. Stress test

Запуск:
![stress](images/stress.png)

Моніторінг:

![stress-metrics](images/metrics-stress.png)

Сповіщення:

![stress-mail](images/mail.png)

AutoScaling:

![stress-ec2](images/ec2.png)
