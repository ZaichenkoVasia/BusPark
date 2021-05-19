# Емулятор зчитувача карточки автобусного парку на основі мікрокомпютера

## Опис

Емулятор зчитувача карточки автобусного парку на основі мікрокомпютера. В системі існують ролі: драйвер та адміністратор, а також основні сутності автопарку - це автобуси та маршрути. При створенні нового автобусу, адміністратор за допомогою своєї id-карти повинен ідентифікувати особистість. Карт-рідер зчитує карту адміністратора та надає веб-серверу відповідь:
  1) При позитивній валідації — автобус буде успішно добавлений, а також буде продемонстроване відповідне сповіщення
  2) У разі провалу аутентифікації запис не буде добавлено у сховище даних і буде присутнє повідомлення про невдачу

Замість зчитувача безконтактних карт було використано файловий емулятор. Файловий емулятор зчитувача картки містить значення true/false, що відповідають підтвердженню/відхиленню права добавлення адміністратором автобусу. У випадку, коли ми отримаємо значення відмінне від true/false доступ буде відхилений. При початку роботи програмного забезпечення створюється файл емулятор зчитувача безконтактних карт із значенням false. При завершенні роботі даний файл буде видалено.
  Допоміжний функціонал веб-сервісу: адміністратор може призначити вільні автобуси маршрутам, автобусам вільних драйверів, а також розпустити їх, зробивши їх вільними. Водій може бачити місце роботи, і він також повинен підтвердити своє нове призначення.

### Дані для входу
- Admin - login: admin@gmail.com password: admin
- Driver - login: driver1@gmail.com password: driver
