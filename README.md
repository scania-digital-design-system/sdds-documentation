![GitHub release (latest by date)](https://img.shields.io/github/v/release/scania-digital-design-system/sdds) ![npm](https://img.shields.io/npm/v/@scania/components)

# SDDS (Scania Digital Design System) - Legacy Documentation

> **⚠️ Important Notice:** The SDDS source code repository will become private on March 17, 2026. This documentation repository is maintained for reference purposes and will remain public. **For all new projects, please use [Tegel Design System](https://tegel.scania.com/)** - our modern, actively maintained design system.

## 🚀 For New Projects: Use Tegel Design System

SDDS is now legacy. For all new projects, we strongly recommend using:

- 🎨 **Tegel Design System**: [https://tegel.scania.com/](https://tegel.scania.com/)
- 📚 **Tegel Documentation**: [https://tds-storybook.tegel.scania.com](https://tds-storybook.tegel.scania.com)
- 📦 **Tegel Packages**: [https://www.npmjs.com/package/@scania/tegel](https://www.npmjs.com/package/@scania/tegel)

---

## 📦 SDDS Packages (Still Available)

SDDS packages remain available on npm and continue to work. All packages are still supported and will receive security updates.

| Package Name                                    | Description                                         | npm Package |
| ----------------------------------------------- | --------------------------------------------------- | ----------- |
| `@scania/components`                            | Scania reusable web components built with StencilJS | [View on npm](https://www.npmjs.com/package/@scania/components) |
| `@scania/theme-light`                            | Scania default theming                              | [View on npm](https://www.npmjs.com/package/@scania/theme-light) |
| `@scania/typography`                            | Scania official typography styling package          | [View on npm](https://www.npmjs.com/package/@scania/typography) |
| `@scania/colour`                                | Scania official colour scale package                | [View on npm](https://www.npmjs.com/package/@scania/colour) |
| `@scania/grid`                                  | Scania official grid package                        | [View on npm](https://www.npmjs.com/package/@scania/grid) |
| `@scania/icons`                                 | Scania official pictograms & icons package          | [View on npm](https://www.npmjs.com/package/@scania/icons) |

Find all packages in [npm @scania organization](https://www.npmjs.com/org/scania)

---

## 📖 Getting Started with SDDS

### Installation

Install SDDS components and theme:

```shell
npm i @scania/components @scania/theme-light --save
```

### Basic Setup

You can use Tegel CSS custom properties to use the design tokens for colour, typography, spacing, and logotype. To have all CSS custom properties available, you need to install both components and scania-theme, and then include `sdds-theme` component in your application.

#### Install Components

```shell
npm i @scania/components --save
```

#### Install Theme

```shell
npm i @scania/theme-light --save
```

#### Import and Initialize

```js
import { defineCustomElements, addTheme } from '@scania/components';
import { theme as scania } from '@scania/theme-light';

// Add theme
addTheme(scania);

// Define custom elements
defineCustomElements();
```

---

## 🌐 Browser Support

- Chrome
- Firefox
- Safari
- Edge (chromium)

---

## 🔄 Migration

### Migrating from SDDS to Tegel Design System

If you're currently using SDDS and planning to migrate to Tegel Design System, please refer to the [Tegel Design System documentation](https://tegel.scania.com/) for migration guides and best practices.

### Migrating from Corporate UI to SDDS

If you're migrating from Corporate UI 4 to SDDS, follow these steps:

1. **Install SDDS components and theme**

   ```shell
   npm i @scania/components @scania/theme-light --save
   ```

2. **Remove Corporate UI from dependencies**

   ```shell
   npm uninstall corporate-ui
   npm uninstall scania-theme
   ```

3. **Update imports**

   ```js
   import { defineCustomElements, addTheme } from '@scania/components';
   import { theme as scania } from '@scania/theme-light';
   ```

4. **Import Bootstrap separately** (if needed)

   SDDS no longer includes Bootstrap. Import Bootstrap 4 CSS and JS separately from [Bootstrap](https://getbootstrap.com/docs/4.6/getting-started/introduction/) if you need it for legacy components.

5. **Import global-style.css**

   Import the helper CSS file to maintain UI for components that haven't been migrated yet:

   ```css
   @import 'bootstrap/dist/css/bootstrap';
   @import '@scania/theme-light/dist/styles/global-style';
   ```

6. **Update component classes**

   Replace Bootstrap classes with SDDS classes. For example:

   ```html
   <!-- Before -->
   <button type="button" class="btn btn-primary">Primary</button>

   <!-- After -->
   <button type="button" class="sdds-btn sdds-btn-primary">Primary</button>
   ```

For more component updates and migration support, visit [Tegel Design System](https://tegel.scania.com/).

---

## 📚 Additional Resources

- **Legacy Corporate UI Documentation:**
  - [Corporate-UI 3](https://cdn.digitaldesign.scania.com/old-docs/cui/index.html)
  - [Corporate-UI 4](https://digitaldesign.devtest.aws.scania.com/)

---

## ⚠️ Repository Status

**The SDDS source code repository will become private on March 17, 2026.** This means:

- ❌ Source code is no longer publicly accessible
- ❌ Issue tracking is not available
- ❌ Pull requests cannot be submitted
- ❌ Repository cannot be forked

**However:**

- ✅ All npm packages remain available and functional
- ✅ Your existing applications continue to work unchanged
- ✅ Packages will receive security updates
- ✅ This documentation repository remains public for reference

---

## 💬 Support

For questions, support, or migration assistance:

- **New Projects**: Use [Tegel Design System](https://tegel.scania.com/) and its support channels
- **Legacy SDDS Projects**: Contact your team's support channel or reach out to the design system team

---

## 📝 License

SDDS packages are published under their respective licenses. Please check individual package documentation for license information.

---

**Last Updated**: March 2026  
**Status**: Legacy - Use [Tegel Design System](https://tegel.scania.com/) for new projects
