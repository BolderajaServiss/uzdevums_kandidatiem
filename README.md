#Darbinieku darba laiku atskaite no SQLite datubāzes

#Resursi:
Tev tiek dots SQLite datubāzes fails: attendance.db
Šajā datubāzē ir divas tabulas:
Employees
id	username
1	janis
2	liga
3	juris
4	dace

Attendance
id	employee_id	date	hours_worked
1	1	2024-06-29	4
2	1	2024-06-29	3.5
3	1	2024-06-28	8
4	2	2024-06-29	5
5	2	2024-06-29	2.5
6	2	2024-06-28	6.75
7	3	2024-06-30	6
8	3	2024-06-27	2
9	3	2024-06-27	7


 
#Uzdevums
Izveidot WEB aplikāciju (vēlams izmantot python), kas:
1.	Sākuma lapā (/) parāda sarakstu ar visiem darbinieku username
o	Iespēja veikt username meklēšanu
2.	Klikšķinot uz kāda darbinieka username, atveras lapa/skats, kur:
o	Redzama tabula ar divām kolonnām- date, hours_worked
o	Tabulā katrai dienai tiek summētas visas nostrādātās stundas šajā datumā (piemēram, ja vienā dienā ir divi ieraksti ar 4h un 3.5h — kopsumma būs 7.5)
o	Tabula sakārtota pēc date DESC
