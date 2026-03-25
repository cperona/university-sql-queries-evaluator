# 📊 Análisis de Consultas SQL


## 📈 Resumen
✅ 6 correctas de 9 queries

## ❌ Query 1: Incorrecto
```diff
--- 
+++ 
@@ -1,13 +1,25 @@
 apellido1 | apellido2 | nombre
 Domínguez | Guerrero | Antonio
+Fahey | Considine | Antonio
 Gea | Ruiz | Sonia
 Gutiérrez | López | Juan
+Hamill | Kozey | Manolo
 Heller | Pagac | Pedro
 Herman | Pacocha | Daniel
 Hernández | Martínez | Irene
 Herzog | Tremblay | Ramón
+Kohler | Schoen | Alejandro
 Koss | Bayer | José
 Lakin | Yundt | Inma
+Lemke | Rutherford | Cristina
+Monahan | Murray | Micaela
+Ramirez | Gea | Zoe
+Ruecker | Upton | Guillermo
 Saez | Vega | Juan
 Sánchez | Pérez | Salvador
+Schmidt | Fisher | David
+Schowalter | Muller | Francesca
+Spencer | Lakin | Esther
+Stiedemann | Morissette | Alfredo
+Streich | Hirthe | Carmen
 Strosin | Turcotte | Ismael
```

⏱ Tiempo: 0.38 ms
🔍 No se usó ningún índice en esta consulta.

---

## ✅ Query 2: Correcto

⏱ Tiempo: 0.33 ms
🔍 No se usó ningún índice en esta consulta.

---

## ✅ Query 3: Correcto

⏱ Tiempo: 0.32 ms
🔍 No se usó ningún índice en esta consulta.

---

## ✅ Query 4: Correcto

⏱ Tiempo: 0.31 ms
🔍 No se usó ningún índice en esta consulta.

---

## ❌ Query 5: Incorrecto
```diff
--- 
+++ 
@@ -1,4 +1,14 @@
 id | nombre | cuatrimestre | curso | id_grado
+52.00 | Biologia celular | 1.00 | 1.00 | 7.00
+53.00 | Física | 1.00 | 1.00 | 7.00
+54.00 | Matemáticas I | 1.00 | 1.00 | 7.00
+55.00 | Química general | 1.00 | 1.00 | 7.00
+56.00 | Química orgánica | 1.00 | 1.00 | 7.00
+62.00 | Botánica agrícola | 1.00 | 2.00 | 7.00
+63.00 | Fisiología vegetal | 1.00 | 2.00 | 7.00
+64.00 | Genética molecular | 1.00 | 2.00 | 7.00
+65.00 | Ingeniería bioquímica | 1.00 | 2.00 | 7.00
+66.00 | Termodinámica y cinética química aplicada | 1.00 | 2.00 | 7.00
 72.00 | Bases moleculares del desarrollo vegetal | 1.00 | 3.00 | 7.00
 73.00 | Fisiología animal | 1.00 | 3.00 | 7.00
 74.00 | Metabolismo y biosíntesis de biomoléculas | 1.00 | 3.00 | 7.00
```

⏱ Tiempo: 0.33 ms
✅ Se usó índice(s) en la consulta: id_grado

---

## ✅ Query 6: Correcto

⏱ Tiempo: 0.41 ms
✅ Se usó índice(s) en la consulta: PRIMARY

---

## ✅ Query 7: Correcto

⏱ Tiempo: 0.41 ms
✅ Se usó índice(s) en la consulta: PRIMARY, PRIMARY,id_asignatura, PRIMARY,nif

---

## ✅ Query 8: Correcto

⏱ Tiempo: 0.39 ms
✅ Se usó índice(s) en la consulta: PRIMARY, PRIMARY,id_departamento, id_profesor,id_grado

---

## ❌ Query 9: Error
- **Descripción**: 'NoneType' object is not iterable

