# DS-information-sharing-blog
This project includes the implemantation of a blog. The content of the blog should be available for students to get information about the University and tips for studying. It should also be possible to communicate, like and comment on entries.  


To-DOs: 


Client:
- getBlogEntries():
	- Anfrage an Server, Server soll Blog-Einträge übermitteln
	- Einträge müssen modelliert werden
	- Plotte Eintrag mit seinen Kommentaren und likes

- addBlogEntries():
	- Broadcast liefert den Eintrag den Server 
	- Server added die Nachricht in die DB
	- Response von Server an den Author: z.B. True, false als Bestätigung, 
	dass Add erfolgt ist

- setComments(blogID): 
	- Kommentar an Server senden
	- Response von Server an den Kommentar-Author: z.B. True, false als Bestätigung, 
	dass Kommentar erfolgt ist

- setLikes(blogID):
	- Like an Server senden
	- Check ob like bereits vorhanden
	- Response von Server an den Liker: z.B. True, false als Bestätigung, 
	dass Like erfolgt ist

- deleteBlogEntries(blogID, userName):
	- ist userName berechtigt?
	- existiert dieser Eintrag in der DB?
	- anfrage bzgl. löschen an Server (Server gibt weiter an DB)
	- Response an Client mit true oder false

- updateBlogEntries(blogID, userName)
	- ist userName berechtigt?
	- existiert dieser Eintrag in der DB?
	- anfrage bzgl. update an Server (Server gibt weiter an DB)
	- Response an Client mit true oder false

- deleteComments(blogID, userName)
	- ist userName berechtigt?
	- existiert dieser Eintrag in der DB?
	- anfrage bzgl. delete an Server (Server gibt weiter an DB)
	- Response an Client mit true oder false

- deleteLike(blogID, userName)
	- ist userName berechtigt?
	- existiert dieser Eintrag in der DB?
	- anfrage bzgl. löschen oder zurückziehen an Server (Server gibt weiter an DB)
	- Response an Client mit true oder false

Server:


Datenbank:


WebBrowser / HTML:
