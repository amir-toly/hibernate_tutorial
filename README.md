Following the first (Tutorial) section from Hibernate 4.3.8 manual

Steps:
- Launch HSQLDB server by running
	mvn exec:java -Dexec.mainClass="org.hsqldb.Server" -Dexec.args="-database.0 file:target/data/tutorial"
- Compile the project by running
	mvn compile
- Store your first Event by running
	mvn exec:java -Dexec.mainClass="org.hibernate.tutorial.EventManager" -Dexec.args="store"
- List existing events by running
	mvn exec:java -Dexec.mainClass="org.hibernate.tutorial.EventManager" -Dexec.args="list"
- Create an event and a person, then bind them together by running
	mvn exec:java -Dexec.mainClass="org.hibernate.tutorial.EventManager" -Dexec.args="addpersontoevent"
- Create a person and the corresponding email address by running
	mvn exec:java -Dexec.mainClass="org.hibernate.tutorial.EventManager" -Dexec.args="addemailaddressforperson"
- Run (you may have to re-import as a Maven Project and clean before) on Tomcat server and go to
	http://localhost:8080/hibernate-tutorial/eventmanager
