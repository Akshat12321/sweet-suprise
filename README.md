# Sweet Surprise

Build a mobile-first, romantic, interactive birthday web app inspired by a digital gift card.

### Key Config & Credentials

- Hardcoded PIN: "1311"

- Image Assets: Use the attached images provided in this chat to populate the polaroids and scrapbook frames across the screens.

### Tech Stack & Styling

- Framework: React, TypeScript, Tailwind CSS

- Animation: Framer Motion (page flips, bouncy buttons, candle flame flicker)

- Celebrations: canvas-confetti

- Icons: lucide-react

- Theme & Palette: Romantic pastel blush (#FFE4E8, #FF4B6E, #FF2E55), cream (#FFF9F5), soft white, rounded cards, polaroid frames with subtle drop shadows.

---

### App Screens & Flow

#### 1. Screen 1: Passcode Screen (`PIN_LOCK`)

- Left Side: Polaroid frame showcasing [Attached Image 1] tilted slightly with a cute white border and tape/sticker decal.

- Right Side (Keypad):

  - Heading: "Enter a passcode"

  - 4 blank passcode square boxes.

  - Numeric Keypad (1–9, *, 0, #) with tactile tap animations.

  - Subtext: "hint: it's our fav code ❤️"

- PIN Verification:

  - Required PIN is "1311".

  - If incorrect: shake animation on boxes and clear input.

  - If "1311" is entered: show green highlight and animate in a pulsing "NEXT" button to proceed.

#### 2. Screen 2: Birthday Greeting (`CELEBRATION`)

- Automatic confetti burst on entry (`canvas-confetti`).

- Cute celebration graphic or illustration (teddy bear / cake / party poppers).

- Text: "HAPPY BIRTHDAY!" in bold, playful lettering.

- "NEXT" button in the bottom right leading to the gift selection screen.

#### 3. Screen 3: Gift Hub (`GIFT_HUB`)

- Title: "Gift for you"

- Subtitle: "click any gift to open"

- 3 interactive gift boxes lined up with floating animations:

  - Box 1 -> Opens Birthday Cake Screen

  - Box 2 -> Opens Scrapbook Screen

  - Box 3 -> Opens Love Letter Screen

- Show a small checkmark icon over gifts that have already been opened.

#### 4. Screen 4: Gift 1 - Birthday Cake (`GIFT_CAKE`)

- Warm pastel red/coral backdrop.

- Illustrated birthday cake with glowing, animated candle flames.

- "BLOW" pill button at the bottom.

- On click "BLOW":

  - Extinguish candle flames with a gentle smoke fade effect.

  - Trigger a burst of confetti.

  - Update heading text smoothly to "happy birthday my love ✨".

  - Switch button to a "BACK" button linking back to the Gift Hub.

#### 5. Screen 5: Gift 2 - Scrapbook Collage (`GIFT_SCRAPBOOK`)

- Title: "Happy birthday baby"

- Scrapbook collage layout featuring:

  - Polaroid photo frames containing [Attached Image 2] and [Attached Image 3] with simulated washi tape at the corners.

  - Decorative cute sticker graphics (hearts, cherries, doodles).

  - Short romantic love quotes or handwritten-style notes interspersed between pictures.

- "BACK" button in the bottom corner returning to the Gift Hub.

#### 6. Screen 6: Gift 3 - Love Letter (`GIFT_LETTER`)

- Interactive envelope opening animation.

- A parchment-style letter sliding out containing a heartfelt birthday message.

- 2 smaller Polaroid-style photo cutouts pinned to the side containing [Attached Image 4] and [Attached Image 5].

- Bottom-right "BACK" button to return to the Gift Hub.

---

### Layout Constraints

- Center everything in a clean phone/tablet aspect ratio card container on desktop view, or fill full-screen on mobile devices.

- Store image URLs and text messages in an editable config array at the top of the app file so they can easily be edited or swapped.

This project was built with [Lovable](https://lovable.dev).

## Build with Lovable

Continue developing this project in the [Lovable editor](https://lovable.dev/projects/53b5bbcc-9f76-4594-9adf-37283d24970e).

- **Ship faster**: describe what you want to build and Lovable handles the code.
- **Stay in sync**: every change made in Lovable is committed straight to this repository.
- **Full ownership**: this code is yours. Push to `main` on GitHub and your changes sync back into Lovable, ready for your next prompt.

## Development

Prefer working locally? You need Node.js and npm — [install with nvm](https://github.com/nvm-sh/nvm#installing-and-updating).

```sh
git clone <this-repository-url>
cd <repository-name>
npm i
npm run dev
```
