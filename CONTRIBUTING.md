# Contributing to TechnoSpartan

> Gracias por considerar contribuir. No es un proceso burocrático: es una forma de asegurar que el código que entra mantiene el nivel del que sale.

## Antes de empezar

- Lee el README del repo y los ADRs si existen.
- Si vas a tocar arquitectura, abre primero un issue para discutirlo. No queremos descartar trabajo bienintencionado.
- Si es un bug, revisa que no esté ya reportado.

## Flujo de trabajo

1. **Fork** del repo (si eres externo) o **rama** `feature/*` desde `develop`.
2. Commits en **inglés**, formato [Conventional Commits](https://www.conventionalcommits.org/):
   ```
   feat(api): add pagination to user list
   fix(db): handle null foreign keys in migration
   docs(readme): update deployment steps
   ```
3. Tests donde tenga sentido. No pedimos 80 % en un script de 20 líneas, sí en lógica de negocio.
4. PR hacia `develop` con descripción clara del **propósito** y el **contexto técnico**.
5. Revisión de código. Se aceptan críticas constructivas; se rechazan comentarios de estilo sin impacto.

## Estándares de código

- **TypeScript estricto**. `any` solo con justificación documentada.
- **Clean Architecture** cuando el dominio justifica la separación.
- Nombres descriptivos. Un `processData` no dice nada; un `normalizePatientSchedule` sí.
- No dejes código comentado. Git ya lo guarda.

## Decisiones arquitectónicas

Si tu cambio implica:
- Nuevo framework o librería
- Cambio en el modelo de datos
- Nueva forma de despliegue o infraestructura

Documenta la decisión. Puede ser un párrafo en el PR o un ADR si es trascendental.

## Ámbito

No aceptamos contribuciones que:
- Añadan dependencias sin justificación de peso y mantenimiento.
- Introduzcan código que solo funciona en un entorno local específico.
- Rompan contratos públicos sin plan de migración.

## Dudas

Abre un issue con etiqueta `question` o escribe a [contacto@codespartan.es](mailto:contacto@codespartan.es).

---

> No buscamos contribuciones perfectas. Buscamos contribuciones con criterio.
