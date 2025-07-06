# Admin Dashboard

_A decoupled frontend and backend architecture_

## Getting Started

1. **Initialize a new Vite + React project with Tailwind CSS and ShadCN UI**

Follow the official ShadCN installation guide for Vite:  
 👉 [ShadCN UI + Vite Installation Guide](https://ui.shadcn.com/docs/installation/vite)

2. **Install initial ShadCN UI components**

```sh
bunx --bun shadcn@latest add button input label textarea select alert-dialog form
```

3. **Install dependencies**

```sh
bun i react-router
```

4. Setup project structure

- Create basic folders

```sh
mkdir -p src/routes src/types src/layouts src/services/api
```

- Delete default files

```sh
rm src/App.css rm src/assets/react.svg
```

- Create basic files

```sh
touch src/routes/index.tsx
```

5. Replace the content of `src/App.tsx` with the following:

```tsx
import { BrowserRouter } from "react-router";
import AppRoutes from "./routes";

function App() {
  return (
    <BrowserRouter>
      <AppRoutes />
    </BrowserRouter>
  );
}

export default App;
```

6.
