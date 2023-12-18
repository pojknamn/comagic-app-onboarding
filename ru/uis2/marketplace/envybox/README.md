### EnvyBox:передача заявок и чатов 
 <br />
 
**Ценность**  <br />  
 
Для получения возможности анализировать эффективность рекламных источников в едином интерфейсе организована передача обращений с виджетов Envybox на сайтах клиента в ЛК CoMagic.  
<br />

**Возможности интеграции**  <br />
Интеграция позволяет передавать информацию в наш ЛК cо следующих виджетов Envybox:  

- обратный звонок, лидогенератор, квизы в качестве заявок;
- чаты  в качестве чатов.
<br />

**Какие данные передаются**    
  
- контактные данные (имя,телефон,email);  
- дата и время создания;  
- вопросы/ответы опроса;
- данные сессии (рекламную компанию, источник, UTM-метки и тд);  
- в случае отсутствия сессии, дефолтную РК или источник.  
<br />


### Подключение интеграции  
 <br />  
 
Интеграция подключается в несколько шагов:  
1. Нажмите "Активен" на этой странице. <br />
2. **Настройте Webhook в Envybox**<br />

<details>
  <summary style="font-weight:bold;"> Подробнее </summary> <br />
  В  Envybox необходимо настроить Webhook на "Webhook url" сервиса CoMagic/UIS из настроек.<br />  
  a. Заходим в  Envybox и выбираем виджет, с которым необходимо произвести настройку и нажимаем настроить.<br />  
  b. Далее в настройках заходим в раздел "Интеграции".<br /> 
  c. В поле "WebHooks уведомления" добавляем наш "Webhook url", а также проставляем галочки в событиях, по которым необходимо слать Webhook.
 
   ![image](env_1.png)![image](env_2.png)  
  Для виджета обратного звонка нужно прожать чек-боксы для пунктов:  
  - Результат звонка (телефон, имя, почта, состоялся/не состоялся, длительность, запись разговора и т.п.)  
  - Заказ звонка в нерабочее время (телефон, имя, почта, откуда пришел, что искал, UTM-метки)  
  ![image](env_3.png)  
  Иначе происходит дублирование заявок.
  
</details> 
<br />

3 **Тип трафика** — необходимо выбрать какую сущность использовать для обращений без сессии. <br />  
В зависимости от выбранного **типа трафика** выводится либо список источников и сайтов  из личного кабинета клиента, либо список рекламных кампаний. Необходимо указать какой **источник и сайт/рекламную кампанию** используем в случае отсутствия сессии. <br /> 

<br />
 
4. Нажмите сохранить. <br />
5. После сохранения будет выведен скрипт, который необходимо установить на сайт в соответствие с описанием в настройках.<br />

После подключения интеграции заявки будут попадать в  Сырые данные -> Обращения и цели.  <br /> 
Для проверки корректности работы интеграции оставьте тестовое обращение в виджете Envybox. <br />

