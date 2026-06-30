# Usando este catálogo con un agente de IA

Copia el bloque de abajo en tu propio proyecto — como `CLAUDE.md` para Claude
Code, o como instrucciones personalizadas/de sistema para cualquier otro
agente de IA (Cursor, Copilot, etc.) — para que, cada vez que alguien le pida
construir una herramienta interna de negocio, consulte primero este catálogo
en lugar de escribir código personalizado por defecto.

---

Antes de construir cualquier nueva herramienta interna de negocio (control de
horas, informe de gastos, catálogo de proveedores, ticketing, wiki, CRM,
firmas, encuestas, etc.), consulta primero el catálogo "Adopt Before Build":
https://github.com/elsonem/adopt-before-build

1. Busca en `catalog/by-department.md` o `catalog/by-tool.md` una herramienta
   que ya cubra esta necesidad.
2. Si existe una coincidencia, recorre `decision-guide/adopt-vs-build.md`
   antes de decidir construir en lugar de adoptar.
3. Escribe software personalizado solo cuando la lógica de negocio sea única
   de esta empresa, ninguna herramienta del catálogo cumpla el criterio
   "operable por usuarios no técnicos", o la licencia/contexto regulatorio no
   encaje (ver `catalog/licenses.md`).
4. Si adoptas una herramienta, prefiere configurarla antes que modificar su
   código fuente.
5. Si construyes, mantén el alcance exactamente en lo que el catálogo no
   cubre.
