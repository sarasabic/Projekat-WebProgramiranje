**Sistem upravljanja bibliotekom**

Aplikacija u koja ima dvije vrste korisnika, admina i običnog korisnika.

Korisnik ima mogućnost da pregleda knjige, autore i kategorije knjiga.

Admin je korisnik koji ima mogucnost kako pregleda knjiga, autora i 
kategorija knjiga, ima mogućnost i dodavanjem novih knjiga, autora i kategorija
i uređivanja i brisanja istih.

Tehnologije koje su korištene u projektu:

Spring Boot: Framework za brzo razvijanje Java aplikacija.
Spring Security: Za autentifikaciju i autorizaciju korisnika.
Thymeleaf: Java templating engine za kreiranje HTML stranica.
JPA/Hibernate: Za pristup bazi podataka.
PostgreSQL: Relacijska baza podataka.
Lombok: Za automatsko generisanje getter/setter metoda i drugih korisnih metoda.
Maven: Alat za izgradnju projekta.

**Konfigurisanje PostgreSQL baze podataka**

U application.properties fajlu (koji se nalazi u src/main/java/resources direktorijumu), 
postaviti parametre za konekciju sa bazom podataka:

spring.application.name=Projekat
spring.datasource.url=jdbc:postgresql://localhost:5432/postgres
spring.datasource.username=your_username
spring.datasource.password=your_password
spring.datasource.driver-class-name=org.postgresql.Driver
spring.jpa.properties.hibernate.dialect = org.hibernate.dialect.PostgreSQLDialect
spring.h2.console.enabled=true
spring.jpa.hibernate.ddl-auto=update
server.port=8084

Zamijenite your_username i your_password sa Vašim podacima PostgreSQL baze.

Aplikacija koristi Java23(Java Development Kit - JDK)

