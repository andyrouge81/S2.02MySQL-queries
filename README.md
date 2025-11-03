# S2.02MySQL-queries

## 📋 Description

This project focuses on practicing **SQL querying and data manipulation** two relational database model **tienda** and **universidad**.
The goal of the exercise is to apply different **SQL selection, filtering, and formatting techniques** to retrieve and present information from the database in various ways.  
This exercise helps reinforce key concepts of **data retrieval and presentation in SQL**, providing hands-on experience with **basic query operations** in a relational database environment.

The repository includes:

- SQL scripts with all required queries for each exercise.
- Schemas defining the relational structure of the *Tienda* and *Universidad* databases.

---

## 📚 Objectives

- Strengthen practical skills in **SQL querying** and **data manipulation**.  
- Practice using **SELECT**, **WHERE**, **ORDER BY**, **LIMIT**, **JOIN**, and other SQL clauses.  
- Understand how to extract and format information from relational data structures.  
- Work with real-world database examples (commercial and academic contexts).  
- Demonstrate the ability to organize SQL exercises in a clean and well-documented format.  

---

## 🧾 Proposed Exercises

## Tienda
<details>
 Base de dades Tienda

Tenim les taules producto i fabricador, cadascuna amb els següents camps:
- producto (codigo, nombre, precio, codigo_fabricante)
- fabricante (codigo, nombre)
El camp 'codigo_fabricante' de l'entitat producto es relaciona amb el camp 'codi' de l'entitat fabricante.
Si us plau, efectua les següents consultes:

- Llista el nom de tots els productes que hi ha en la taula producto.
- Llista els noms i els preus de tots els productes de la taula producto.
- Llista totes les columnes de la taula producto.
- Llista el nom dels productes, el preu en euros i el preu en dòlars estatunidencs (USD).
- Llista el nom dels productes, el preu en euros i el preu en dòlars estatunidencs (USD). Utilitza els següents àlies per a les columnes: nom de producto, euros, dòlars.
- Llista els noms i els preus de tots els productes de la taula producto, convertint els noms a majúscula.
- Llista els noms i els preus de tots els productes de la taula producto, convertint els noms a minúscula.
- Llista el nom de tots els fabricants en una columna, i en una altra columna obtingui en majúscules els dos primers caràcters del nom del fabricant.
- Llista els noms i els preus de tots els productes de la taula producto, arrodonint el valor del preu.
- Llista els noms i els preus de tots els productes de la taula producto, truncant el valor del preu per a mostrar-lo sense cap xifra decimal.
- Llista el codi dels fabricants que tenen productes en la taula producto.
- Llista el codi dels fabricants que tenen productes en la taula producto, eliminant els codis que apareixen repetits.
- Llista els noms dels fabricants ordenats de manera ascendent.
- Llista els noms dels fabricants ordenats de manera descendent.
- Llista els noms dels productes ordenats, en primer lloc, pel nom de manera ascendent i, en segon lloc, pel preu de manera descendent.
- Retorna una llista amb les 5 primeres files de la taula fabricante.
- Retorna una llista amb 2 files a partir de la quarta fila de la taula fabricante. La quarta fila també s'ha d'incloure en la resposta.
- Llista el nom i el preu del producte més barat. (Utilitza solament les clàusules ORDER BY i LIMIT). NOTA: Aquí no podria usar MIN(preu), necessitaria GROUP BY.
- Llista el nom i el preu del producte més car. (Utilitza solament les clàusules ORDER BY i LIMIT). NOTA: Aquí no podria usar MAX(preu), necessitaria GROUP BY.
- Llista el nom de tots els productes del fabricant el codi de fabricant del qual és igual a 2.
- Retorna una llista amb el nom del producte, preu i nom de fabricant de tots els productes de la base de dades.
- Retorna una llista amb el nom del producte, preu i nom de fabricant de tots els productes de la base de dades. Ordena el resultat pel nom del fabricant, per ordre alfabètic.
- Retorna una llista amb el codi del producte, nom del producte, codi del fabricador i nom del fabricador, de tots els productes de la base de dades.
- Retorna el nom del producte, el seu preu i el nom del seu fabricant, del producte més barat.
- Retorna el nom del producte, el seu preu i el nom del seu fabricant, del producte més car.
- Retorna una llista de tots els productes del fabricant Lenovo.
- Retorna una llista de tots els productes del fabricant Crucial que tinguin un preu major que 200 €.
- Retorna un llistat amb tots els productes dels fabricants Asus, Hewlett-Packardy Seagate. Sense utilitzar l'operador IN.
- Retorna un llistat amb tots els productes dels fabricants Asus, Hewlett-Packardy Seagate. Fent servir l'operador IN.
- Retorna un llistat amb el nom i el preu de tots els productes dels fabricants el nom dels quals acabi per la vocal e.
- Retorna un llistat amb el nom i el preu de tots els productes el nom de fabricant dels quals contingui el caràcter w en el seu nom.
- Retorna un llistat amb el nom de producte, preu i nom de fabricant, de tots els productes que tinguin un preu major o igual a 180 €. Ordena el resultat, en primer lloc, pel preu (en ordre descendent) i, en segon lloc, pel nom (en ordre ascendent).
- Retorna un llistat amb el codi i el nom de fabricant, solament d'aquells fabricants que tenen productes associats en la base de dades.
- Retorna un llistat de tots els fabricants que existeixen en la base de dades, juntament amb els productes que té cadascun d'ells. El llistat haurà de mostrar també aquells fabricants que no tenen productes associats.
- Retorna un llistat on només apareguin aquells fabricants que no tenen cap producte associat.
- Retorna tots els productes del fabricador Lenovo. (Sense utilitzar INNER JOIN).
- Retorna totes les dades dels productes que tenen el mateix preu que el producte més car del fabricant Lenovo. (Sense usar INNER JOIN).
- Llista el nom del producte més car del fabricant Lenovo.
- Llista el nom del producte més barat del fabricant Hewlett-Packard.
- Retorna tots els productes de la base de dades que tenen un preu major o igual al producte més car del fabricant Lenovo.
- Llesta tots els productes del fabricant Asus que tenen un preu superior al preu mitjà de tots els seus productes.

</details>

## Universidad

<details>

Base de dades Universidad

Si us plau, descàrrega la base de dades del fitxer schema_universidad.sql, visualitza el diagrama E-R en un editor i efectua les següents consultes:

- Retorna un llistat amb el primer cognom, segon cognom i el nom de tots els/les alumnes. El llistat haurà d'estar ordenat alfabèticament de menor a major pel primer cognom, segon cognom i nom.
- Esbrina el nom i els dos cognoms dels alumnes que no han donat d'alta el seu número de telèfon en la base de dades.
- Retorna el llistat dels alumnes que van néixer en 1999.
- Retorna el llistat de professors/es que no han donat d'alta el seu número de telèfon en la base de dades i a més el seu NIF acaba en K.
- Retorna el llistat de les assignatures que s'imparteixen en el primer quadrimestre, en el tercer curs del grau que té l'identificador 7.
- Retorna un llistat dels professors/es juntament amb el nom del departament al qual estan vinculats. El llistat ha de retornar quatre columnes, primer cognom, segon cognom, nom i nom del departament. El resultat estarà ordenat alfabèticament de menor a major pels cognoms i el nom.
- Retorna un llistat amb el nom de les assignatures, any d'inici i any de fi del curs escolar de l'alumne/a amb NIF 26902806M.
- Retorna un llistat amb el nom de tots els departaments que tenen professors/es que imparteixen alguna assignatura en el Grau en Enginyeria Informàtica (Pla 2015).
- Retorna un llistat amb tots els alumnes que s'han matriculat en alguna assignatura durant el curs escolar 2018/2019.
- Resol les 6 següents consultes utilitzant les clàusules LEFT JOIN i RIGHT JOIN.
 
- Retorna un llistat amb els noms de tots els professors/es i els departaments que tenen vinculats. El llistat també ha de mostrar aquells professors/es que no tenen cap departament associat. El llistat ha de retornar quatre columnes, nom del departament, primer cognom, segon cognom i nom del professor/a. El resultat estarà ordenat alfabèticament de menor a major pel nom del departament, cognoms i el nom.
- Retorna un llistat amb els professors/es que no estan associats a un departament.
- Retorna un llistat amb els departaments que no tenen professors/es associats.
- Retorna un llistat amb els professors/es que no imparteixen cap assignatura.
- Retorna un llistat amb les assignatures que no tenen un professor/a assignat.
- Retorna un llistat amb tots els departaments que no han impartit assignatures en cap curs escolar.

Consultes resum:

- Retorna el nombre total d'alumnes que hi ha.
- Calcula quants alumnes van néixer en 1999.
- Calcula quants professors/es hi ha en cada departament. El resultat només ha de mostrar dues columnes, una amb el nom del departament i una altra amb el nombre de professors/es que hi ha en aquest departament. El resultat només ha d'incloure els departaments que tenen professors/es associats i haurà d'estar ordenat de major a menor pel nombre de professors/es.
- Retorna un llistat amb tots els departaments i el nombre de professors/es que hi ha en cadascun d'ells. Tingui en compte que poden existir departaments que no tenen professors/es associats. Aquests departaments també han d'aparèixer en el llistat.
- Retorna un llistat amb el nom de tots els graus existents en la base de dades i el nombre d'assignatures que té cadascun. Tingues en compte que poden existir graus que no tenen assignatures associades. Aquests graus també han d'aparèixer en el llistat. El resultat haurà d'estar ordenat de major a menor pel nombre d'assignatures.
- Retorna un llistat amb el nom de tots els graus existents en la base de dades i el nombre d'assignatures que té cadascun, dels graus que tinguin més de 40 assignatures associades.
- Retorna un llistat que mostri el nom dels graus i la suma del nombre total de crèdits que hi ha per a cada tipus d'assignatura. El resultat ha de tenir tres columnes: nom del grau, tipus d'assignatura i la suma dels crèdits de totes les assignatures que hi ha d'aquest tipus.

</details>

---

## 🧰 Technologies Used

- **MySQL Server 8.0+**  
- **MySQL Workbench** for query execution and schema visualization  
- SQL (EER diagram)  

---

## ⚙️ Requirements

Before running the project, make sure you have:
- MySQL Server installed and running  
- MySQL Workbench or another compatible SQL client  
- Basic understanding of SQL commands and relational concepts  

---

## 🪛 Installation

1. Clone or download** this repository:
   ```bash
   git clone https://github.com/andyrouge81/S2.02MySQL-queries.git
   cd S2.02MySQL-queries

2. Open MySQL Workbench and connect to your local MySQL server.
3. Load the provided SQL scripts:
  - For the Tienda database: tienda_queries.sql
  - For the Universidad database: universidad_queries.sql

4. Execute each script using the ⚡️ Run button in MySQL Workbench.
  - Each query is written on a single line as required.
    
---

## ▶️ Execution

1. Start the MySQL Server on your local machine.
2. Make sure the service is active before opening Workbench.
3. Open MySQL Workbench and connect to your MySQL instance.
4. Load and execute the .sql files included in the repository:

   ```bash
     pathDirectory/tienda_queries.sql;
    pathDirectory/universidad_queries.sql;

5. Verify that all queries run successfully and return the expected results.

---

##  🤝 Contributions

If you'd like to collaborate:

1. Fork the repository
   
3. Create a new branch:
    ```bash 
   feature/new-sql-query

4. Commit your changes

    ```bash
    git commit -m "feat: the query does not run"
   
5. Submit a Pull Request
    ```bash
    git push origin feature/myQuerySolution

---

💌 Contact

For questions or feedback, feel free to open an Issue or reach out via [GitHub Profile](https://github.com/andyrouge81)
