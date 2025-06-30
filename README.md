# Darbinieku darba laiku atskaite no SQLite datubāzes

## Resursi

Tev tiek dots **SQLite datubāzes fails**: `attendance.db`  
Šajā datubāzē ir divas tabulas:

### Tabulu struktūra

**`Employees`**

| id | username |
|:----|:-----------|
| 1  | janis       |
| 2  | liga        |
| 3  | juris       |
| 4  | dace        |

**`Attendance`**

| id | employee_id | date       | hours_worked |
|:----|:-------------|:-------------|:----------------|
| 1  | 1               | 2024-06-29 | 4               |
| 2  | 1               | 2024-06-29 | 3.5             |
| 3  | 1               | 2024-06-28 | 8               |
| 4  | 2               | 2024-06-29 | 5               |
| 5  | 2               | 2024-06-29 | 2.5             |
| 6  | 2               | 2024-06-28 | 6.75            |
| 7  | 3               | 2024-06-30 | 6               |
| 8  | 3               | 2024-06-27 | 2               |
| 9  | 3               | 2024-06-27 | 7               |

---

## 📌 Uzdevums

Izveidot **WEB aplikāciju** (vēlams izmantot Python):

### 📍 Sākuma lapa `/`
- Parāda sarakstu ar visiem darbinieku `username`
- Iespēja veikt **username meklēšanu**

---

### 📍 Darbinieka skatījums 
- Klikšķinot uz kāda darbinieka username, atveras lapa/skats, kur:
  - Redzama **tabula ar divām kolonnām: `date`, `hours_worked`**
  - Tabulā katrai dienai **tiek summētas visas nostrādātās stundas šajā datumā**
    - 📌 *Piemērs*:  
      Ja vienā dienā ir divi ieraksti ar 4h un 3.5h — kopsumma būs **7.5**
  - Tabula **sakārtota pēc `date` DESC**

---


