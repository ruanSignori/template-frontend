## Pacotes, e FrameWorks utilizados

- Next
- TypeScript
- TailwindCss
- Jest
- Eslint

## Instalar dependências

```bash
 yarn
 #ou
 npm i
```

## Iniciar o projeto

Execute um dos seguintes comandos, conforme o gerenciador de pacotes utilizado.

```bash
npm run dev
# ou
yarn dev
# ou
pnpm dev
# ou
bun dev
```

Acesse [http://localhost:3000](http://localhost:3000) para ver o site em funcionamento.

## Estrutura de pastas

```
├─ public/ # Recursos estáticos públicos (imagens, arquivos, etc.)
│  └─ images/ # Imagens utilizadas no projeto
├─ src/ # Irá conter todo o código fonte do projeto
|  └─ @types/ # Definição de tipos TypeScript para bibliotecas
|  └─ app/
|  └─ components/ # Armazenar componentes React reutilizáveis
|  └─ functions/ # Funcionalidades específicas do projeto que podem ou não, ser reutilizáveis
|  └─ hooks/ # React Hooks personalizados
|  └─ lib/ # Funções e manipulação de chamada para API's
|  └─ styles/ # Definições de classes com Tailwind
|  └─ test/ # Testes de scripts
│  │  └─ integration / # Testes de integração (chamada e consumo de api)
|  |  └─ unitary / # Testes unitários (botões, operações matemáticas, algoritmos)
|  └─ types/ # Adicionar tipo à variáveis
├─ .env.example # Variáveis de ambiente (crie um arquivo .env para salvar os seus valores)
├─ next.config.js # Configurações específicas do Next.js
├─ package.json # Arquivo de configuração do npm
├─ README.md # Este arquivo
├─ tailwind.config.js # Configurações específicas do Tailwindcss
├─ tsconfig.json # Configurações ambiente do TypeScript
```

## Estrutura de arquivos

```
├─ types
|  └─ index.ts
|  └─ example-user.ts
|  └─ other-example-user.ts
```

```typescript
// example-user.ts
export interface ExampleModel {
  name: string;
  age: number;
}
```

```typescript
// index.ts
export { ExampleModel } from "./example-user";
```

Deixar o `index.ts` fazer a exportação para evitar que o código de importação fique muito verboso.
