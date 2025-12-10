# AWWWARDS INTERACTIONS PRESETS v2
Hiệu ứng từ Awwwards winners - mô tả tự nhiên, keywords để implement

---

## Cách dùng

File này là "menu" các effects. Mỗi effect được mô tả bằng ngôn ngữ tự nhiên - AI sẽ tự implement phù hợp với context và style của project.

**Keywords** được đánh dấu để dễ search và reference.

---

## FOUNDATION - Nền tảng

### Smooth Scroll
`lenis` `locomotive-scroll` `lerp` `momentum` `inertia`

Nền tảng của mọi Awwwards site. Scroll mượt như lụa, có momentum và easing tự nhiên. Khi dừng scroll, trang tiếp tục trượt nhẹ rồi dừng từ từ thay vì dừng đột ngột. Cảm giác như đang lướt trên băng.

Thường dùng: Lenis hoặc Locomotive Scroll kết hợp GSAP ScrollTrigger.

**Quan trọng:** Không có smooth scroll thì mọi effect khác đều mất cảm giác premium.

---

### Scroll Velocity Awareness
`scroll-velocity` `scroll-direction` `speed-based`

Website nhận biết tốc độ và hướng scroll. Scroll nhanh → effects nhanh/mạnh hơn. Scroll chậm → effects nhẹ nhàng. Scroll lên vs xuống có thể trigger behaviors khác nhau.

Ứng dụng: Marquee text chạy nhanh hơn khi scroll nhanh, parallax intensity thay đổi theo velocity, elements skew theo hướng scroll.

---

## TEXT ANIMATIONS

### Line Reveal (Mask)
`text-reveal` `line-mask` `overflow-hidden` `translateY` `stagger`

Chữ xuất hiện từng dòng từ dưới lên, như đang được vén màn. Mỗi dòng nằm trong container có overflow hidden, text translate từ 100% lên 0. Stagger 0.1-0.15s giữa các dòng.

Khi nào dùng: Headlines, hero text, section titles. Gần như mọi Awwwards site đều có.

---

### Character Stagger
`split-text` `char-animation` `letter-stagger` `3d-rotate`

Từng ký tự xuất hiện riêng lẻ với stagger rất nhỏ (0.02-0.05s). Có thể kèm rotation, blur, hoặc scale. Tạo cảm giác chữ đang "được đánh máy" hoặc "lắp ráp từng mảnh".

Variations:
- Fade up từ dưới
- Rotate từ trục X (như lật thẻ)
- Random delay tạo hiệu ứng organic
- Blur to sharp

---

### Text Scramble / Decode
`scramble` `decode` `glitch-text` `random-chars` `typewriter`

Text hiển thị qua giai đoạn "giải mã" - random characters chạy rồi settle vào đúng chữ. Mỗi ký tự nhảy qua vài random chars trước khi đúng. Mang vibe tech, hacker, futuristic.

Khi nào dùng: Tech sites, creative agencies muốn edgy, hover states cho links, hero headlines.

---

### Gradient Text Fill on Scroll
`gradient-text` `scroll-fill` `text-highlight` `reading-progress`

Text có gradient hoặc opacity thay đổi theo scroll position. Phần đã scroll qua sáng lên (hoặc đổi màu), phần chưa tới thì mờ. Như đang highlight text theo reading progress.

Thường dùng cho: Long-form text, manifesto sections, storytelling, about pages.

---

### Marquee / Infinite Ticker
`marquee` `ticker` `infinite-scroll` `horizontal-loop`

Text chạy liên tục theo một hướng, loop vô tận. Comeback của hiệu ứng 90s nhưng với typography đẹp hơn.

Variations:
- Chạy liên tục một hướng
- Đổi hướng khi hover
- Đổi hướng theo scroll direction
- Tốc độ thay đổi theo scroll velocity
- Hai rows chạy ngược chiều

Khi nào dùng: Dividers giữa sections, footer, brand statements, skill lists.

---

### Kinetic Typography
`kinetic` `word-scatter` `text-explosion` `independent-words`

Words hoặc letters di chuyển độc lập theo scroll hoặc cursor. Mỗi từ có speed/direction riêng. Tạo cảm giác typography "sống" và phản ứng với user.

Variations:
- Words parallax ở speeds khác nhau
- Letters scatter khi scroll
- Text explosion từ center
- Words follow cursor với delays khác nhau

---

### Typing / Typewriter
`typing` `typewriter` `cursor-blink` `sequential-reveal`

Text xuất hiện từng ký tự như đang được gõ. Có cursor nhấp nháy ở cuối. Classic nhưng vẫn effective cho certain contexts.

Khi nào dùng: Hero subtitles, terminal aesthetics, chatbot interfaces, code snippets.

---

## SCROLL EFFECTS

### Parallax Layers
`parallax` `depth` `z-layers` `scroll-speed` `foreground-background`

Các elements di chuyển với tốc độ khác nhau khi scroll, tạo cảm giác depth 3D. Layer gần (foreground) scroll nhanh, layer xa (background) scroll chậm.

Intensity: Subtle (-10% đến -30%) cho elegant, dramatic (-50% trở lên) cho impact.

Tip: Background images parallax nhẹ, decorative elements parallax mạnh hơn, text thường giữ tốc độ normal.

---

### Horizontal Scroll Section
`horizontal-scroll` `pin` `scrub` `scroll-hijack` `side-scroll`

Scroll dọc bình thường, nhưng có section mà khi tới thì content chạy ngang. Section được pin lại, scroll dọc được convert thành chuyển động ngang.

Cảm giác: Như đang xem slideshow được điều khiển bằng scroll. Cinematic, gallery-like.

Khi nào dùng: Project showcases, image galleries, timeline, feature tours.

**Warning:** Dùng có chừng mực. Quá nhiều scroll hijacking làm user frustrated.

---

### Pin & Progressive Reveal
`pin` `sticky` `progressive-reveal` `scroll-timeline` `step-reveal`

Section được pin/sticky, content bên trong reveal dần theo scroll progress. Elements fade in, slide in, hoặc transform vào vị trí khi user scroll.

Variations:
- Stacked cards reveal từng cái
- Text paragraphs highlight lần lượt
- Features appear one by one
- Before/after comparison
- Step-by-step storytelling

---

### Scale on Scroll (Hero Zoom)
`zoom` `scale` `hero-zoom` `dive-in` `scroll-scale`

Element (thường là image hoặc video) zoom in hoặc zoom out theo scroll. Tạo cảm giác "dive into" hoặc "pull back from" content.

Common uses:
- Hero image zoom out khi scroll xuống (reveal more context)
- Image zoom in khi approach (focus attention)
- Full-page zoom transition giữa sections
- Product reveal từ xa đến gần

---

### Clip-path Reveal
`clip-path` `mask` `wipe` `reveal-animation` `shape-reveal`

Content được reveal bằng cách animate clip-path - như một cửa sổ mở ra hoặc curtain kéo đi. Có thể từ bất kỳ hướng nào.

Shapes phổ biến:
- Inset (rectangular wipe từ edges)
- Circle (từ center expand ra)
- Polygon (creative shapes, diagonal reveals)

Khi nào dùng: Image reveals, section transitions, hero entrances, project thumbnails.

---

### Sticky Footer Reveal
`sticky-footer` `reveal-underneath` `page-lift` `footer-discovery`

Content scroll đi và reveal footer ở phía dưới - như đang lật một trang giấy. Footer luôn ở đó fixed, chỉ bị che bởi main content.

Cảm giác: Surprising, elegant ending. Footer feels "discovered" không phải "reached".

---

### Image Sequence (Apple Style)
`image-sequence` `frame-animation` `scroll-video` `canvas-sequence`

Scroll controls một sequence of images, tạo hiệu ứng như video được điều khiển bằng scroll. Như các product pages của Apple.

Technical: Preload 100-300 frames, render to canvas, GSAP scrub controls frame index.

Khi nào dùng: Product reveals, 3D object rotation, process visualization, storytelling.

---

### Elastic/Staggered Grid Scroll
`elastic-grid` `staggered-scroll` `column-speed` `grid-parallax`

Grid layout mà mỗi column/row scroll ở tốc độ hơi khác nhau, tạo hiệu ứng "elastic" mềm mại khi scroll.

Cảm giác: Grid feels alive, organic, không rigid như normal grid.

---

## HOVER & CURSOR

### Magnetic Elements
`magnetic` `cursor-attraction` `hover-pull` `elastic-snap`

Button hoặc element bị "hút" về phía cursor khi hover gần. Element follow cursor trong phạm vi của nó. Khi leave, snap back với elastic bounce.

Physics: Lerp/easing để follow smooth, elastic ease khi snap back.

Khi nào dùng: CTAs, navigation items, social icons, any interactive element muốn feel alive.

---

### Custom Cursor
`custom-cursor` `cursor-follow` `cursor-dot` `cursor-circle` `blend-mode`

Thay thế cursor mặc định bằng custom element. Thường là dot nhỏ + circle lớn follow với delay (lerp).

Variations:
- Dot + trailing circle
- Scale up khi hover clickable
- Change color/blend mode based on background
- Morph shape theo context
- Hide on scroll, show on move

Common: `mix-blend-mode: difference` để cursor luôn visible trên mọi background.

---

### Text Cursor Labels
`cursor-text` `cursor-label` `contextual-cursor` `view-play-drag`

Cursor hiển thị text label tùy theo element đang hover. "View" cho images, "Play" cho videos, "Drag" cho sliders.

Implementation: Hidden label div follows cursor, show/change text on hover specific elements via data attributes.

---

### Link Underline Animations
`underline` `hover-line` `draw-underline` `slide-underline`

Underline không chỉ appear/disappear mà animate - grow, slide, draw.

Patterns phổ biến:
- Grow từ left to right
- Grow từ center ra hai bên
- Slide out right, new one slide in from left
- Draw như đang vẽ
- Thickness/color change on hover

---

### Menu Hover - Reveal Image
`menu-image` `hover-preview` `cursor-image` `project-preview`

Khi hover vào menu item/project title, một preview image xuất hiện. Image có thể follow cursor hoặc appear ở vị trí fixed.

Variations:
- Image follows cursor
- Image appears at fixed position
- Multiple images cycle through
- Image with parallax effect on cursor move
- Clip-path reveal animation

---

### Menu Hover - Marquee Text
`menu-marquee` `hover-ticker` `text-scroll-hover`

Khi hover vào menu item, text bắt đầu scroll/marquee trong container của nó. Very signature Awwwards effect.

Implementation: Two layers - static text và marquee text. On hover, static hides, marquee shows và animates.

---

### Image Hover - Scale & Pan
`hover-zoom` `image-pan` `ken-burns` `overflow-hidden`

Image zoom in nhẹ khi hover, có thể kèm subtle pan theo cursor position. Container overflow hidden để crop. Ken Burns effect variation.

---

### Card Tilt (3D Perspective)
`card-tilt` `perspective` `mouse-position` `3d-transform`

Card tilt theo mouse position, tạo cảm giác 3D. Có thể kèm reflection, light effect, shadow movement.

Physics: Calculate mouse position relative to card center, apply rotateX/Y transforms, add perspective to parent.

---

### Button Hover States
`button-hover` `fill-animation` `border-animation` `state-change`

Buttons với elaborate hover states:
- Background fill từ một direction
- Border draws around
- Text color inverts
- Icon animates
- Multiple layers reveal

---

## IMAGE & MEDIA EFFECTS

### Image Reveal (Scroll-triggered)
`image-reveal` `lazy-reveal` `scroll-appear` `fade-scale`

Images không load/appear ngay mà reveal khi scroll tới. Có thể fade, scale, slide, hoặc clip-path reveal.

Variations:
- Simple fade + slight scale up
- Slide in from sides
- Clip-path wipe
- Blur to sharp
- Grayscale to color

---

### Image Distortion on Hover
`webgl` `distortion` `displacement` `wave-effect` `liquid`

Image bị distort khi hover - wave effect, liquid ripple, RGB split. Cần WebGL/Three.js hoặc CSS filters for simpler versions.

Effects:
- Wave/ripple từ cursor position
- RGB channel split
- Noise displacement
- Liquid/gooey morph
- Glitch effect

---

### Image-to-Image Transition
`image-swap` `displacement-transition` `morph` `crossfade`

Hover để transition từ image A sang image B với effect. Không chỉ crossfade mà có displacement, distortion trong quá trình.

Khi nào dùng: Before/after, product color variants, team member photos (casual/professional).

---

### Video on Hover
`video-hover` `play-on-hover` `preview-video` `autoplay-hover`

Video plays khi hover, pause khi leave. Poster image shows khi không hover.

Considerations: Preload, muted autoplay, smooth transition between poster và video.

---

### Lazy Load with Blur
`lazy-load` `blur-up` `progressive-image` `placeholder`

Images load với low-res blurred placeholder trước, then sharp image fades in. Like Medium's image loading.

---

## PAGE TRANSITIONS

### Fade Through
`page-transition` `fade` `crossfade` `opacity`

Simple nhất: Page cũ fade out, page mới fade in. Có thể có slight overlap (crossfade) hoặc fade to color rồi fade in.

---

### Slide / Wipe Transition
`slide-transition` `wipe` `directional` `push`

Page slide ra một hướng, page mới slide vào từ hướng ngược lại. Direction có thể based on navigation direction.

---

### Expand from Element (Shared Element)
`zoom-transition` `expand` `morph` `flip-animation` `shared-element`

Click vào element (card, image), element đó expand ra full screen và morph thành page mới. Content của new page reveals bên trong.

Còn gọi là: Shared element transition, FLIP animation. Very impressive khi done right.

---

### Curtain / Overlay Transition
`curtain` `overlay` `cover` `theatrical`

Một layer (màu solid, gradient, hoặc pattern) cover screen từ một direction, rồi reveal page mới từ direction khác. Theatrical, dramatic.

Variations:
- Single curtain wipe
- Two curtains meet in middle
- Multiple strips with stagger
- Circle expand from click position

---

### Pixelation / Dissolve
`pixelate` `dissolve` `dither` `noise-transition`

Page transition qua hiệu ứng pixelation hoặc noise dissolve. Retro, glitchy feel.

---

## 3D & WEBGL

### Particle Systems
`particles` `canvas` `points` `interactive-particles`

Background hoặc decorative particles react to cursor hoặc scroll. Có thể là dots, lines connecting, shapes, hay abstract forms.

Behaviors:
- Follow cursor
- Repel from cursor
- Attract to cursor
- React to scroll velocity
- Form shapes/text

---

### 3D Scene Background
`three.js` `webgl-background` `3d-environment` `ambient`

3D scene làm background cho website. Có thể là abstract shapes, environments, hoặc product showcase.

Interactions: React to scroll, cursor, gyroscope (mobile).

---

### Shader Effects
`glsl` `shader` `post-processing` `visual-effects`

Custom shaders cho unique visual effects:
- Chromatic aberration
- Noise/grain overlay
- Color manipulation
- Distortion effects
- Light/glow effects

---

### Scroll-driven 3D
`scroll-3d` `rotate-on-scroll` `3d-scroll` `object-manipulation`

3D objects rotate, move, or transform based on scroll position. Product showcases, storytelling with 3D elements.

---

## MICRO-INTERACTIONS

### Button Press Feedback
`button-press` `tactile` `click-feedback` `active-state`

Khi click button, có visual feedback như đang nhấn xuống - translateY xuống một chút, shadow giảm. Release thì bounce back.

---

### Form Input Animations
`input-focus` `label-float` `validation-feedback` `form-micro`

Input fields với animated states:
- Label float lên khi focus/filled
- Border highlight animation
- Validation states với smooth transitions
- Character count animations

---

### Toggle / Switch
`toggle` `switch` `state-transition` `morph-toggle`

Toggle switches với smooth animation giữa states. Indicator moves, colors change, icons morph.

---

### Loading States
`skeleton` `shimmer` `pulse` `loading-animation`

Loading states với style:
- Skeleton screens với shimmer effect
- Pulse animation cho placeholders
- Progress indicators
- Creative loaders matching brand

---

### Notification / Toast
`toast` `notification` `slide-in` `auto-dismiss`

Notifications appear với animation, auto-dismiss sau duration. Slide in from edge, stack nicely if multiple.

---

### Accordion / Expand
`accordion` `expand-collapse` `height-animation` `smooth-toggle`

Content expand/collapse với smooth height animation. Icon rotates, content fades in.

---

### Counter Animation
`counter` `number-roll` `count-up` `odometer`

Numbers animate from 0 to target value, hoặc roll like odometer. Trigger on scroll into view.

---

### Copy to Clipboard
`copy` `clipboard` `success-feedback` `tooltip-confirm`

Click to copy với visual confirmation. Button text changes, tooltip appears, checkmark animation.

---

## LAYOUT & STRUCTURE

### Staggered Grid Animation
`grid-stagger` `item-reveal` `masonry-animate` `sequential`

Grid items appear với stagger delay, tạo wave effect. Items có thể fade, scale, slide vào từ different directions.

---

### List Item Animations
`list-animate` `item-stagger` `hover-highlight` `active-indicator`

List items với hover states, staggered entrance, active indicators. Menu items, feature lists, pricing tables.

---

### Section Transitions
`section-enter` `scroll-section` `viewport-trigger` `section-animate`

Mỗi section có entrance animation khi scroll vào viewport. Consistent pattern xuyên suốt site.

---

### Scroll Progress Indicator
`scroll-progress` `reading-progress` `progress-bar` `scroll-indicator`

Visual indicator showing scroll progress. Could be line at top, circle indicator, or integrated into design.

---

### Back to Top
`back-to-top` `scroll-to-top` `appear-on-scroll` `smooth-scroll-top`

Button appears sau khi scroll một khoảng, click để smooth scroll về top. Often với animation khi appear/disappear.

---

## MATCHING GUIDE

### Theo Style

**Minimal/Clean:**
- Text: Line reveal, subtle fade
- Scroll: Gentle parallax, fade in
- Hover: Underline grow, opacity change
- Transitions: Simple fade

**Bold/Creative:**
- Text: Character animation, scramble
- Scroll: Horizontal scroll, dramatic zoom
- Hover: Magnetic, image distortion
- Transitions: Expand, curtain

**Editorial/Luxury:**
- Text: Elegant line reveal, slow timing
- Scroll: Smooth parallax, pin & reveal
- Hover: Refined underlines, subtle zoom
- Transitions: Crossfade, elegant wipes

**Tech/Futuristic:**
- Text: Scramble, glitch effects
- Scroll: 3D transforms, clip-path
- Hover: Custom cursor, distortion
- Transitions: Geometric wipes, pixelation

**Playful/Creative:**
- Text: Bouncy reveals, color changes
- Scroll: Fun parallax, unexpected movements
- Hover: Exaggerated magnetic, playful cursors
- Transitions: Colorful curtains, morphs

### Theo Content Type

**Portfolio:** Image reveals, project hovers với preview, smooth page transitions
**Agency:** Bold scroll effects, creative cursors, impressive page transitions
**E-commerce:** Subtle hovers, quick transitions, micro-interactions for UX
**Editorial:** Text-focused effects, reading progress, parallax images
**Product/SaaS:** Feature reveals, demo animations, conversion-focused micro-interactions

---

## PERFORMANCE NOTES

**Animate only (GPU-accelerated):**
- transform (translate, scale, rotate)
- opacity
- clip-path (modern browsers)

**Avoid animating:**
- width, height
- margin, padding
- top, left, right, bottom
- box-shadow (fake with pseudo-element)

**Best practices:**
- Use `will-change` sparingly và remove after animation
- Throttle scroll/mouse events
- Prefer CSS transitions for simple effects
- Use GSAP for complex choreography
- Test on mid-range devices
- Provide `prefers-reduced-motion` fallback

---

## LIBRARIES QUICK REFERENCE

**Smooth scroll:** Lenis, Locomotive Scroll
**Animation:** GSAP + ScrollTrigger (industry standard)
**Text splitting:** SplitType, splitting.js
**3D/WebGL:** Three.js, PixiJS, OGL
**Page transitions:** Barba.js, Swup
**Utilities:** IntersectionObserver (native)

**CDN Links:**
```
GSAP: https://cdnjs.cloudflare.com/ajax/libs/gsap/3.12.5/gsap.min.js
ScrollTrigger: https://cdnjs.cloudflare.com/ajax/libs/gsap/3.12.5/ScrollTrigger.min.js
Lenis: https://unpkg.com/lenis@1.1.14/dist/lenis.min.js
Three.js: https://cdnjs.cloudflare.com/ajax/libs/three.js/r128/three.min.js
Barba: https://unpkg.com/@barba/core
```

---

## 2024-2025 TRENDS

**Motion as Expectation:** Animation không còn là bonus - đang trở thành expectation. Từ subtle logo animations đến looping product demos.

**Scroll Storytelling:** Websites như interactive stories, scroll controls narrative progression.

**3D Integration:** WebGL effects ngày càng phổ biến, nhưng subtle integration hơn là full 3D experiences.

**Micro-interactions Everywhere:** Tiny delightful moments ở mọi interaction point.

**Performance First:** Fast, smooth experiences. Heavy effects nhưng optimized well.

**Accessibility Aware:** Motion preferences respected, keyboard navigation, screen reader support.

---

## MỞ RỘNG

Thêm effect mới theo format:

```
### [Tên Effect]
`keyword1` `keyword2` `keyword3`

[Mô tả tự nhiên về effect - cảm giác, behavior, context]

Variations:
- [Variation 1]
- [Variation 2]

Khi nào dùng: [Use cases]
```

AI sẽ tự implement phù hợp với project context.
