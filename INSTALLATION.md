# Installations

## Angular

```script
npx -p @angular/cli@[version] ng new name  [--no-standalone]
```

### Angular 18.2.5

| Script | Installation | Build Size (prod) | Build Size (application, prod) |
|--------|--------------|-------------------|--------------------------------|
| `npx -p @angular/cli@18 ng new angular-18.2.5-no-standalone --no-standalone` | 324 MB | 1.34 MB | |
| `npx -p @angular/cli@18 ng new angular-18.2.5-standalone` | 322 MB | 1.35 MB | |

## Vue

```script
npm create vue@latest
```

### Vue 3.5.10

| Script | Installation | Build Size (prod) | Build Size (application, prod) |
|--------|--------------|-------------------|--------------------------------|
| `npm create vue@latest` (no typescript) | 87 MB | 79 KB | |
| `npm create vue@latest` (typescript) | 130.5 MB | 79 KB | |

## React

### React 18.3.1 (Next.js Framework)

```script
npx create-next-app@latest
```

| Script | Installation | Build Size (prod) | Build Size (application, prod) |
|--------|--------------|-------------------|--------------------------------|
| `npx create-next-app@latest` (no typescript) | 270 MB | 879 KB | |
| `npm create-next-app@latest` (typescript) | 274 MB | 879 KB | |

### React 18.3.1 (Remix Framework)

```script
npx create-remix
```

| Script | Installation | Build Size (prod) | Build Size (application, prod) |
|--------|--------------|-------------------|--------------------------------|
| `npx create-remix` | 198 MB | 395 KB | |

### React 18.3.1 (Gatsby)

```script
npx create-gatsby
```

| Script | Installation | Build Size (prod) | Build Size (application, prod) |
|--------|--------------|-------------------|--------------------------------|
| `npx create-gatsby` (no typescript) | 371 MB | 1.2 MB | |
| `npx create-gatsby` (typescript) | 406 MB | 1.2 MB | |

### React (Create-React-App)

```script
npx create-react-app [name]
```

| Script | Installation | Build Size (prod) | Build Size (application, prod) |
|--------|--------------|-------------------|--------------------------------|
| `npx create-react-app` | 250 MB | 563 KB | |

# Site-Level Notes

## Options

| Framework | Version | TypeScript | Unit Tests | E2E Tests | ESLint | Prettier |
|-----------|---------|------------|------------|-----------|--------|----------|
| Angular | 18.2.5 | DEFAULT | DEFAULT | (can install) | - | - |
| React (Create-React-App) | 18.3.1 (5.0.1) | - | DEFAULT | - | - | - |
| React (Gatsby) | 18.3.1 (3.13.1) | optional | - | - | - | - |
| React (Next.js) | 18.3.1 (14.2.14) | optional | - | - | optional | - |
| React (Remix) | 18.3.1 (2.12.1) | DEFAULT | - | - | DEFAULT | - |
| Vue | 3.5.10 | optional | optional | optional | optional | optional |

## Lighthouse

(original code)

| Framework | Version | Performance | Accessibility | Best Practices | SEO | Performance Metrics |
|-----------|---------|-------------|---------------|----------------|-----|---------------------|
| Angular | 18.2.5 | 91 | 95 | 81 | 90 | 1.4 s FCP, 1.4 s LCP, 0 ms TBT, 0 CLS, 1.4 s SI |
| React (Create-React-App) | 18.3.1 (5.0.1) | 100 | 100 | 81 | 100 | 0.2 s FCP, 0.4 s LCP, 0 ms TBT, 0 CLS, 0.2 s SI |
| React (Gatsby) | 18.3.1 (3.13.1) | 100 | 95 | 81 | 91 | 0.2 s FCP, 0.5 s LCP, 0 ms TBT, 0 CLS, 0.2 s SI |
| React (Next.js) | 18.3.1 (14.2.14) | 100 | 100 | 81 | 100 | 0.3 s FCP, o.7 s LCP, 0 ms TBT, 0 CLS, 0.3 s SI |
| React (Remix) | 18.3.1 (2.12.1) | 100 | 100 | 81 | 100 | 0.4 s FCP, 0.5 s LCP, 0 ms TBT, 0 CLS, 0.4 s SI |
| Vue | 3.5.10 | 100 | 88 | 81 | 91 | 0.4 s FCP, 0.4 s LCP, 0 ms TBT, 0 CLS, 0.4 s SI |

1. FCP: First Contentful Paint
2. LCP: Largest Contentful Paint
3. TBT: Total Blocking Time
4. CLS: Cumulative Layout Shift
5. SI: Speed Index
