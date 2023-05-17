# baza
baza podataka skole

Upiti :

Koliko ima djaka s imenom i prezimenom i vecim prosekom od 9 :
SELECT COUNT(*) AS Broj_Studenti
FROM skola
WHERE Ime = 'Dusan' AND Prezime = 'Glisic' AND Prosek > 9;

Svi djaci s vecim prosekom od 8 :
SELECT * FROM `skola` WHERE prosek > 8

Koliko ima djaka s prezimenom Taskovic :
SELECT COUNT(*) AS Broj_Studenti FROM skola where prezime = 'Taskovic';

Koliko ima djaka s imenom Dusan :
SELECT COUNT(*) from skola where ime = 'Dusan';

Na bazu se logujemo kao user root i password=NEWPASSWORD to sam postigao na sledecim upitom:
use mysql;
UPDATE user SET authentication_string=PASSWORD("NEWPASSWORD") WHERE User='root';

Primarni kljuc je jmbg zato sto je jedina unique not null kolona.
