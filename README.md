# Ebook App Concept

> 👨‍💻 Developed by **[Suresh Kumar Meesala](https://github.com/SureshKumarMeesala)** · 🎨 UI design by **Lorenzo Perniciaro** (credits below)

A mobile app built with **React Native (0.88+)**, **Expo SDK 58+** and **Expo Router**, using **JavaScript and JSX (`.js`, `.jsx`)**. Every screen is built from the original Sketch design `ebook-app-concept-lorez.sketch` by **Lorenzo Perniciaro**: one route per artboard, with the artboard's layout, colours, images and text.

![Ebook App Concept screens](./showcase.jpg)

## 📱 Screens (3 design artboards)

Listed in the order of the app's flow. "Taps" is the number of tap targets wired on the screen (buttons, tabs, back arrows, list rows).

| # | Screen (artboard) | Route | Size | Taps |
|---|---|---|---|---|
| 1 | **Book Dark** · start screen | `src/app/book-dark.jsx` | 375 × 812 | 4 |
| 2 | **Book Dark 3** | `src/app/book-dark-3.jsx` | 375 × 812 | 3 |
| 3 | **Book Dark 2** | `src/app/book-dark-2.jsx` | 375 × 812 | 1 |

Screenshots of every screen are in [`screenshots/`](./screenshots).

## 🧩 How it's built

- `src/screens/*.json`: each design artboard converted to screen data (vector shapes, gradients, image fills, masks, shadows, blurs and rich text, positioned as in the design), plus its tap targets
- `src/sketch/SketchScreen.jsx`: draws a screen at the device's width with `react-native-svg`, native `Text`/`TextInput` and `expo-blur`, and handles navigation between screens
- `src/app/`: Expo Router routes, one per artboard (`index.jsx` opens the start screen)
- `assets/images/`: images used by the design

## 🛠️ Tech Stack

- **Framework**: React Native 0.88+ / Expo SDK 58+
- **Navigation**: Expo Router (file-based routing)
- **Language**: JavaScript & JSX (`.js`, `.jsx`)
- **Rendering**: `react-native-svg`, `expo-blur`
- **Fonts**: Google Fonts via `@expo-google-fonts` (Montserrat, Playfair Display, Poppins), standing in for the design's original fonts where those aren't free

<!-- run-locally:start -->

## ▶️ Run locally

```bash
npm install
npx expo start
```

Then press `i` for the iOS simulator, `a` for Android, or `w` for the web, or scan the QR code with Expo Go.

<!-- run-locally:end -->

<!-- developer:start -->

## 👨‍💻 Developer

This React Native app was developed by **Suresh Kumar Meesala**.

| | |
|---|---|
| Developer | [Suresh Kumar Meesala](https://github.com/SureshKumarMeesala) |
| GitHub | [@SureshKumarMeesala](https://github.com/SureshKumarMeesala) |
| Organization | [FreeAppSource](https://github.com/FreeAppSource) |
| Repository | <https://github.com/FreeAppSource/ebook-app-concept> |

<!-- developer:end -->

---

<!-- design-credits:start -->

## 🎨 Design Credits

This app is based on the free **eBook App Concept** design by **Lorenzo Perniciaro**, downloaded from Sketch App Sources. All visual design credit goes to the designer. The screens are reproduced from the original Sketch file; fonts that aren't free are replaced with similar Google Fonts, so some details may differ slightly from the original.

| | |
|---|---|
| Designer | [Lorenzo Perniciaro](https://www.sketchappsources.com/contributor/lorenzoperniciaro) |
| Original design | [eBook App Concept](https://dribbble.com/shots/10682895--FREE-e-books-app) |
| Downloaded from | [Sketch App Sources](https://www.sketchappsources.com/free-source/4340-ebook-app-concept-sketch-freebie-resource.html) |
| Dribbble | <http://www.dribbble.com/lorez> |
| Website | <http://www.lorenzoperniciaro.com/> |
| Original file | `ebook-app-concept-lorez.sketch` |
| License / usage | Not stated on the page. Free download; give credit (Sketch App Sources Terms). Confirm with the designer before commercial use. |

**Attribution:**

> UI design: "eBook App Concept" by Lorenzo Perniciaro (https://dribbble.com/shots/10682895--FREE-e-books-app), downloaded from Sketch App Sources (https://www.sketchappsources.com/free-source/4340-ebook-app-concept-sketch-freebie-resource.html).

The original design source files are not included in this repository; get them from the links above. This app's **code** is released under the [MIT License](./LICENSE); the visual design remains the designer's (see [NOTICE](./NOTICE)).

Photos, brand logos and avatars inside the design may belong to third parties and are not covered by the designer's permission.

<!-- design-credits:end -->
