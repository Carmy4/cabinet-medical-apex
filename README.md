# 🏥 PROIECT BD-P2: Cabinet Medical 

## 📖 Descrierea Proiectului
Acest repository conține implementarea mea pentru aplicația de gestiune a unui cabinet medical, dezvoltată în Oracle APEX. Proiectul a fost realizat în echipă (2 studenți), iar acest portofoliu evidențiază structura bazei de date și modulele interfeței grafice dezvoltate exclusiv de mine.

## 🗄️ Structura Bazei de Date (Proiectare Comună)
Aplicația funcționează pe o schemă relațională formată din următoarele tabele:
* **cbMedic**: Stochează detaliile medicilor (ID, nume, cod specialitate, cod grad).
* **cbProgramare**: Gestionează programările pacienților (cod, dată, CNP pacient, nume pacient, medic, cabinet).
* **cbReteta**: Conține detaliile prescripțiilor medicale (cod programare, număr item, medicament, doză zilnică, durata).
* **cbSpecialitate**: Definește specialitățile disponibile și coeficientul de plată.
* **cbGrad**: Nomenclatorul gradelor medicale și tariful de bază.

## ⚙️ Funcționalități APEX Implementate (Contribuție Proprie)
Pentru interfața aplicației, am fost responsabilă de dezvoltarea următoarelor module și rapoarte:
* **Vizualizare medici:** Raport detaliat cu toți medicii din baza de date.
* **Ierarhii Medic-Programare:** Pagină complexă pentru vizualizarea ierarhică a pacienților care s-au programat la un anumit medic.
* **Căutare parametrizată pacienți:** Pagină de vizualizare a programărilor unui pacient, filtrate dinamic pe baza CNP-ului introdus (utilizând parametri de tip `PageItem`).
* **Raportare Statistici Medici:** Raport de sinteză care afișează o listă cu: numele medicului, specialitatea, gradul și numărul total de programări pentru acesta.

## 📂 Fișierele Proiectului
* Scripturile SQL care cuprind instrucțiunile DDL (crearea tabelelor și a constrângerilor de integritate) și DML (inserarea datelor de test: 8 medici, 30 programări, 40 rețete).
* Exportul aplicației Oracle APEX conținând paginile și logica dezvoltată.
