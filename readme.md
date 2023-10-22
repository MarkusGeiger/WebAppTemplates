# Collection of templates for ASP.NET Core WebApps with integrated react SPA

## Step 1 - Add Types and tsconfig

```
npm install --save typescript @types/node @types/react @types/react-dom @types/jest
```

```
npx tsc --init
```

## Step 2 - Rename the .js files to .ts/.tsx

Set `jsx` to `react` in `tsconfig.json`

Remove service-worker and registration for it => PWA is not used here at the moment.

Convert the class components to function components.

There is a special props type where children are needed: `PropsWithChildren``