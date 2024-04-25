# Next.js App Directory Snippets Extension

## Snippets

### Typescript

#### `comp` (React Component)

##### Sets component name to the PascalCase version of the file name by default.

##### `navigation-menu.tsx`

```tsx
interface NavigationMenuProps {}

export default function NavigationMenu(props: Readonly<NavigationMenu>) {
    return <span>NavigationMenu</span>;
}
```

#### `acomp` (Asynchronous React Component)

##### Sets component name to the PascalCase version of the file name by default.

##### `theme-switch.tsx`

```tsx
interface ThemeSwitchProps {}

export default async function ThemeSwitch(props: Readonly<ThemeSwitchProps>) {
    return <span>ThemeSwitch</span>;
}
```

#### `compc` (React Component With Children)

##### Sets component name to the PascalCase version of the file name by default.

##### `menu-wrapper.tsx`

```tsx
interface MenuWrapperProps {
    children: React.ReactNode;
}

export default function MenuWrapper({ children }: Readonly<MenuWrapperProps>) {
    return <span>{children}</span>;
}
```

#### `acompc` (Asynchronous React Component With Children)

##### Sets component name to the PascalCase version of the file name by default.

##### `form-container.tsx`

```tsx
interface FormContainerProps {
    children: React.ReactNode;
}

export default async function FormContainer({ children }: Readonly<FormContainerProps>) {
    return <span>{children}</span>;
}
```

#### `rlayout` (Next.js Root Layout)

##### Basic Next.js Root Layout setup.

##### `app/layout.tsx`

```tsx
import type { Metadata } from "next";

export const metadata: Metadata = {
    title: "Title",
    description: "Description",
};

export default function RootLayout({ children }: Readonly<{ children: React.ReactNode }>) {
    return (
        <html lang="en">
            <body>{children}</body>
        </html>
    );
}
```

#### `arlayout` (Asynchronous Next.js Root Layout)

##### Basic Next.js Root Layout setup but this time with the async keyword. Use in case you want to fetch server-side data.

##### `app/layout.tsx`

```tsx
import type { Metadata } from "next";

export const metadata: Metadata = {
    title: "Title",
    description: "Description",
};

export default async function RootLayout({ children }: Readonly<{ children: React.ReactNode }>) {
    return (
        <html lang="en">
            <body>{children}</body>
        </html>
    );
}
```

#### `layout` (Next.js Layout)

##### Sets layout name to the PascalCase version of the parent folder name + Layout by default.

##### `dashboard/layout.tsx`

```tsx
export default function DashboardLayout({ children }: Readonly<{ children: React.ReactNode }>) {
    return <div>{children}</div>;
}
```

#### `alayout` (Asynchronous Next.js Layout)

##### Sets layout name to the PascalCase version of the parent folder name + Layout by default. This time with the async keyword. Use in case you want to fetch server-side data.

##### `devices/layout.tsx`

```tsx
export default async function DevicesLayout({ children }: Readonly<{ children: React.ReactNode }>) {
    return <div>{children}</div>;
}
```

#### `page` (Next.js Page)

##### Sets page name to the PascalCase version of the parent folder name + Page by default.

##### `pricing/page.tsx`

```tsx
export default function PricingPage({
    params,
    searchParams,
}: Readonly<{
    params: { slug: string };
    searchParams: Record<string, string | string[]>;
}>) {
    return <span>PricingPage</span>;
}
```

#### `apage` (Asynchronous Next.js Page)

##### Sets page name to the PascalCase version of the parent folder name + Page by default. This time with the async keyword. Use in case you want to fetch server-side data.

##### `settings/page.tsx`

```tsx
export default function SettingsPage({
    params,
    searchParams,
}: Readonly<{
    params: { slug: string };
    searchParams: Record<string, string | string[]>;
}>) {
    return <span>SettingsPage</span>;
}
```

### Javascript

#### `comp` (React Component)

##### Sets component name to the PascalCase version of the file name by default.

##### `navigation-menu.jsx`

```jsx
export default function NavigationMenu(props) {
    return <span>NavigationMenu</span>;
}
```

#### `acomp` (Asynchronous React Component)

##### Sets component name to the PascalCase version of the file name by default.

##### `theme-switch.jsx`

```jsx
export default async function ThemeSwitch(props) {
    return <span>ThemeSwitch</span>;
}
```

#### `compc` (React Component With Children)

##### Sets component name to the PascalCase version of the file name by default.

##### `menu-wrapper.tsx`

```jsx
export default function MenuWrapper({ children }) {
    return <span>{children}</span>;
}
```

#### `acompc` (Asynchronous React Component With Children)

##### Sets component name to the PascalCase version of the file name by default.

##### `form-container.jsx`

```jsx
export default async function FormContainer({ children }) {
    return <span>{children}</span>;
}
```

#### `rlayout` (Next.js Root Layout)

##### Basic Next.js Root Layout setup.

##### `app/layout.jsx`

```jsx
export const metadata = {
    title: "Title",
    description: "Description",
};

export default function RootLayout({ children }) {
    return (
        <html lang="en">
            <body>{children}</body>
        </html>
    );
}
```

#### `arlayout` (Asynchronous Next.js Root Layout)

##### Basic Next.js Root Layout setup but this time with the async keyword. Use in case you want to fetch server-side data.

##### `app/layout.jsx`

```jsx
export const metadata = {
    title: "Title",
    description: "Description",
};

export default async function RootLayout({ children }) {
    return (
        <html lang="en">
            <body>{children}</body>
        </html>
    );
}
```

#### `layout` (Next.js Layout)

##### Sets layout name to the PascalCase version of the parent folder name + Layout by default.

##### `dashboard/layout.jsx`

```jsx
export default function DashboardLayout({ children }) {
    return <div>{children}</div>;
}
```

#### `alayout` (Asynchronous Next.js Layout)

##### Sets layout name to the PascalCase version of the parent folder name + Layout by default. This time with the async keyword. Use in case you want to fetch server-side data.

##### `devices/layout.jsx`

```jsx
export default async function DevicesLayout({ children }) {
    return <div>{children}</div>;
}
```

#### `page` (Next.js Page)

##### Sets page name to the PascalCase version of the parent folder name + Page by default.

##### `pricing/page.jsx`

```jsx
export default function PricingPage({ params, searchParams }) {
    return <span>PricingPage</span>;
}
```

#### `apage` (Asynchronous Next.js Page)

##### Sets page name to the PascalCase version of the parent folder name + Page by default. This time with the async keyword. Use in case you want to fetch server-side data.

##### `settings/page.jsx`

```jsx
export default function SettingsPage({ params, searchParams }) {
    return <span>SettingsPage</span>;
}
```
