# AWWWARDS INTERACTIONS PRESETS
Hiệu ứng phổ biến trên các website đạt giải - mô tả tự nhiên

---

## Cách dùng file này

Đây là "menu" các effects thường thấy trên Awwwards winners. Mỗi effect được mô tả bằng ngôn ngữ tự nhiên - AI sẽ tự implement phù hợp với context.

**Keywords** được đánh dấu để dễ search và reference.

---

## FOUNDATION

### Smooth Scroll
`lenis` `smooth-scroll` `lerp` `momentum`

Nền tảng của mọi Awwwards website. Scroll mượt như lụa, có momentum và easing tự nhiên. Không có smooth scroll thì mọi effect khác đều mất đi sự premium.

Cảm giác: Như đang lướt trên băng, không phải nhảy từng bước. Scroll dừng lại từ từ thay vì dừng đột ngột.

Thường dùng: Lenis library kết hợp GSAP ScrollTrigger.

---

## TEXT ANIMATIONS

### Line Reveal
`text-reveal` `mask` `overflow-hidden` `stagger` `translateY`

Chữ xuất hiện từng dòng từ dưới lên, như đang được vén màn. Mỗi dòng nằm trong một container có overflow hidden, text translate từ 100% lên 0.

Timing: Stagger 0.1-0.15s giữa các dòng. Ease mạnh ở đầu, nhẹ ở cuối (power4.out).

Khi nào dùng: Headlines, hero text, section titles. Gần như mọi Awwwards site đều có effect này.

---

### Character Reveal
`split-text` `char-animation` `stagger` `3d-rotate`

Từng ký tự xuất hiện riêng lẻ với stagger rất nhỏ. Có thể kèm rotation, blur, hoặc scale. Tạo cảm giác chữ đang "được đánh máy" hoặc "lắp ráp".

Timing: Stagger 0.02-0.05s. Duration ngắn ~0.5s mỗi char.

Variations:
- Fade up từ dưới
- Rotate từ trục X (như lật thẻ)
- Random delay tạo hiệu ứng organic
- Blur to sharp

---

### Text Scramble / Glitch
`scramble` `random-chars` `typewriter` `decode`

Text hiển thị qua giai đoạn "giải mã" - random characters chạy rồi settle vào đúng chữ. Mang vibe tech, hacker, futuristic.

Cảm giác: Như đang decode một message bí mật. Mỗi ký tự nhảy qua vài random chars trước khi đúng.

Khi nào dùng: Tech sites, creative agencies muốn edgy, hover states cho links.

---

### Gradient Text on Scroll
`gradient` `background-clip` `scroll-linked` `opacity-mask`

Text có gradient hoặc opacity thay đổi theo scroll position. Phần đã scroll qua sáng lên, phần chưa tới thì mờ.

Thường dùng cho: Long-form text, manifesto sections, storytelling.

---

### Marquee Text
`marquee` `infinite-scroll` `ticker` `horizontal-loop`

Text chạy liên tục theo một hướng, loop vô tận. Comeback của hiệu ứng 90s nhưng với typography đẹp hơn.

Variations:
- Chạy liên tục (như ticker)
- Chỉ chạy khi hover
- Đổi hướng khi scroll lên/xuống
- Tốc độ thay đổi theo scroll velocity

Khi nào dùng: Dividers giữa sections, footer, showcase text, brand statements.

---

## SCROLL EFFECTS

### Parallax Layers
`parallax` `depth` `z-layers` `scroll-speed`

Các elements di chuyển với tốc độ khác nhau khi scroll, tạo cảm giác depth 3D. Layer gần scroll nhanh, layer xa scroll chậm.

Intensity: Subtle (-10% đến -30%) cho elegant, dramatic (-50% trở lên) cho impact.

Tip: Background images parallax nhẹ, decorative elements parallax mạnh hơn.

---

### Horizontal Scroll Section
`horizontal-scroll` `pin` `scrub` `scroll-hijack`

Scroll dọc bình thường, nhưng có một section mà khi tới thì content chạy ngang. Section được pin lại, scroll dọc được convert thành chuyển động ngang.

Cảm giác: Như đang xem slideshow được điều khiển bằng scroll. Cinematic.

Khi nào dùng: Project showcases, image galleries, timeline, feature tours.

Warning: Dùng có chừng mực. Quá nhiều scroll hijacking làm user frustrated.

---

### Pin & Reveal
`pin` `sticky` `progressive-reveal` `scroll-timeline`

Section được pin/sticky, content bên trong reveal dần theo scroll progress. Có thể là text xuất hiện, images fade in, hoặc elements animate vào vị trí.

Variations:
- Stacked cards reveal từng cái
- Text paragraphs highlight lần lượt  
- Before/after comparison
- Step-by-step storytelling

---

### Scale on Scroll
`zoom` `scale` `scroll-linked` `hero-zoom`

Element (thường là image hoặc video) zoom in hoặc zoom out theo scroll. Tạo cảm giác "dive into" content.

Common uses:
- Hero image zoom out khi scroll xuống (reveal more)
- Image zoom in khi approach (focus attention)
- Full-page zoom transition giữa sections

---

### Clip-path Reveal
`clip-path` `mask` `wipe` `reveal-animation`

Content được reveal bằng cách animate clip-path - như một cửa sổ mở ra. Có thể từ bất kỳ hướng nào hoặc từ center ra.

Shapes phổ biến:
- Inset (rectangular wipe)
- Circle (từ center expand ra)
- Polygon (creative shapes)

Khi nào dùng: Image reveals, section transitions, hero entrances.

---

### Sticky Footer Reveal
`sticky-footer` `clip-path` `z-index` `reveal-underneath`

Content scroll đi và reveal footer ở phía dưới - như đang lật một trang giấy. Footer luôn ở đó, chỉ bị che bởi content.

Cảm giác: Surprising, elegant ending. Footer feels "discovered" không phải "reached".

---

## HOVER & CURSOR

### Magnetic Elements
`magnetic` `cursor-follow` `attraction` `elastic`

Button hoặc element bị "hút" về phía cursor khi hover gần. Tạo cảm giác interactive, alive.

Physics: Element follow cursor với lerp/easing. Khi leave, snap back với elastic bounce.

Khi nào dùng: CTAs, navigation items, interactive elements muốn draw attention.

---

### Custom Cursor
`custom-cursor` `cursor-follow` `cursor-blend` `cursor-scale`

Thay thế cursor mặc định bằng custom element. Có thể thay đổi size, shape, color, blend mode tùy theo element đang hover.

Variations:
- Dot nhỏ + circle lớn follow với delay
- Text cursor ("View", "Play", "Drag")
- Blend mode (difference) để luôn visible
- Scale up khi hover clickable elements
- Morph shape theo context

---

### Image Reveal on Hover
`hover-reveal` `clip-path` `mask-animation` `image-wipe`

Image ẩn, khi hover thì reveal bằng animation. Thường dùng clip-path hoặc một overlay element animate đi.

Variations:
- Wipe từ một cạnh
- Expand từ center
- Diagonal reveal
- Blur to sharp

---

### Link Hover - Underline Animation
`underline` `hover` `scaleX` `draw-line`

Underline không chỉ appear/disappear mà animate - grow từ trái, từ giữa, hoặc draw như đang vẽ.

Patterns phổ biến:
- Grow từ left to right
- Grow từ center ra hai bên
- Existing underline slide out, new one slide in
- Thickness change
- Color transition

---

### Menu Item Hover - Marquee
`menu-hover` `marquee` `text-loop` `overflow-scroll`

Khi hover vào menu item, text bắt đầu scroll/marquee trong container của nó. Rất signature Awwwards effect.

---

### Image Hover - Zoom & Pan
`hover-zoom` `overflow-hidden` `scale` `parallax-hover`

Image zoom in nhẹ khi hover, có thể kèm subtle pan theo cursor position. Container overflow hidden để crop.

---

## PAGE TRANSITIONS

### Fade Through
`page-transition` `fade` `opacity` `crossfade`

Simple nhất: Page cũ fade out, page mới fade in. Có thể có slight overlap (crossfade) hoặc fade to color rồi fade in.

---

### Slide / Wipe
`slide-transition` `translateX` `wipe` `directional`

Page slide ra một hướng, page mới slide vào từ hướng ngược lại. Có thể kết hợp với slight scale.

---

### Expand from Element
`zoom-transition` `expand` `morph` `shared-element`

Click vào element (card, image), element đó expand ra full screen và morph thành page mới. Very smooth, very impressive.

Còn gọi là: Shared element transition, FLIP animation.

---

### Curtain / Overlay
`curtain` `overlay` `reveal` `theatrical`

Một layer (màu solid, gradient, hoặc pattern) cover screen, rồi reveal page mới. Theatrical, dramatic.

---

## MICRO-INTERACTIONS

### Button Press
`button-active` `press-down` `tactile` `feedback`

Khi click button, có visual feedback như đang nhấn xuống - translateY xuống một chút, shadow giảm. Release thì bounce back.

---

### Form Focus
`input-focus` `label-float` `border-animation` `underline-grow`

Input khi focus có animation: label float lên, border highlight, underline grow từ center.

---

### Loading States
`skeleton` `shimmer` `pulse` `progress`

Trong khi loading: skeleton screens với shimmer effect, hoặc subtle pulse animation cho placeholders.

---

### Toggle / Switch
`toggle` `morph` `state-change` `smooth-transition`

Toggle switches với smooth animation giữa states. Có thể morph shape, change color, move indicator.

---

## CREATIVE / ADVANCED

### Image Distortion
`webgl` `distortion` `displacement` `wave`

Image bị distort khi hover hoặc scroll - wave effect, displacement, RGB split. Cần WebGL/Three.js hoặc CSS filters.

---

### 3D Card Tilt
`perspective` `rotateX` `rotateY` `mouse-position`

Card tilt theo mouse position, tạo cảm giác 3D. Có thể kèm reflection, shadow movement.

---

### Particle Systems
`particles` `canvas` `generative` `interactive`

Background hoặc decorative particles react to cursor hoặc scroll. Có thể là dots, lines, shapes.

---

### Morphing Shapes
`svg-morph` `blob` `organic` `fluid`

Shapes (blobs, abstract forms) morph liên tục hoặc khi triggered. Tạo cảm giác organic, alive.

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
- Transitions: Crossfade, wipe

**Tech/Futuristic:**
- Text: Scramble, glitch effects
- Scroll: 3D transforms, clip-path
- Hover: Custom cursor, distortion
- Transitions: Geometric wipes

### Theo Content

**Portfolio:** Image reveals, project hovers với preview, smooth transitions
**Agency:** Bold scroll effects, creative cursors, impressive page transitions
**E-commerce:** Subtle hovers, quick transitions, micro-interactions for UX
**Editorial:** Text-focused effects, reading progress, parallax images

---

## PERFORMANCE NOTES

**Animate only:**
- transform (translate, scale, rotate)
- opacity
- clip-path (modern browsers)

**Avoid animating:**
- width, height
- margin, padding
- top, left
- box-shadow (fake with pseudo-element)

**Best practices:**
- Use `will-change` sparingly
- Throttle scroll/mouse events
- Prefer CSS transitions for simple effects
- Use GSAP for complex choreography
- Test trên mid-range devices
- Provide `prefers-reduced-motion` fallback

---

## LIBRARIES REFERENCE

- **Smooth scroll:** Lenis, Locomotive Scroll
- **Animation:** GSAP + ScrollTrigger (industry standard)
- **Text splitting:** SplitText (GSAP), splitting.js
- **3D/WebGL:** Three.js, PixiJS, OGL
- **Page transitions:** Barba.js, Swup
- **Utilities:** IntersectionObserver (native)
