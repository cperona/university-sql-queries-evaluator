# 📊 Análisis de Consultas SQL


## 📈 Resumen
✅ 14 correctas de 18 queries

## ✅ Query 1: Correcto

⏱ Tiempo: 0.44 ms
🔍 No se usó ningún índice en esta consulta.

---

## ✅ Query 2: Correcto

⏱ Tiempo: 0.32 ms
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

## ✅ Query 5: Correcto

⏱ Tiempo: 0.36 ms
✅ Se usó índice(s) en la consulta: id_grado

---

## ✅ Query 6: Correcto

⏱ Tiempo: 0.43 ms
✅ Se usó índice(s) en la consulta: PRIMARY

---

## ✅ Query 7: Correcto

⏱ Tiempo: 0.43 ms
✅ Se usó índice(s) en la consulta: PRIMARY,id_asignatura, PRIMARY,nif, PRIMARY

---

## ✅ Query 8: Correcto

⏱ Tiempo: 0.45 ms
✅ Se usó índice(s) en la consulta: PRIMARY,id_departamento, id_profesor,id_grado, PRIMARY

---

## ✅ Query 9: Correcto

⏱ Tiempo: 0.35 ms
✅ Se usó índice(s) en la consulta: PRIMARY,id_curso_escolar, PRIMARY

---

## ✅ Query 10: Correcto

⏱ Tiempo: 0.45 ms
✅ Se usó índice(s) en la consulta: PRIMARY

---

## ✅ Query 11: Correcto

⏱ Tiempo: 0.31 ms
🔍 No se usó ningún índice en esta consulta.

🚨 **Problemas detectados:**
🚨 `JOIN` sin índice. Revisar claves foráneas e índices.

---

## ✅ Query 12: Correcto

⏱ Tiempo: 0.31 ms
✅ Se usó índice(s) en la consulta: id_departamento

---

## ✅ Query 13: Correcto

⏱ Tiempo: 0.35 ms
✅ Se usó índice(s) en la consulta: id_profesor, PRIMARY

---

## ✅ Query 14: Correcto

⏱ Tiempo: 0.33 ms
✅ Se usó índice(s) en la consulta: id_profesor

---

## ❌ Query 15: Incorrecto
```diff
--- 
+++ 
@@ -1,10 +1,2 @@
-nombre
-Informática
-Matemáticas
-Economía y Empresa
-Educación
-Agronomía
-Química y Física
-Filología
-Derecho
-Biología y Geología
+total
+12.00
```

⏱ Tiempo: 0.33 ms
🔍 No se usó ningún índice en esta consulta.

---

## ❌ Query 16: Incorrecto
```diff
--- 
+++ 
@@ -1,2 +1,2 @@
-total
-12.00
+count(*)
+2.00
```

⏱ Tiempo: 0.30 ms
🔍 No se usó ningún índice en esta consulta.

---

## ❌ Query 17: Incorrecto
```diff
--- 
+++ 
@@ -1,2 +1,10 @@
-total
-2.00
+departamento | total
+Informática | 2.00
+Matemáticas | 2.00
+Economía y Empresa | 2.00
+Educación | 3.00
+Agronomía | 1.00
+Química y Física | 2.00
+Filología | 0.00
+Derecho | 0.00
+Biología y Geología | 0.00
```

⏱ Tiempo: 0.34 ms
✅ Se usó índice(s) en la consulta: id_departamento

---

## ❌ Query 18: Error
- **Descripción**: 1064 (42000): You have an error in your SQL syntax; check the manual that corresponds to your MySQL server version for the right syntax to use near '' at line 22

