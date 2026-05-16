<!-- ⚠️ LEER ANTES DE ENVIAR
  Todo PR debe estar vinculado a un issue que tenga la etiqueta "status:approved".
  Los PRs sin un issue vinculado y aprobado serán rechazados automáticamente por CI.
  Consultá CONTRIBUTING.md para ver el flujo completo de contribución.
-->

## 🔗 Issue vinculado

Closes #

<!-- Reemplazá el # de arriba por el número del issue, por ejemplo: Closes #42 -->

---

## 🏷️ Tipo de PR

¿Qué tipo de cambio introduce este PR?

- [ ] `type:bug` — Corrección de bug (cambio no disruptivo que corrige un issue)
- [ ] `type:feature` — Nueva funcionalidad (cambio no disruptivo que agrega funcionalidad)
- [ ] `type:docs` — Solo documentación
- [ ] `type:refactor` — Refactorización de código (sin cambios funcionales)
- [ ] `type:chore` — Cambios de build, CI o tooling
- [ ] `type:breaking-change` — Cambio disruptivo (fix o feature que cambia comportamiento existente)

---

## 📝 Resumen

<!-- Describí de forma clara y concisa qué hace este PR y por qué. -->

---

## 📂 Cambios

| Archivo / área | Qué cambió        |
| -------------- | ----------------- |
| `path/to/file` | Descripción breve |

---

## 🧪 Plan de pruebas

**Tests unitarios**

```bash
go test ./...
```

**Tests E2E** (requieren Docker)

```bash
cd e2e && ./docker-test.sh
```

- [ ] Pasan los tests unitarios (`go test ./...`)
- [ ] Pasan los tests E2E (`cd e2e && ./docker-test.sh`)
- [ ] Probado manualmente en local

<!-- Describí pasos adicionales de prueba manual si hace falta. -->

---

## 🤖 Checks automatizados

Los siguientes checks corren automáticamente en este PR:

| Check                             | Estado | Descripción                                                                                               |
| --------------------------------- | ------ | --------------------------------------------------------------------------------------------------------- |
| Check PR Cognitive Load           | ⏳     | El PR debería mantenerse dentro de 400 líneas cambiadas (`additions + deletions`) o usar `size:exception` |
| Check Issue Reference             | ⏳     | El cuerpo del PR debe contener `Closes/Fixes/Resolves #N`                                                 |
| Check Issue Has `status:approved` | ⏳     | El issue vinculado debe haber sido aprobado antes de empezar el trabajo                                   |
| Check PR Has `type:*` Label       | ⏳     | Debe aplicarse exactamente una etiqueta `type:*`                                                          |
| Unit Tests                        | ⏳     | Debe pasar `go test ./...`                                                                                |
| E2E Tests                         | ⏳     | Debe pasar `cd e2e && ./docker-test.sh`                                                                   |

---

## ✅ Checklist para contributors

- [ ] El PR está vinculado a un issue con `status:approved`
- [ ] El PR se mantiene dentro de 400 líneas cambiadas, o solicité/obtuve una etiqueta `size:exception` aplicada por maintainers con justificación documentada
- [ ] Agregué la etiqueta `type:*` correspondiente a este PR
- [ ] Pasan los tests unitarios (`go test ./...`)
- [ ] Pasan los tests E2E (`cd e2e && ./docker-test.sh`)
- [ ] Actualicé la documentación si era necesario
- [ ] Mis commits siguen el formato [Conventional Commits](https://www.conventionalcommits.org/)
- [ ] Mis commits no incluyen trailers `Co-Authored-By`

---

## 💬 Notas para reviewers

<!-- Opcional: cualquier cosa a la que quieras que reviewers presten atención especial. -->
