# Документация за проект Traveller's app
github: https://github.com/dragosa4a/Traveller-s-app

## Увод
Програма, която позволава на своите потребители да споделята снимки, изживявания и впечатления от своите пътувания по света. Програмата обработва и съхранява данните във файлове.

## Имплементация
Проектът е реализиран чрез съвкупност от класове, които описват дата, пътуване, потребител и база данни от потребители.

Класът, който описва една дата е Date.

Обектите от тип Date съдържат следдните член - данни:

* int day - ден
* int month - месец
* int year - година

Класът, който описва едно пътуване е Trip.

Обектите от тип Trip съдържат следните член - данни:

* char destination[MAX_DEST_SIZE] - дестинация
*	Date from - (дата) начало на пътуването
*	Date to - (дата) край на пътуването
*	unsigned mark - оценка
*	char comment[MAX_COM_SIZE] - коментар
*	vector<string> images - снимки
  
  Класът, който описва един потребител е User.
  
  Обектите от тип User съдържат следните член - данни:
  
  * char username[MAX_SIZE] - потребителско име
	* char password[MAX_SIZE] - парола
	* char email_address[MAX_SIZE + 5] - имейл адрес
	* vector<Trip> personal_database - лична база данни, която съдържа пътуванията на потребителя
	* vector<string> friends - приятели
  
  Класът, който описва базата данни от потребители е Userdatabase.
  
  Обектите от тип Userdatabase съдържат следните член - данни:
  
  * vector<User> users - потребители
  
  Документацията по кода е създадена с Doxygen и се съдържа в Documentation/html/index.html.
  
  ## Инструкции за употреба
  С програмата се работи лесно като единственото, което трябва да правите е да я следвате като отговарята на задаваните от нея въпроси. 
  
  ## Допълнителна информация
  Проектът е реализиран на Visual Studio като е използван езикът за програмиране C++. 
  Относно управлението на динамичната памет:
  * използван е vector, който сам се грижи за паметта
  * използван е string, който сам се грижи за паметта
  
  ## Заключение
  Програмата разполага с приличен на брой функционалности, от които няма да останете разочаровани и вашите емоции ще бъдат споделени.
  Възможно е в бъдеще да бъдат добавени още функционалности като например:
  * списък с любимите дестинации на потребителя
  * предвиждания на разходи за пътуването
