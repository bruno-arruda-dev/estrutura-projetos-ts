# Estrutura de Projetos TypeScript (Frontend e Backend)

> 🏗️ Esta estrutura segue o padrão **Modular por Domínio (Feature-based)**, onde cada funcionalidade do sistema (ex: produto, usuário) possui seus próprios componentes, serviços, controllers, etc., agrupados em uma única pasta. Isso facilita a escalabilidade, legibilidade e manutenibilidade de projetos grandes.

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
