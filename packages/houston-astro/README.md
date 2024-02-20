# Houston-Astro

The same cool blues, minty greens, and soft purples your used to on Visual Studio, but now packaged for ExpressiveCode's Astro package and Astro's Shiki!

## Install

```
npm i houston-astro
```

## Usage

### Astro ShikiConfig

In your `astro.config.mjs`

```tsx
import { defineConfig } from 'astro/config'
import houston from 'houston-astro';

export default defineConfig({
  markdown: {
    shikiConfig: {
      theme: houston,
    }
  }
})

```

### Astro Expressive Code

In your `astro.config.mjs`

```tsx
import { defineConfig } from 'astro/config'
import astroExpressiveCode from 'astro-expressive-code'
import houston from 'houston-astro';

export default defineConfig({
  integrations: [
    astroExpressiveCode({
      themes: [houston],
    }),
  ],
})

```

### Starlight Expressive Code 

In your `astro.config.mjs`

```tsx
import { defineConfig } from 'astro/config'
import houston from 'houston-astro';

export default defineConfig({
	integrations: [
		starlight({
			expressiveCode: { themes: [houston] },
        })
    ]
});
```

## Issues

Houston is a work in progress. Please [open an issue on our repository](https://github.com/withastro/houston-vscode/issues).
