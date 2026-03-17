Live Demo link: https://react-ecommerce-store-ojvp.vercel.app/

<img width="1855" height="812" alt="image" src="https://github.com/user-attachments/assets/dd184a74-bd3a-451c-946a-d1373eb3c568" />

<img width="1799" height="819" alt="image" src="https://github.com/user-attachments/assets/03b25b0e-3d6e-4f4e-b515-478d2c7c0802" />

<img width="1831" height="803" alt="image" src="https://github.com/user-attachments/assets/82195e86-5073-4171-b27f-740fd451c2b8" />

<img width="1791" height="801" alt="image" src="https://github.com/user-attachments/assets/af13046b-170a-4a79-a60c-9861ddfe645e" />

<img width="1793" height="795" alt="image" src="https://github.com/user-attachments/assets/ea8c75d1-1416-4085-a79d-6536b6d12874" />

<img width="1372" height="794" alt="image" src="https://github.com/user-attachments/assets/bec346f1-2858-4775-83df-52fa3c0123a7" />

<img width="1772" height="806" alt="image" src="https://github.com/user-attachments/assets/3a26b93e-e38b-45f6-aa75-aa605ec0a5d8" />

# Ecommerce React App

Tech Stack
- React
- TypeScript
- Axios
- JSON Server (mock backend)

## Run the project

1. Install dependencies
npm install

2. Start backend
npx json-server --watch backend-app/db.json --port 3000

3. Start frontend
npm run dev










# React + TypeScript + Vite

This template provides a minimal setup to get React working in Vite with HMR and some ESLint rules.

Currently, two official plugins are available:

- [@vitejs/plugin-react](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react) uses [Babel](https://babeljs.io/) (or [oxc](https://oxc.rs) when used in [rolldown-vite](https://vite.dev/guide/rolldown)) for Fast Refresh
- [@vitejs/plugin-react-swc](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react-swc) uses [SWC](https://swc.rs/) for Fast Refresh

## React Compiler

The React Compiler is not enabled on this template because of its impact on dev & build performances. To add it, see [this documentation](https://react.dev/learn/react-compiler/installation).

## Expanding the ESLint configuration

If you are developing a production application, we recommend updating the configuration to enable type-aware lint rules:

```js
export default defineConfig([
  globalIgnores(['dist']),
  {
    files: ['**/*.{ts,tsx}'],
    extends: [
      // Other configs...

      // Remove tseslint.configs.recommended and replace with this
      tseslint.configs.recommendedTypeChecked,
      // Alternatively, use this for stricter rules
      tseslint.configs.strictTypeChecked,
      // Optionally, add this for stylistic rules
      tseslint.configs.stylisticTypeChecked,

      // Other configs...
    ],
    languageOptions: {
      parserOptions: {
        project: ['./tsconfig.node.json', './tsconfig.app.json'],
        tsconfigRootDir: import.meta.dirname,
      },
      // other options...
    },
  },
])
```

You can also install [eslint-plugin-react-x](https://github.com/Rel1cx/eslint-react/tree/main/packages/plugins/eslint-plugin-react-x) and [eslint-plugin-react-dom](https://github.com/Rel1cx/eslint-react/tree/main/packages/plugins/eslint-plugin-react-dom) for React-specific lint rules:

```js
// eslint.config.js
import reactX from 'eslint-plugin-react-x'
import reactDom from 'eslint-plugin-react-dom'

export default defineConfig([
  globalIgnores(['dist']),
  {
    files: ['**/*.{ts,tsx}'],
    extends: [
      // Other configs...
      // Enable lint rules for React
      reactX.configs['recommended-typescript'],
      // Enable lint rules for React DOM
      reactDom.configs.recommended,
    ],
    languageOptions: {
      parserOptions: {
        project: ['./tsconfig.node.json', './tsconfig.app.json'],
        tsconfigRootDir: import.meta.dirname,
      },
      // other options...
    },
  },
])
```
