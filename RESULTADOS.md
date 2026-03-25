# 📊 Análisis de Consultas SQL


## 📈 Resumen
✅ 10 correctas de 12 queries

## ✅ Query 1: Correcto

⏱ Tiempo: 0.49 ms
🔍 No se usó ningún índice en esta consulta.

---

## ✅ Query 2: Correcto

⏱ Tiempo: 0.28 ms
🔍 No se usó ningún índice en esta consulta.

---

## ✅ Query 3: Correcto

⏱ Tiempo: 0.30 ms
🔍 No se usó ningún índice en esta consulta.

---

## ✅ Query 4: Correcto

⏱ Tiempo: 0.30 ms
🔍 No se usó ningún índice en esta consulta.

---

## ✅ Query 5: Correcto

⏱ Tiempo: 0.32 ms
✅ Se usó índice(s) en la consulta: id_grado

---

## ✅ Query 6: Correcto

⏱ Tiempo: 0.43 ms
✅ Se usó índice(s) en la consulta: PRIMARY

---

## ✅ Query 7: Correcto

⏱ Tiempo: 0.52 ms
✅ Se usó índice(s) en la consulta: PRIMARY, PRIMARY,id_asignatura, PRIMARY,nif

---

## ✅ Query 8: Correcto

⏱ Tiempo: 0.43 ms
✅ Se usó índice(s) en la consulta: PRIMARY, id_profesor,id_grado, PRIMARY,id_departamento

---

## ✅ Query 9: Correcto

⏱ Tiempo: 0.37 ms
✅ Se usó índice(s) en la consulta: PRIMARY, PRIMARY,id_curso_escolar

---

## ✅ Query 10: Correcto

⏱ Tiempo: 0.45 ms
✅ Se usó índice(s) en la consulta: PRIMARY

---

## ❌ Query 11: Incorrecto
```diff
--- 
+++ 
@@ -1 +1,11 @@
 apellido1 | apellido2 | nombre
+Ramirez | Gea | Zoe
+Hamill | Kozey | Manolo
+Lemke | Rutherford | Cristina
+Fahey | Considine | Antonio
+Spencer | Lakin | Esther
+Streich | Hirthe | Carmen
+Ruecker | Upton | Guillermo
+Monahan | Murray | Micaela
+Stiedemann | Morissette | Alfredo
+Schowalter | Muller | Francesca
```

⏱ Tiempo: 0.36 ms
✅ Se usó índice(s) en la consulta: PRIMARY, PRIMARY,id_departamento

---

## ❌ Query 12: Error
- **Descripción**: 'NoneType' object is not iterable

