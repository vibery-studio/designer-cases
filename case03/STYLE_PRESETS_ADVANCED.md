# STYLE PRESETS: ADVANCED EFFECTS
Extension pack cho designers muốn portfolio thật ấn tượng

---

## Khi nào dùng pack này?

- User nói muốn "ấn tượng", "wow", "khác biệt", "creative developer"
- Target audience là creative agencies, design studios, tech companies đánh giá cao craft
- User có background front-end hoặc muốn thể hiện technical skill
- Portfolio cho roles như: Creative Technologist, Design Engineer, Interactive Designer

**Lưu ý:** Effects ấn tượng cần đánh đổi:
- Load time chậm hơn
- Cần external libraries (Three.js, GSAP, P5.js)
- Mobile experience có thể khác desktop
- Không phải recruiter nào cũng appreciate

---

## IMMERSIVE STYLES

### P. Particle Universe
Không gian 3D với particles bay lơ lửng. Khi scroll, như đang di chuyển qua vũ trụ. Mouse tương tác với particles - đẩy ra hoặc hút vào. Màu sắc deep space - navy đậm, tím galaxy, điểm sáng như sao. Typography floating trong không gian.

Hero section là một canvas Three.js full-screen. Content xuất hiện như đang emerge từ darkness. Projects như những constellation - hover vào thì particles tụ lại thành hình.

**Vibe:** Interstellar gặp Apple keynote
**Best for:** Creative technologists, những người muốn flex technical skill
**Key moments:** First load (particles form từ chaos), scroll transitions, project hover states

### Q. Liquid Morph
Mọi thứ đều fluid. Shapes morph liên tục. Blobs chảy vào nhau. Cursor để lại trail như kéo qua chất lỏng. Transitions không bao giờ sharp - luôn melt, flow, transform.

Color palette organic - gradients chuyển màu như dầu loang trên nước. Có thể dùng WebGL shader cho liquid distortion effect. Text có thể wave nhẹ như đang nổi trên mặt nước.

**Vibe:** Lava lamp gặp high-end fragrance website
**Best for:** Motion designers, brand designers, những người làm việc với luxury/beauty
**Key moments:** Page transitions (liquid wipe), hover distortions, scroll-triggered morphs

### R. Kinetic Typography
Text là nhân vật chính và nó SỐNG. Characters split ra rồi reassemble. Words cascade như thác. Scroll trigger text animations phức tạp - mỗi section có choreography riêng.

Có thể kết hợp: text reveal từng character, text following cursor, text reacting to scroll velocity, parallax layers của text. Background minimal để typography shine.

**Vibe:** Typography poster của David Carson animate lên
**Best for:** Type designers, brand designers, motion graphics people
**Key moments:** Hero text entrance, section transitions, name/title animations

### S. Dimensional Layers  
Parallax on steroids. Không chỉ 2-3 layers mà 5-7 layers depth. Mouse movement tạo perspective shift như đang nhìn qua cửa sổ vào một thế giới khác. Scroll tạo cảm giác đang dive deeper.

Elements có shadows cực kỳ realistic - soft, multiple light sources. Cards tilt theo mouse như đang cầm physical object. Depth of field blur cho layers xa.

**Vibe:** iOS parallax wallpaper gặp diorama 3D
**Best for:** UI designers muốn show depth understanding, product designers
**Key moments:** Initial load (layers settle vào vị trí), mouse parallax, scroll depth

### T. Glitch Reality
Digital artifacts có chủ đích. RGB split. Scan lines. Random glitches khi interact. Nhưng controlled chaos - không phải broken, mà là aesthetic choice.

Có thể combine: datamosh effects on images, text glitch on hover, screen tear transitions, noise grain overlay. Color palette có thể cyberpunk hoặc monochrome với accent neon.

**Vibe:** Mr. Robot credits gặp 90s VHS
**Best for:** Edgy creative roles, gaming industry, những người không muốn "safe"
**Key moments:** Transitions between sections, hover states, idle animations (random glitches)

### U. Scroll Cinema
Portfolio như một bộ phim. Scroll controls timeline. Mỗi scroll tick là một frame. Elements animate in/out như scene transitions. Có thể có horizontal sections break vertical flow.

Progress indicator như film reel hoặc timeline. Sections có thể pin và animate through trước khi release. Video backgrounds, cinemagraphs. Widescreen aspect ratio cho images.

**Vibe:** Interactive documentary, Apple product page storytelling
**Best for:** Video/motion designers, storytellers, những người có strong narrative
**Key moments:** Section pins với micro-animations, video sync với scroll, finale sequence

### V. Generative Canvas
Background là một generative art piece - luôn unique, luôn moving. P5.js hoặc canvas API. Có thể là: flow field, particle system, cellular automata, perlin noise landscape.

Art responds to user - mouse position affects parameters, scroll changes color/speed/density. Mỗi visit là experience khác nhau. Screenshots sẽ luôn unique.

**Vibe:** Creative coding exhibition, digital art gallery
**Best for:** Creative coders, generative artists, experimental designers
**Key moments:** Mọi lúc - canvas luôn living, luôn có gì đó để nhìn

### W. Physics Playground  
Elements có physics. Drag and drop. Gravity. Bounce. Collision. Portfolio như một sandbox - visitor có thể tương tác, xáo trộn, play around.

Project cards có thể được kéo thả. Scroll có momentum và bounce. Easter eggs khi interact đủ nhiều. Có thể có hidden games hoặc interactions.

**Vibe:** Beaker app gặp creative portfolio
**Best for:** Interaction designers, game designers, playful personalities
**Key moments:** First interaction (discover things are draggable), physics surprises, easter eggs

---

## COMBINATION IDEAS

Có thể mix elements từ các styles:

- **Particle Universe + Kinetic Typography:** Text formed bởi particles
- **Liquid Morph + Dimensional Layers:** Layers với liquid transitions
- **Glitch Reality + Scroll Cinema:** Cinematic với glitch transitions
- **Generative Canvas + Physics:** Interactive generative background

---

## TECHNICAL NOTES (cho AI reference)

**Libraries phổ biến:**
- Three.js: 3D, particles, shaders
- GSAP + ScrollTrigger: Scroll animations, timelines
- P5.js: Generative art, creative coding
- Matter.js: Physics simulations
- Lenis/Locomotive: Smooth scroll
- PixiJS: 2D WebGL effects

**Performance considerations:**
- Throttle mouse events
- Use requestAnimationFrame
- Lazy load heavy sections  
- Provide reduced-motion fallback
- Test on mid-range devices

**Mobile adaptations:**
- Simplify hoặc disable complex effects
- Touch-friendly interactions
- Gyroscope thay cho mouse parallax
- Battery/performance conscious

---

## MATCHING GUIDE

Chọn style dựa trên:

**Technical comfort của user:**
- Biết code → Full effects OK
- Designer only → Cần simple deploy, maybe simpler effects

**Target audience:**
- Creative agencies → Go wild
- Corporate → Tone down, focus subtle polish
- Startups → Balance impressive + practical

**Content type:**
- Heavy visuals/videos → Scroll Cinema, Liquid Morph
- Typography focused → Kinetic Typography
- Conceptual/abstract → Generative Canvas, Particle Universe
- Playful personality → Physics Playground

**Muốn người xem nhớ điều gì?**
- Technical skill → Particle Universe, Generative Canvas
- Motion/animation skill → Liquid Morph, Kinetic Typography
- Attention to detail → Dimensional Layers
- Unique personality → Glitch Reality, Physics Playground
