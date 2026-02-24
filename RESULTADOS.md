# 📊 Análisis de Consultas SQL


## 📈 Resumen
✅ 15 correctas de 25 queries

## ❌ Query 1: Incorrecto
```diff
--- 
+++ 
@@ -1,13 +1,13 @@
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
+Daniel | Herman | Pacocha
+Inma | Lakin | Yundt
+Irene | Hernández | Martínez
+Ismael | Strosin | Turcotte
+José | Koss | Bayer
+Juan | Gutiérrez | López
+Juan | Saez | Vega
+Pedro | Heller | Pagac
+Ramón | Herzog | Tremblay
+Salvador | Sánchez | Pérez
+Sonia | Gea | Ruiz
```

⏱ Tiempo: 0.38 ms
🔍 No se usó ningún índice en esta consulta.

---

## ✅ Query 2: Correcto

⏱ Tiempo: 0.30 ms
🔍 No se usó ningún índice en esta consulta.

---

## ✅ Query 3: Correcto

⏱ Tiempo: 0.31 ms
🔍 No se usó ningún índice en esta consulta.

---

## ✅ Query 4: Correcto

⏱ Tiempo: 0.33 ms
🔍 No se usó ningún índice en esta consulta.

---

## ✅ Query 5: Correcto

⏱ Tiempo: 0.32 ms
✅ Se usó índice(s) en la consulta: id_grado

---

## ✅ Query 6: Correcto

⏱ Tiempo: 0.38 ms
✅ Se usó índice(s) en la consulta: PRIMARY, PRIMARY,id_departamento

---

## ❌ Query 7: Incorrecto
```diff
--- 
+++ 
@@ -1,4 +1,4 @@
-nombre | anyo_inicio | anyo_fin
+nombre | año de inicio | año de fin
 Álgegra lineal y matemática discreta | 2014.00 | 2015.00
 Cálculo | 2014.00 | 2015.00
 Física para informática | 2014.00 | 2015.00
```

⏱ Tiempo: 0.54 ms
✅ Se usó índice(s) en la consulta: PRIMARY, PRIMARY,nif, PRIMARY,id_asignatura,id_curso_escolar

---

## ✅ Query 8: Correcto

⏱ Tiempo: 0.42 ms
✅ Se usó índice(s) en la consulta: PRIMARY, id_profesor,id_grado, PRIMARY,id_departamento

---

## ✅ Query 9: Correcto

⏱ Tiempo: 0.37 ms
✅ Se usó índice(s) en la consulta: PRIMARY, PRIMARY,id_curso_escolar

---

## ✅ Query 10: Correcto

⏱ Tiempo: 0.41 ms
✅ Se usó índice(s) en la consulta: PRIMARY

---

## ✅ Query 11: Correcto

⏱ Tiempo: 0.34 ms
✅ Se usó índice(s) en la consulta: PRIMARY

---

## ❌ Query 12: Error
- **Descripción**: 1054 (42S22): Unknown column 'prpfesor.id_departamento' in 'on clause'


## ✅ Query 13: Correcto

⏱ Tiempo: 0.34 ms
✅ Se usó índice(s) en la consulta: PRIMARY, id_profesor

---

## ✅ Query 14: Correcto

⏱ Tiempo: 0.30 ms
✅ Se usó índice(s) en la consulta: id_profesor

---

## ❌ Query 15: Incorrecto
```diff
--- 
+++ 
@@ -1,9 +1,13 @@
 nombre
-Informática
+Matemáticas
 Matemáticas
 Economía y Empresa
+Economía y Empresa
+Educación
+Educación
 Educación
 Agronomía
+Química y Física
 Química y Física
 Filología
 Derecho
```

⏱ Tiempo: 0.35 ms
✅ Se usó índice(s) en la consulta: id_departamento, id_profesor

---

## ✅ Query 16: Correcto

⏱ Tiempo: 0.29 ms
🔍 No se usó ningún índice en esta consulta.

---

## ✅ Query 17: Correcto

⏱ Tiempo: 0.30 ms
🔍 No se usó ningún índice en esta consulta.

---

## ✅ Query 18: Correcto

⏱ Tiempo: 0.36 ms
✅ Se usó índice(s) en la consulta: id_departamento, PRIMARY

---

## ❌ Query 19: Incorrecto
```diff
--- 
+++ 
@@ -1,10 +1,10 @@
 departamento | total
+Agronomía | 1.00
+Biología y Geología | 0.00
+Derecho | 0.00
+Economía y Empresa | 2.00
+Educación | 3.00
+Filología | 0.00
 Informática | 2.00
 Matemáticas | 2.00
-Economía y Empresa | 2.00
-Educación | 3.00
-Agronomía | 1.00
 Química y Física | 2.00
-Filología | 0.00
-Derecho | 0.00
-Biología y Geología | 0.00
```

⏱ Tiempo: 0.37 ms
✅ Se usó índice(s) en la consulta: id_departamento

---

## ❌ Query 20: Incorrecto
```diff
--- 
+++ 
@@ -1,4 +1,4 @@
-grau | total
+grado | total
 Grado en Ingeniería Informática (Plan 2015) | 51.00
 Grado en Biotecnología (Plan 2015) | 32.00
 Grado en Ingeniería Agrícola (Plan 2015) | 0.00
```

⏱ Tiempo: 0.36 ms
✅ Se usó índice(s) en la consulta: id_grado

---

## ❌ Query 21: Incorrecto
```diff
--- 
+++ 
@@ -1,2 +1,2 @@
-grau | total
+grado | total
 Grado en Ingeniería Informática (Plan 2015) | 51.00
```

⏱ Tiempo: 0.33 ms
✅ Se usó índice(s) en la consulta: id_grado

---

## ❌ Query 22: Incorrecto
```diff
--- 
+++ 
@@ -1,6 +1,6 @@
-grau | tipo | total_creditos
+grado | tipos | total_creditos
+Grado en Biotecnología (Plan 2015) | básica | 60.00
+Grado en Biotecnología (Plan 2015) | obligatoria | 120.00
 Grado en Ingeniería Informática (Plan 2015) | básica | 72.00
 Grado en Ingeniería Informática (Plan 2015) | obligatoria | 54.00
 Grado en Ingeniería Informática (Plan 2015) | optativa | 180.00
-Grado en Biotecnología (Plan 2015) | básica | 60.00
-Grado en Biotecnología (Plan 2015) | obligatoria | 120.00
```

⏱ Tiempo: 0.34 ms
✅ Se usó índice(s) en la consulta: PRIMARY, id_grado

---

## ❌ Query 23: Incorrecto
```diff
--- 
+++ 
@@ -1,3 +1,6 @@
 anyo_inicio | total
 2014.00 | 3.00
+2015.00 | 0.00
+2016.00 | 0.00
+2017.00 | 0.00
 2018.00 | 3.00
```

⏱ Tiempo: 0.36 ms
✅ Se usó índice(s) en la consulta: id_curso_escolar

---

## ✅ Query 24: Correcto

⏱ Tiempo: 0.37 ms
✅ Se usó índice(s) en la consulta: PRIMARY, id_profesor

---

## ❌ Query 25: Error
- **Descripción**: 'NoneType' object is not iterable

