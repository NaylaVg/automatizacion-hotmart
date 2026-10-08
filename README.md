# automatizacion-hotmart

La idea es crear un software donde pueda utilizar varios agentes IA para promocionar automáticamente un producto de Hotmart
Estructura
hotmart-automation/
├── .env
├── .env.example
├── .gitignore
├── README.md
├── requirements.txt
├── manage.py
├── config/               # settings, urls, celery.py
├── apps/
│   ├── content/          # ContentPost, generación de copy, publicación
│   ├── messaging/        # webhook de Meta, clasificador, respuestas
│   └── leads/            # sincronización con Odoo, seguimientos
├── integrations/
│   ├── meta_client.py    # llamadas a Graph API
│   ├── claude_client.py  # llamadas a la API de Claude
│   └── odoo_client.py    # XML-RPC / JSON-RPC
├── docs/
│   ├── bitacora/         # entradas en Markdown (material del e-book)
│   └── marketing/        # briefing y plan de marketing
└── youtube/              # guiones y notas de cada video
