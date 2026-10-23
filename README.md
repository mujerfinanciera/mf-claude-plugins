# Mujer Financiera · Plugins para Claude

Marketplace de plugins de [Mujer Financiera](https://www.mujer-financiera.com) para Claude.

## Plugins

| Plugin | Qué hace | Estado |
|---|---|---|
| `mf-finanzas` | Organiza tus finanzas personales con la metodología MF. Hoy incluye la skill **presupuesto-mf**. | v0.1 |

## Instalar

En claude.ai o la app de Claude: **Customize > Plugins > Add > Add marketplace** y pegá `mujerfinanciera/mf-claude-plugins`.

En Claude Code:

```
/plugin marketplace add mujerfinanciera/mf-claude-plugins
/plugin install mf-finanzas@mujer-financiera
```

O en un solo paso:

```
/plugin install mf-finanzas --marketplace mujerfinanciera/mf-claude-plugins
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

## Próximamente

- Más skills del método MF: deudas, ahorro por metas.
- Disponible en el directorio de plugins de Claude.

## Feedback

Abrí un issue en este repo o escribinos a hola@mujer-financiera.com.
