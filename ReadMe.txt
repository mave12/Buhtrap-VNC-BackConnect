BC-Server. ?????? 2.7.17.1
--------------------------

?????????-?????? ??? ????????????? ? SOCKS ? VNC.

??? ???????, ?????????-?????? ????????? ???? ??? ????????? TCP ?????? (????????? ?????), ? ???????, ? ??????????, 
 ???????????? ????????? ?????????? (????? ??????: ??????(?)).
?????? ???????? ID ??????? ?? ??????? ?? ????????. ?????????-?????? ???????????? ??????????? ? ???? ??????, ????????? ?
 ??????? ?????????? TCP-????. ? ??????????? ?????, ? ??????????, ??????????? ???? ??? ????????? ????????.
?????? ?????????-??????? ?? ???? ????? ???????? ? ????, ????? ??????? ????????? ??????????? ??????????? ??????????????
 ???????????? ????????? ???????????.

?????????-?????? ???????????? ???? ???????? (\BcServer\bcserver.ini).
??? ??????? ???? ?????? GeoIp ?? MySQL ???????, ?????????-?????? ???????? ?????????? ??????, ? ??????? ?????????,
 ?????????????? ??????, ?? ??? IP-??????.

 
????????? ?????????? ???? ?????? MySQL-?????? ??? ???????? ?????????? ???????????. 
? ???? ?????? ??????????? ????????? ?????????: 
	- CreateTime	- ????? ???????? ?????? (????? ??????? ?????????? ???????);
	- AccessTime	- ????? ?????????? ?????? (????? ?????????? ??????????? ???????);
	- ServerPort	- TCP-????, ?????????? ??? ???????;
	- ClientPort	- TCP-????, ?????????? ??? ???????;
	- Address		- IP-????? ???????;
	- Flags			- ???? ????????? ?????????? (1 - ?????? ?????????, 0 - ????????);
	- UserId		- ID ??????? ?? ??????? ???????? ??????;
	- CountryCode	- ????????? ??? ?????? ??? ???????? ??????;
	- LoadPct		- % ???????? ???????. ???????????? ??? ????????? ????? ???????? ??????????? ? ???-?? 
						?????????? ????????????	?? ??????.

?????????????? ?????? ? ?????? ????????? ? ???????? ??????? WIN32
??? ????? ?????:
- ???????????????? ????????? ??? ?????? WIN32, ???????? ????????? ???????:
	sc create "BcServer" binPath= "c:\bcserver\bcserver.exe" start= auto
- ????????? ??????:
	net start bcserver
	

?????? ???????:

\BcServer		- ??? ????????? ???????. ?????????? ? ??????????? ???? WIN32.
\Handle			- ??? ???-??????? ???????, ???????????? ??? ???????? ?????????? ?????????? ? ????????????.

\bcserver.sql	- ?????? ??? ???????? ???????????? ? ???? ?????? ?????????-??????? ?? MySQL-???????.
\geoip.sql		- ?????? ??? ?????? GeoIp.csv ?? MySQL-??????.

\bcserver.ini	- ?????? ????? ???????? ???????.

\sslcerts.bat	- ?????? ??? ????????? SSL ?????? ??????? ? ???????.


??? ????? ??? ??????:

1. MS Visual Studio 2005;
2. MS Windows7 SDK;
3. MySQL Connector/C (http://www.mysql.com/downloads/connector/c/)

????? ????????? MySQL Connector ?????????? ????????? ? VS ???? ? .H ? .LIB ?????? ??? MySQL.
?????????? LIBMYSQL.DLL ?????????? ??? ?????? ?????????-???????.
