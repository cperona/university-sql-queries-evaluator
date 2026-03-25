# 📊 Análisis de Consultas SQL


## 📈 Resumen
✅ 4 correctas de 9 queries

## ❌ Query 1: Incorrecto
```diff
--- 
+++ 
@@ -1,13 +1,25 @@
-apellido1 | apellido2 | nombre
-Domínguez | Guerrero | Antonio
-Gea | Ruiz | Sonia
-Gutiérrez | López | Juan
-Heller | Pagac | Pedro
-Herman | Pacocha | Daniel
-Hernández | Martínez | Irene
-Herzog | Tremblay | Ramón
-Koss | Bayer | José
-Lakin | Yundt | Inma
-Saez | Vega | Juan
-Sánchez | Pérez | Salvador
-Strosin | Turcotte | Ismael
+nombre | apellido1 | apellido2
+Antonio | Domínguez | Guerrero
+Antonio | Fahey | Considine
+Sonia | Gea | Ruiz
+Juan | Gutiérrez | López
+Manolo | Hamill | Kozey
+Pedro | Heller | Pagac
+Daniel | Herman | Pacocha
+Irene | Hernández | Martínez
+Ramón | Herzog | Tremblay
+Alejandro | Kohler | Schoen
+José | Koss | Bayer
+Inma | Lakin | Yundt
+Cristina | Lemke | Rutherford
+Micaela | Monahan | Murray
+Zoe | Ramirez | Gea
+Guillermo | Ruecker | Upton
+Juan | Saez | Vega
+Salvador | Sánchez | Pérez
+David | Schmidt | Fisher
+Francesca | Schowalter | Muller
+Esther | Spencer | Lakin
+Alfredo | Stiedemann | Morissette
+Carmen | Streich | Hirthe
+Ismael | Strosin | Turcotte
```

⏱ Tiempo: 0.37 ms
🔍 No se usó ningún índice en esta consulta.

---

## ❌ Query 2: Incorrecto
```diff
--- 
+++ 
@@ -1,3 +1,8 @@
 nombre | apellido1 | apellido2
 Pedro | Heller | Pagac
 Ismael | Strosin | Turcotte
+Esther | Spencer | Lakin
+Carmen | Streich | Hirthe
+Antonio | Fahey | Considine
+Guillermo | Ruecker | Upton
+Francesca | Schowalter | Muller
```

⏱ Tiempo: 0.32 ms
🔍 No se usó ningún índice en esta consulta.

---

## ❌ Query 3: Incorrecto
```diff
--- 
+++ 
@@ -1,3 +1,3 @@
-id | nombre | apellido1 | apellido2 | fecha_nacimiento
-7.00 | Ismael | Strosin | Turcotte | 1999-05-24
-22.00 | Antonio | Domínguez | Guerrero | 1999-02-11
+id | nif | nombre | apellido1 | apellido2 | ciudad | direccion | telefono | fecha_nacimiento | sexo | tipo
+7.00 | 97258166K | Ismael | Strosin | Turcotte | Almería | C/ Neptuno | NULL | 1999-05-24 | H | alumno
+22.00 | 41491230N | Antonio | Domínguez | Guerrero | Almería | C/ Cabo de Gata | 626652498 | 1999-02-11 | H | alumno
```

⏱ Tiempo: 0.35 ms
🔍 No se usó ningún índice en esta consulta.

🚨 **Problemas detectados:**
⚠️ Evitar `SELECT *`. Usar solo las columnas necesarias.

---

## ✅ Query 4: Correcto

⏱ Tiempo: 0.33 ms
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

⏱ Tiempo: 0.34 ms
✅ Se usó índice(s) en la consulta: id_grado

---

## ✅ Query 6: Correcto

⏱ Tiempo: 0.41 ms
✅ Se usó índice(s) en la consulta: PRIMARY

---

## ✅ Query 7: Correcto

⏱ Tiempo: 0.40 ms
✅ Se usó índice(s) en la consulta: PRIMARY, PRIMARY,id_asignatura, PRIMARY,nif

---

## ✅ Query 8: Correcto

⏱ Tiempo: 0.39 ms
✅ Se usó índice(s) en la consulta: id_profesor,id_grado, PRIMARY,id_departamento, PRIMARY

---

## ❌ Query 9: Error
- **Descripción**: 'NoneType' object is not iterable

