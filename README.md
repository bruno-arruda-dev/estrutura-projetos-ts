# Estrutura de Projetos TypeScript (Frontend e Backend)

Este repositório contém um guia de estrutura modular por domínio (feature-based), aplicável a projetos em React, Next.js, Node e NestJS.

---

## 📦 Estrutura Recomendada

```
src/
├── produto/
│   ├── components/
│   ├── dto/
│   ├── hooks/
│   ├── services/
│   ├── utils/
│   ├── entities/
│   ├── produto.page.tsx
│   └── produto.controller.ts

├── usuario/
│   ├── components/
│   ├── dto/
│   ├── services/
│   ├── usuario.page.tsx
│   └── usuario.controller.ts

├── shared/
│   ├── components/
│   ├── hooks/
│   ├── styles/
│   ├── types/
│   └── middlewares/

├── lib/
│   ├── formataCpf.ts
│   └── geraToken.ts

├── config/
│   ├── axios.ts
│   ├── env.ts
│   └── database.ts

├── routes/
├── main.ts / index.tsx
└── app.module.ts
```

---

## ✅ Recomendações

- Use `shared/` para tudo que for reaproveitado entre features.
- Use `lib/` para helpers e utilitários genéricos, desacoplados.
- Use `config/` para arquivos de configuração global.
- Prefira `hooks/`, `dto/` e `components/` específicos dentro da feature.
