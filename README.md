<!-- This is an educational repository that contains homeworks, completed as part of Vadim Ksendzov's training course on software testing.
Here I am learning how to work in GitHub.
Below is my homework and solution -->


XML
 #Создать внешний репозиторий c названием XML.
 #На гитхабе создаем новый публичный репозиторий XML 
 
 #Клонировать репозиторий XML на локальный компьютер.
 #Копируем ссылку на репозиторий https://github.com/gadaborshev/gr29_github_xml.git
 
	$ git clone https://github.com/gadaborshev/gr29_github_xml.git
	Cloning into 'gr29_github_xml'...
	remote: Enumerating objects: 3, done.
	remote: Counting objects: 100% (3/3), done.
	remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
	Receiving objects: 100% (3/3), done.

 #Внутри локального XML создать файл “new.xml”.
 
	touch new.xml
  
 #Добавить файл под гит.
	
	git add new.xml
	
 #Закоммитить файл.
 
	$ git commit -m "created file new.xml"
	[main 26a6944] created file new.xml
	1 file changed, 0 insertions(+), 0 deletions(-)
	create mode 100644 new.xml

	
 #Отправить файл на внешний GitHub репозиторий.
	
	$ git push
	Enumerating objects: 4, done.
	Counting objects: 100% (4/4), done.
	Delta compression using up to 12 threads
	Compressing objects: 100% (2/2), done.
	Writing objects: 100% (3/3), 278 bytes | 278.00 KiB/s, done.
	Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
	To https://github.com/gadaborshev/gr29_github_xml.git
    060edce..26a6944  main -> main


 #Отредактировать содержание файла “new.xml” - написать информацию о себе (ФИО, возраст, количество домашних животных, будущая желаемая зарплата). Всё написать в формате XML.
 
	vim new.xml 
	<xml>
		<Identity>"Gadaborshev Ruslan Tarkhanovich"</Identity>
		<Age>"41"</Age>
		<Pets>"I don't have pets, but I have three children :-)"</Pets>
		<DesiredSalary>"Let's start with $1000"</DesiredSalary>
		
 #Отправить изменения на внешний репозиторий.
 
	$ git add new.xml; 
	$ git commit -m "added some info about me"
	main fe771b7] added some info about me
	1 file changed, 6 insertions(+)
	$ git push
	Enumerating objects: 5, done.
	Counting objects: 100% (5/5), done.
	Delta compression using up to 12 threads
	Compressing objects: 100% (3/3), done.
	Writing objects: 100% (3/3), 436 bytes | 436.00 KiB/s, done.
	Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
	To https://github.com/gadaborshev/gr29_github_xml.git
    26a6944..fe771b7  main -> main

 
 #Создать файл preferences.xml
 
	vim preferences.xml
	
 #В файл preferences.xml добавить информацию о своих предпочтениях (Любимый фильм, любимый сериал, любимая еда, любимое время года, сторона которую хотели бы посетить) в формате XML.
 
	<xml>

		<FavoriteMovie>"There are a lot of them"</FavoriteMovie>
		<FavoriteSeries>"Silicon Valley"</FavoriteSeries>
		<FavoriteFood>"Seafood"</FavoriteFood>
		<CountryIWouldLikeToVisit>"USA"</CountryIWouldLikeToVisit>
 
 
 #Создать файл sklls.xml добавить информацию о скиллах которые будут изучены на курсе в формате XML
 
	vim sklls.xml
	<xml>
		<skill>"Basic theory (What is testing, bug reports, documentation, types, methods, areas of testing, etc.) SDLC, STLC"</skill>
		<skill>"What is a client-server architecture"</skill>
		<skill>"HTTP Methods of requests to the server"</skill>
		<skill>"HTTP server response codes"</skill>
		<skill>"Structures of HTTP requests and responses"</skill>
		<skill>"What is JSON, XML. Their structure"</skill>
		<skill>"API testing via Postman (JS, API autotests)"</skill>
		<skill>"Removing and reading logs from an external server"</skill>
		<skill>"Sniffing http web traffic via Charles and Fiddler"</skill>
		<skill>"Dev Tools of web browsers (Google Chrome, FireFox)"</skill>
		<skill>"VPN. (How it works, why you need it, how to use it, tool options)"</skill>
		<skill>"Mobile testing"</skill>
		<skill>"Feature iOS, Android, guidelines"</skill>
		<skill>"Building iOS applications on XCode. (Those who do not have a Mac computer, just look)"</skill>
		<skill>"Building Android applications on Android Studio"</skill>
		<skill>"ADB (android device management)"</skill>
		<skill>"Setting up proxy and vpn on iOS and Android"</skill>
		<skill>"nterception (sniffing) of mobile traffic via Charles and Fiddler on iOS and Android"</skill>
		<skill>"Command line (terminal) Linux (copying, creating, viewing, moving files on servers without a graphical interface)"</skill>
		<skill>"Basics of bash scripting, automation of routine tasks on the server"</skill>
		<skill>"Basics of bash scripting, automation of routine tasks on the server"</skill>
		<skill>"Access to remote servers"</skill>
		<skill>"SQL basics (Create, Delete, Drop, Insert Into, Select, From, Where, Join)"</skill>
		<skill>"Postgres database (installation, configuration and use)"</skill>
		<skill>"Non-relational database Redis (installation, configuration and use)"</skill>
		<skill>"Load testing in Jmeter"</skill>
		<skill>"Scrum development methodology"</skill>
		<skill>"Python. (Learning the basics. Creating a client-server application)"</skill>
		
 #Отправить сразу 2 файла на внешний репозиторий.
 
	$ git add .
	$ git commit -am "added two new files"
	[main 7406633] added two new files
	2 files changed, 39 insertions(+)
	create mode 100644 preferences.xml
	create mode 100644 skills.xml
	$ git push
	Enumerating objects: 5, done.
	Counting objects: 100% (5/5), done.
	Delta compression using up to 12 threads
	Compressing objects: 100% (4/4), done.
	Writing objects: 100% (4/4), 1.26 KiB | 1.26 MiB/s, done.
	Total 4 (delta 0), reused 0 (delta 0), pack-reused 0
	To https://github.com/gadaborshev/gr29_github_xml.git
	fe771b7..7406633  main -> main

 
 #На веб интерфейсе создать файл bug_report.XML.
 
	done
 
 #Сделать Commit changes (сохранить) изменения на веб интерфейсе.
 
	done
	
 #На веб интерфейсе модифицировать файл bug_report.XML, добавить баг репорт в формате XML.
 
	done
	
 #Сделать Commit changes (сохранить) изменения на веб интерфейсе.
 
	done
	
 #Синхронизировать внешний и локальный репозиторий XML
 
	$ git fetch
	remote: Enumerating objects: 4, done.
	remote: Counting objects: 100% (4/4), done.
	remote: Compressing objects: 100% (3/3), done.
	remote: Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
	Unpacking objects: 100% (3/3), 933 bytes | 2.00 KiB/s, done.
	From https://github.com/gadaborshev/gr29_github_xml
    7406633..3ad0c03  main       -> origin/main
	$ git pull
	Updating 7406633..3ad0c03
	Fast-forward
	bug_report.xml | 10 ++++++++++
	1 file changed, 10 insertions(+)
	create mode 100644 bug_report.xml
