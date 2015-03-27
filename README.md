Following the first (Tutorial) section from Hibernate 4.3.8 manual

Steps:
- Launch HSQLDB server by running
	mvn exec:java -Dexec.mainClass="org.hsqldb.Server" -Dexec.args="-database.0 file:target/data/tutorial"
- Compile the project by running
	mvn compile
- Store your first Event by running
	mvn exec:java -Dexec.mainClass="org.hibernate.tutorial.EventManager" -Dexec.args="store"
