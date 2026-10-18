# KW-Cloude-Plugin

Plugin de KeyWords para Claude Code, para que cualquier usuario de KeyWords lo instale sin acceso al código de la app.

## Instalación (usuario final)

1. En KeyWords: **Mi perfil → Conectar Claude Code → Generar token** y correr el comando `claude mcp add ...` que aparece. Eso conecta el servidor MCP con tu cuenta.
2. En Claude Code:
   ```
   /plugin marketplace add Kyriokes/KW-Cloude-Plugin
   /plugin install keywords@keywords
   ```
3. Tener la extensión **Claude in Chrome** conectada y la sesión iniciada en los portales donde vayas a postular.
4. Decirle a Claude: "postulá mi cola" (o `/postular`).

## Contenido

- `.claude-plugin/marketplace.json`: catálogo con un solo plugin.
- `plugins/keywords/skills/postular/SKILL.md`: el flujo de postulación y sus reglas (confirmación antes de cada envío, sin LinkedIn ni Indeed, sin cuentas ni contraseñas).

El plugin no trae el servidor MCP: se agrega en el paso 1 con el token personal, así el token no queda en archivos del plugin.

## Probarlo localmente

```
/plugin marketplace add ./
/plugin install keywords@keywords
```
