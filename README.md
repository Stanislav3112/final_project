Проводилось тестирование пользовательского интерфейса c элементами позитивного и негативного функционального тестирования исходя из представленных требований c помощью программной библиотеки Selenium WebDriver и фреймворка pytest . 
Использовался шаблон проектирования PageObject.
Список тест-кейсов, чек-лист и баги представлены в файле “тест-кейсы 28 модуль .xlsx”
В файлах:
	test_authorization_by_code_page_rt.py,
	test_authorization_page_rt.py,
	test_registration_page_rt.py
 описана реализация тест-кейсов.

В файле conftest.py реализована логика запуска браузера и добавлен обработчик, который считывает из командной строки параметр browser_name, 
а так же language (если сайт поддерживает разные языки)
Браузер объявлется в фикстуре browser и передается в тест как параметр.

Пример: тест запускается с параметром browser_name следующей командой: 
pytest -v -s --browser_name chrome .\test_authorization_page_rt.py

Install all requirements: pip3 install -r requirements.txt

