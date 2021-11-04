# TelegramBot-PostgreSQL
Telegram Bot on Python with the PostgreSQL database integrated into it

Today, cities often host various cultural events.For example, it could be a festival, a concert, a film screening, etc.How can I get to these events?You can get to these events in two ways:

Like a viewer. That is, buy a ticket for this event.
As an employee. That is, a person who has accreditation to attend this event.
Principle of operation: This project implements the following functionality: There is a file with the Telegram-bottom code and there is a file with requests to the database.When a user enters the bot, he presses / start. Then the bot displays a message with buttons (registration, verification, deletion).When a user presses a registration button, he is invited to choose who he wants to go to the event.If he goes as a viewer, then he must enter the ticket number. If he goes as a journalist (conditionally), then he must enter the accreditation number and name of the publication in which he works.If the user does not remember whether he was registered or not, he presses the "check" button, and the bot gives him an indication of what needs to be done. If the user is in the database, he will be given the corresponding message.If the user does not come to the event, and he wants to "cancel the record" he presses the "deleting" button. The bot gives him an indication of what needs to be done and then the user is given a deletion message.

Notes: In both files, the values of some variables have "read readme". This means that these variables contain unique data. What does it mean?This means that this is data that is individual for each user, for example, a token bot. Each bot has its own.Also, unique data includes bot connection data to the database.To use Python to transfer SQL queries, you need to connect to the database. That is, in the code you need to specify the values of the variables: database name, username, password, local host, port.Each user has his own data, he sets them when installing the DBMS and creating the database (you can see the corresponding guides).

Launch: The bot starts using the command line (terminal). To do this, go from the folder where the bot file is located and register the launch command (their methods are in each operating system).For the correct work, a database server must be enabled.
