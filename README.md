# Mujer Financiera · Plugins para Claude

Marketplace de plugins de [Mujer Financiera](https://www.mujer-financiera.com) para Claude.

## Plugins

| Plugin | Qué hace | Estado |
|---|---|---|
| `mf-finanzas` | Organiza tus finanzas personales con la metodología MF. Hoy incluye la skill **presupuesto-mf**. | Beta |

## Instalar (Claude Code)

```
/plugin marketplace add mujerfinanciera/mf-claude-plugins
/plugin install mf-finanzas@mujer-financiera
```

Después, en cualquier conversación: "ayudame a armar mi presupuesto" o `/mf-finanzas:presupuesto-mf`.

## Probar en local sin instalar

```
claude --plugin-dir ./plugins/mf-finanzas
```

## Validar antes de publicar

```
claude plugin validate ./plugins/mf-finanzas
```

## Estructura

```
mf-claude-plugins/
├── .claude-plugin/
│   └── marketplace.json          # catálogo del marketplace MF
└── plugins/
    └── mf-finanzas/
        ├── .claude-plugin/
        │   └── plugin.json       # manifest del plugin
        └── skills/
            └── presupuesto-mf/
                ├── SKILL.md      # el método, paso a paso
                ├── templates/    # plantillas de salida (md + csv)
                └── examples/     # conversación de ejemplo
```

## Roadmap

- [ ] Sabrina valida `SKILL.md` (reglas 50/30/20 y 80/20, fondo de emergencia 1→3-6 meses, tono)
- [ ] Probar con 3-5 alumnas beta y ajustar
- [ ] Skills siguientes: `deudas-mf`, `ahorro-metas-mf`
- [ ] Conector MCP con Nora (presupuesto sobre datos reales)
- [ ] Enviar al directorio oficial de Anthropic
