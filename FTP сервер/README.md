### Основные задания:

1. Посмотреть содержимое папки:

![Screenshot_3](https://user-images.githubusercontent.com/90050887/147092657-bc10a40a-2b47-4402-aa33-0044e8f7e095.png)
![Screenshot_4](https://user-images.githubusercontent.com/90050887/147092678-33bcecf5-ea70-4f9e-959a-854be764f688.png)


3. Создать папку;

![Screenshot_3](https://user-images.githubusercontent.com/90050887/147092657-bc10a40a-2b47-4402-aa33-0044e8f7e095.png)
![Screenshot_4](https://user-images.githubusercontent.com/90050887/147092678-33bcecf5-ea70-4f9e-959a-854be764f688.png)

Домашняя папка пользователя

![Screenshot_5](https://user-images.githubusercontent.com/90050887/147092682-ab83dd10-7c1c-40fe-ba9c-4ecb0162e7f3.png)

В ней созданная нами

![Screenshot_6](https://user-images.githubusercontent.com/90050887/147092685-d09f929b-ff93-4b89-a439-29d6c189c2f2.png)


5. Удалить папку;

![Screenshot_7](https://user-images.githubusercontent.com/90050887/147092686-81d365be-caa0-465f-abf4-68c325a6240b.png)
![Screenshot_8](https://user-images.githubusercontent.com/90050887/147092688-89b691ab-6c56-4b20-996c-9dcd7d321cdc.png)

![Screenshot_9](https://user-images.githubusercontent.com/90050887/147092714-e6904d6f-0798-46d8-a600-9dd6516effce.png)


7. Удалить файл; Создание и переименование далее
9. Переименовать файл;

![Screenshot_10](https://user-images.githubusercontent.com/90050887/147092711-ad7769ca-e98a-4ef9-b52a-c7b9e6b0c31e.png)
![Screenshot_11](https://user-images.githubusercontent.com/90050887/147092660-4aa15d55-bc9e-48fd-a2d5-b94c66868101.png)

![Screenshot_12](https://user-images.githubusercontent.com/90050887/147092690-7dec547e-028d-4ac6-af99-de3bbcf876fa.png)

![Screenshot_13](https://user-images.githubusercontent.com/90050887/147092691-b127badf-cc45-443b-a548-a3508cf00964.png)
![Screenshot_14](https://user-images.githubusercontent.com/90050887/147092693-311b88b3-818b-43bf-8b8d-06455d7f4db7.png)
![Screenshot_15](https://user-images.githubusercontent.com/90050887/147092697-e419b44b-930a-4a75-b435-4d8b4958b3b9.png)


11. Скопировать файл с клиента на сервер;

![Screenshot_16](https://user-images.githubusercontent.com/90050887/147092698-98ac0505-48fe-400c-97b6-58c4485c899b.png)
![Screenshot_17](https://user-images.githubusercontent.com/90050887/147092719-9a8bcc11-a2ef-487c-b76e-b9e369a3d072.png)


13. Скопировать файл с сервера на клиент;

![Screenshot_18](https://user-images.githubusercontent.com/90050887/147092715-cda49a96-8e86-48a4-b48f-4b2c5deef847.png)
![Screenshot_19](https://user-images.githubusercontent.com/90050887/147092661-3e6d1bcf-6090-48bf-b8e0-be1e36474319.png)

Клиент запущен в корневой директории сервера поэтому получается, что скопировали в рабобую директорию клиент, которая
является и рабочей директорией сервера

![Screenshot_20](https://user-images.githubusercontent.com/90050887/147092701-67864cc4-027c-4df6-aa81-65fcfa599918.png)


15. Выход (отключение клиента от сервера);

командой exit закрывается клиентское приложение


### Дополнительные задания:

1. Ограничьте возможности пользователя рамками одной определенной директории. Внутри нее он может делать все, что хочет: создавать и удалять любые файлы и папки. Нужно проследить, чтобы пользователь не мог совершить никаких действий вне пределов этой директории. Пользователь, в идеале, вообще не должен догадываться, что за пределами этой директории что-то есть.
Как видно было из предыдщуих скринов выйти за пределы папки - корня не может, а это рабочая папка пользователя у admin эта папка - корень сервера.

![Screenshot_21](https://user-images.githubusercontent.com/90050887/147092702-a13774a4-3959-49c7-8d61-a67e30699395.png)
![Screenshot_22](https://user-images.githubusercontent.com/90050887/147092703-69f69e48-b692-468c-bb67-b19af57236d8.png)

3. Добавьте логирование всех действий сервера в файл. Можете использовать разные файлы для разных действий, например: подключения, авторизации, операции с файлами.
Логи пишутся в файл корень сервера log.txt

![Screenshot_23](https://user-images.githubusercontent.com/90050887/147092705-9d389836-2073-455c-a943-c19952ab59f9.png)
![Screenshot_24](https://user-images.githubusercontent.com/90050887/147092708-d411ad5b-3499-4577-bd21-a8d91f386ff8.png)


5. Добавьте возможность авторизации пользователя на сервере.
Можно увидеть на каждом скриншоте.
7. Добавьте возможность регистрации новых пользователей на сервере. При регистрации для пользователя создается новая рабочая папка (проще всего для ее имени использовать логин пользователя) и сфера деятельности этого пользователя ограничивается этой папкой.
пользоваталь вводит логин пароль, если такой пользователь не существует - то создается, если существует, то проверяется корректность введенных данных.

![Screenshot_25](https://user-images.githubusercontent.com/90050887/147092722-edaf3d21-5c63-4e04-9ebe-0da41efe7e34.png)

Неудачная авторизация
9. Реализуете квотирование дискового пространства для каждого пользователя.
По 10Мб на пользователя, пример неудачной попытки:

![Screenshot_29](https://user-images.githubusercontent.com/90050887/147094182-86192a69-51cb-46d1-83b0-b8c1f384082a.png)

Папка весит уже больше 10Мб.

![Screenshot_26](https://user-images.githubusercontent.com/90050887/147092721-bfd7b7eb-f481-4154-879d-84f454d853ff.png)
![Screenshot_27](https://user-images.githubusercontent.com/90050887/147092653-08d28494-a294-4f12-9715-2f559f773471.png)


11. Реализуйте учётную запись администратора сервера.

log/pass =  admin/admin, рабочая директория - рабочая директория сервера, то есть папка с папками пользователя
13. Напишите отладочный клиент. Клиент должен подключаться к серверу и в автоматическом режиме тестировать корректность его работы. Используйте подход, аналогичный написанию модульных тестов. Клиент должен вывести предупреждающее сообщение, если сервер работает некорректно. 
файл ftp-test-client log/pass = test/test

![Screenshot_28](https://user-images.githubusercontent.com/90050887/147092710-1e5afbe6-55e5-45e4-9aab-bcbd0eed8a84.png)
