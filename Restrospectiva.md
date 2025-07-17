#  Retrospectiva Individual - Sprint Final

##  1. Prácticas, herramientas o técnicas que funcionaron bien
- Usamos GitFlow para estructurar el proyecto con ramas `feature/`, `develop` y `release`, lo que permitió mantener un flujo ordenado.
- Hicimos Pull Requests con revisión entre compañeras/os, lo que ayudó a validar cambios antes de mezclar código.
- Registramos avances, problemas y decisiones directamente en GitHub con comentarios claros.

**Elemento de configuración asociado:** documentación de mantenimiento, diseño y pruebas.

---

##  2. Prácticas que podrían mejorar
- No consideramos desde el inicio la exclusión de archivos de compilación como `.dll`, `.exe` y carpetas `bin/`, `obj/`, lo que causó conflictos en los PR.
- A veces trabajamos directamente en `develop` o no actualizamos las ramas locales antes de subir cambios.
- Hubo confusión al momento de resolver conflictos, por falta de experiencia con merges.

**Elemento de configuración asociado:** software ejecutable, listados, especificación del software.

---

##  3. ¿Qué se debería dejar de hacer?
- Subir archivos generados automáticamente por el sistema (compilaciones).
- Hacer merges o commits sin revisar correctamente el estado de la rama remota y sin resolver conflictos localmente.

**Elemento de configuración asociado:** datos de prueba y prueba validada, documentación provisional.

---

##  4. ¿Qué deberíamos estar haciendo (pero no hicimos)?
- Crear un archivo `.gitignore` al comienzo del proyecto para evitar que se suban archivos innecesarios.
- Automatizar validaciones con GitHub Actions o Codacy desde el inicio.
- Hacer una revisión semanal de ramas activas y Pull Requests para evitar acumulación de tareas en último momento.

**Elemento de configuración asociado:** documentación de planificación, configuración del entorno.

---

## 😊😢😠 Mad / Sad / Glad

- **Glad:** Nos gustó aprender a usar bien GitHub, trabajar en equipo con ramas y revisiones, y ver cómo se puede mejorar el código en colaboración.
- **Sad:** Nos sentimos abrumados cuando aparecieron errores por archivos no ignorados y no sabía cómo resolverlos.
- **Mad:** Nos enojamos cuando tuvimos  que repetir el proceso varias veces por no planificar bien los merges ni configurar `.gitignore`.
- **Sad:** Nos sentimos abrumados cuando no entendiamos como funcionaba github.

---

## 5 Whys - Análisis de causa raíz

**Problema:** Se subieron archivos compilados y hubo conflictos que interrumpieron el flujo de trabajo.

1. **¿Por qué ocurrió esto?** → Porque se subieron archivos de compilación (`bin/`, `obj/`, `.dll`).
2. **¿Por qué se subieron esos archivos?** → Porque no estaban en el archivo `.gitignore`.
3. **¿Por qué no se configuró `.gitignore` al principio?** → Porque no sabíamos su importancia o se nos olvidó.
4. **¿Por qué no sabíamos eso?** → Porque no revisamos buenas prácticas al iniciar el proyecto.
5. **¿Por qué no aplicamos buenas prácticas?** → Porque comenzamos a trabajar de inmediato sin definir reglas de configuración inicial.

**Conclusión:** El problema raíz fue la falta de una configuración inicial clara del repositorio y la ausencia de un `.gitignore` adecuado y que no conociamos
bien como funcionaba github.

---
