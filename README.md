# Sitio Web Know How S.A. de C.V.

Sitio comercial de Know How — software hospitalario, agentes IA y consultoría organizacional.

## Estructura

```
sitio-web/
├── docs/         Documentación, contenido, decisiones (NO se publica)
├── src/          Código del sitio (esto SÍ se publica)
└── assets/       Imágenes, logos, fuentes
```

## Stack

- HTML5 + CSS3 + JavaScript vanilla
- Sin framework
- Sin build step
- Hosting: Cloudflare Pages
- Repo: github.com/nicolasmolina-boop/knowhow

## Cómo trabajar

### Editar local
1. Abrí cualquier archivo de `src/` con VS Code
2. Hacé los cambios
3. Probá abriendo `src/index.html` directo en el navegador (doble click)

### Publicar
```bash
git add .
git commit -m "describe el cambio"
git push
```
Cloudflare Pages detecta el push y despliega solo en ~30 segundos.

### Ver el sitio en vivo
- Producción: (pendiente — cuando se conecte el dominio)
- Preview de Cloudflare: (pendiente — cuando se conecte el repo)

## Reglas

1. **Nunca subir credenciales, API keys, contraseñas.** Usar variables de entorno de Cloudflare si hace falta.
2. **Cada cambio debe tener un commit message claro.** No `update`, no `cambios`.
3. **Probar local antes de pushear.**
4. **Las imágenes pesadas se optimizan antes de subir** (TinyPNG o Squoosh).
5. **No agregar dependencias sin necesidad.** Cada librería es deuda futura.

## Documentos importantes

- [KH-01 Contexto Empresa](../[KH-01]%20Contexto%20Empresa.md)
- [KH-02 Decisión Sitio Web](../[KH-02]%20Decision%20Sitio%20Web.md)
- [Estructura de páginas](docs/estructura-paginas.md)
