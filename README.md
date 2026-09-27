# NEXO Planos

Comparador no visual cinematográfico: planos TIM / Vivo / Claro / Nio, solicitação com documentos, IA que não inventa e painel multinível.

## Rodar

```bash
node server.js
```

Abre `http://localhost:3040`

Painel: `/admin.html`  
Login inicial: `dono@nexo.local` / `nexo2026` — troque depois.

## Render

1. New → Web Service
2. Conecte este repositório
3. Start command: `node server.js`
4. Disco persistente (opcional) montado em `/opt/render/project/src/data` para leads e uploads sobreviverem ao restart

## Vercel

Este app é um servidor Node contínuo (JSON + uploads). No Vercel o filesystem é efêmero. Use Render para persistir pedidos, ou ligue o Supabase depois.

## Supabase

Ainda não está no código. O banco atual é `data/db.json`. Próximo passo: tabelas `plans`, `leads`, `knowledge`, `users`, `escalations` + Storage para documentos.
