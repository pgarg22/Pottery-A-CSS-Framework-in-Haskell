# Pottery: A CSS Framework in Haskell

**Pottery** is a functional CSS framework developed in Haskell using the [Clay](https://hackage.haskell.org/package/clay) EDSL (Embedded Domain Specific Language). Clay provides a type-safe, composable, and maintainable way to generate CSS. With Pottery, we leverage popular design paradigms like **Vertical Rhythm** and the **Golden Ratio** to build scalable and aesthetically pleasing stylesheets programmatically.

This repository includes:
- Functional libraries for CSS generation using Haskell
- Two design systems: **Vertical Rhythm** and **Golden Ratio**
- A final report detailing the concepts and implementation
- Licensing information

---

## 📁 Repository Contents

- `README.md` – Project documentation.
- `Golden Ratio/` – Haskell source files for golden ratio-based styling mixins.
- `Vertical Rhythm/` – Haskell source files for vertical rhythm-based styling mixins.
- `Final Report.pdf` – In-depth report describing the theory and implementation.
- `LICENSE` – Open source license.

---

## ✨ Vertical Rhythm

### 📚 Concept

Vertical rhythm is a key typographic principle that enhances readability by maintaining consistent spacing between lines and elements. It depends on:
- **Font size**
- **Line height**
- **Spacing (margin/padding)**

By aligning these to a common vertical grid, layouts become visually harmonious and easier to navigate.

### 🛠️ Our Implementation

We provide configurable variables and a set of reusable mixins to apply vertical rhythm in your stylesheets.

#### Configurable Parameters
- `baseFontSize`
- `baseLineHeight`
- `fontUnit`
- `relativeFontSizing`
- `roundToNearestHalfLine`
- `rhythmBorderStyle`

#### Key Mixins
- `establishBaseline` – Establishes the vertical rhythm baseline.
- `baseline` – Returns baseline styles.
- `rhythm` – Computes rhythm units.
- `toFontSize` / `fontSize` – Adjusts font size.
- `linesToFontSize` – Ensures text fits rhythm units.
- `Leader` / `Trailer` – Adds vertical spacing via margin or padding.
- `propertyRhythm` – Shorthand to add spacing around elements.
- `rhythmBorders`, `leadingBorder`, `trailingBorder`, `horizontalBorder` – Maintain rhythm with borders.

---

## 🌀 Golden Ratio

### 📚 Concept

The **Golden Ratio (φ ≈ 1.618)** has long been used in art, architecture, and design to achieve natural balance and harmony. In web design, applying the golden ratio helps in proportioning text, images, and layout for a visually appealing experience.

### 🛠️ Our Implementation

These mixins adjust typography and spacing based on content width using the golden ratio.

#### Key Mixins
- `grTitleSize` – Title size based on container width.
- `grHeadlineSize` – Headline size styling.
- `grSubHeadlineSize` – Subheadline adjustments.
- `grFontSize` – Base font sizing.
- `grSecondaryText` – Styles for secondary body text.
- `grBaseLineheight` – Line height based on the golden ratio.
- `grCustomLineheight` – User-defined line height using φ.

---

## 🚀 Getting Started

1. Clone the repository.
2. Explore the `Vertical Rhythm` and `Golden Ratio` folders for Haskell code.
3. Use the mixins in your Clay-based CSS generation pipelines.
4. Read `Final Report.pdf` for detailed design explanations and usage examples.

---

## 📜 License

This project is licensed under the terms of the [LICENSE](./LICENSE) file.

---

## 🙏 Acknowledgements

- [Clay](https://hackage.haskell.org/package/clay) – Functional CSS preprocessor in Haskell.
- Design inspiration from traditional typographic theory and modern responsive design practices.
