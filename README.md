# database-systems
-- create
CREATE TABLE SPECIES (
  speciesid INTEGER PRIMARY KEY,
  name TEXT NOT NULL,
  height INTEGER,
  weight INTEGER
);

-- insert
INSERT INTO SPECIES VALUES (0001, 'Hippo', 36,450);
INSERT INTO SPECIES VALUES (0002, 'Lion',37,370);
INSERT INTO SPECIES VALUES (0003, 'Fish', 26,210);
INSERT INTO SPECIES VALUES(0004,'Buffalo',40,348);
-- fetch 
SELECT * FROM SPECIES WHERE speciesid = 0003;

--create
CREATE TABLE HABITAT (
  habitatid INTEGER PRIMARY KEY,
  name TEXT NOT NULL,
  location TEXT NOT NULL,
  area INTEGER
  );
  
--insert
INSERT INTO HABITAT VALUES(00096,'Kilgoris','Roysambu',32);
INSERT INTO HABITAT VALUES(00097,'Bakambu','Olekarai',42);
INSERT INTO HABITAT VALUES(00098,'Malkameri','Narok',52);
INSERT INTO HABITAT VALUES(00098,'Namanga','Samburu',60);
--fetch
SELECT * FROM HABITAT WHERE habitatid = 00097;

--create
CREATE TABLE PROJECT (
 projectid INTEGER PRIMARY KEY,
 name TEXT NOT NULL,
 startdate INTEGER,
 enddate INTEGER,
 budget INTEGER,
 status TEXT NOT NULL
 );
 
 --insert
INSERT INTO PROJECT VALUES(000178,'Astra',2024-11-23,2025-05-02,25000,'Progress');
INSERT INTO PROJECT VALUES(000179,'Ares',2024-10-09,2026-07-17,100000,'Pending');
INSERT INTO PROJECT VALUES(000180,'Rogue',2024-08-11,2027-04-12,600000,'Declined');
INSERT INTO PROJECT VALUES(000181,'Ankles',2024-02-03,2026-05-25,30000,'Progress');
INSERT INTO PROJECT VALUES(000182,'Infra',2023-04-12,2024-09-20,50000,'Completed');
INSERT INTO PROJECT VALUES(000183,'Yego',2025-06-10,2028-03-21,200000,'Pending');
--fetch 
SELECT * FROM PROJECT WHERE projectid = 000180;

--create
CREATE TABLE RESOURCES (
resourceid INTEGER PRIMARY KEY,
name TEXT NOT NULL,
quantity INTEGER
);

--insert
INSERT INTO RESOURCES VALUES(000678,'Food',300);
INSERT INTO RESOURCES VALUES(000679,'Rangers',600);
INSERT INTO RESOURCES VALUES(000680,'Vehicles'40);
--fetch
SELECT * FROM RESOURCES WHERE resourceid = 000679;

GO
