# SQL Markdown for Cheatsheet.

## Introduktion

Eksempel på SQL Markdown I Github. Denne liste er en referat til SQL begraber til Hovedforløbet.

## kategorier

I SQL(Structured Quary Language) er der kommandoer som er del i kategorier som man bruger til at organizer I forhol til deres funktioner, de er
- DDL: Data Definition Language
- DQL: Data Query Language
- DML: Data Manipulation Language
- DCL: Data Control Language 
- TCL: Transaction Control Language

Desse konmander er målrettet til opgaver så som uplægning af databaser, CRUD modelen, vedligeholde rettiheder og kontroller transaktioner mellem servers og klienter.

### DDL

DDL er den grundlæggenet set af kommandoer i SQL, det er simpelt men også fundementalt at kende dem fordi det inholder Create, Alter Tuncate og Drop

- Create: Skaber en ny tabel I.e Create Table TECTStudentDB
- Alter: Rediger talel til at giv et nyt navn, droppe/slete den. I.e Alter Table Add PostCode INT(255)
  - Rename: Skifter tabelens name når man bruger alter talbe. I.E Alter Table TECTStudentDB Rename to TECTStudentDB1  
- Drop: Sletter talellen: I.e Drop Table TECTStudentDB
- Truncate: Sletter alt data inde i tabelen men ikke selve tabelen. I.e Truncate Table TECTStudentDB

### DQL 

DQL er den mest simple kommando men også en er de meste vigige, fordi den eneste komando der tilhøre den er "Select", hvor man hender data gemmen en query hvor man kan vælge en eller flere kolonner fra en tabel I.E Select Name From TECTStudentDB.


### DML

DML er brugt til at hente, rediger, updater data i en database. De er de komandoer man bruger til at arbejde I database og hånder data. CRUD (Create, Read, Update, Delete) er de fire operationer man bruger til at I SQL


- Create skaber en ny tabel eller database
- Read henter og læser dataen for brugern
- Update rediger og juster data
- Delete sletter data.

Eksempler på kommandoer er:

- Insert: Sætter data in I en tabel Insert into vælger den tabel man vælger og Values er de værdier man vil tilføje I tabelen I.E Insert into TECTStudentDB(StudentID, Name) Values(1, 'Michael Rasmussen')
- Update: Updater eller regider data i tablen. Det er altid en god ide at bruge Primary Keyen som "Where" Syntaksen for at være sikker på at man har valgt en rette felt. I.E Upate TECTStudentDB Set Name = 'Ole'; TECTStudentDB
- Delete: Sletter data I tablen I.E Delete Name Where TECTStudentDB = 1

### DCL

DCL giver eller tag tilladelse til at bruge databasen og framhæve data til at beskyde det fra tyveri eller ander forme af hærværk.

Eksempler på kommandoer er.

- Grant: Giver bruger tilladese til at bruge Databasen I.e Grant Select on TECTStudentDB to "John Walsh", "Shawn Hennesay";
- Rework: Nægter eller tilbage tager retiheder for Datasen. I.e  Revoke Select on TECTStudentDB to  "John Walsh", "Shawn Hennesay";

### TCL Hjælper med at skabe savepoints og kontroller hvordan man gemmer sin database, normalt er databaser sættet til autocommit hvor den automatisk gemmer sin database men det er også godt ha' kontrol over vis man ved uheld sletter eller laver ændringer man gerne vil rette.

Eksempler på kommandoer er:

Autocommit: Gemmer databaseen automatisk I.e Set Autocommit = On/Off;
Commit: Manuelt gemmer sin database
Savepoint: Gemmer database med et bestemt navn I.e Savapoint RedMig 
Rollback: Fremhæver data fra den seneste Commit, vis man skal vælge en savepoint bruger man "Rollback To" komandoen: I.E Rollback to RedMig


## Andre komandoer

## Operators

## Begraber

## Database objekter

## Contrains

## Funktioner 

## Nøgleord

## Joins

## Sæt Operators

## DDL eksempeler

## DQL eksempler

## DML eksempler
