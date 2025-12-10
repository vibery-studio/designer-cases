# INTERACTIONS PRESETS
Animation & interaction patterns - apply sau khi layout đã chuẩn

---

## Cách dùng

File này là "menu" các interaction patterns. Khi layout đã xong, chọn và apply những patterns phù hợp với design.

**Không cần dùng hết.** Một trang subtle có thể chỉ cần hover states. Một trang impressive có thể layer nhiều effects.

**Rule of thumb:** Ít mà tốt hơn nhiều mà loạn. Một scroll animation đẹp ấn tượng hơn 10 effects random.

---

## HOVER STATES

### Subtle (cho minimal designs)

**Opacity fade**
Text hoặc element giảm nhẹ opacity khi chưa hover, full opacity khi hover. Ngược lại với thông thường - tạo cảm giác "activate".

**Underline grow**
Underline bắt đầu từ giữa (hoặc trái) và grow ra khi hover. Không xuất hiện đột ngột.

**Color shift**
Màu chuyển nhẹ - có thể là đậm hơn, nhạt hơn, hoặc shift sang accent color. Transition mượt.

**Letter-spacing breathe**
Text hơi nới rộng letter-spacing khi hover. Rất subtle, chỉ vài pixel. Tạo cảm giác "mở ra".

### Standard (cho hầu hết designs)

**Lift & shadow**
Element nâng lên nhẹ (translateY -2 đến -4px) và shadow đậm/lan rộng hơn. Classic và hiệu quả.

**Background fill**
Background color fill từ một góc hoặc từ dưới lên. Có thể dùng pseudo-element với transform scale.

**Border appear**
Border fade in hoặc draw từ một góc. Tạo cảm giác "select".

**Icon animate**
Icon bên cạnh text có thể: arrow di chuyển sang phải, plus xoay thành x, hoặc subtle bounce.

### Bold (cho expressive designs)

**Scale pop**
Element scale lên 1.02-1.05. Nhanh và snappy, không slow motion.

**Tilt/rotate**
Xoay nhẹ 1-3 độ. Tạo cảm giác playful, physical.

**Color invert**
Background và text swap màu. Dramatic nhưng clear.

**Glitch flash**
RGB split hoặc position jitter nhanh. Chỉ cho edgy designs.

---

## SCROLL ANIMATIONS

### Entrance effects (elements xuất hiện khi scroll tới)

**Fade in**
Đơn giản nhất. Opacity 0 → 1. Có thể kết hợp với slight movement.

**Rise up**
Bắt đầu thấp hơn vị trí cuối ~20-30px, di chuyển lên trong khi fade in. Classic, elegant.

**Slide from side**
Từ trái hoặc phải. Dùng cho elements muốn nhấn mạnh direction hoặc asymmetric layouts.

**Scale in**
Bắt đầu nhỏ hơn (0.95-0.98), scale lên full size. Subtle zoom effect.

**Blur to sharp**
Bắt đầu hơi blur, transition sang sharp. Tạo cảm giác "focus".

### Stagger patterns (nhiều elements xuất hiện)

**Sequential**
Element 1, rồi element 2, rồi element 3... Delay đều nhau (0.1-0.15s between).

**Cascade**
Grid items xuất hiện theo wave - từ trên xuống hoặc từ góc ra. Delay tính theo vị trí.

**Random scatter**
Mỗi element có random delay nhỏ. Tạo cảm giác organic, less robotic.

### Continuous scroll effects

**Parallax layers**
Background và foreground di chuyển khác tốc độ. Tạo depth. Đừng quá aggressive - subtle là đẹp.

**Sticky sections**
Section pin lại trong khi content bên trong animate. Dùng cho storytelling, reveals.

**Progress-linked**
Animation progress tied to scroll position. Có thể là: image sequence, drawing SVG, counter tăng...

**Horizontal scroll**
Một section scroll ngang trong khi page scroll dọc. Eye-catching nhưng cần clear affordance.

---

## PAGE TRANSITIONS

### Load effects (khi page mới load)

**Curtain reveal**
Một layer che phủ, sau đó slide/fade đi để reveal content. Theatrical.

**Content cascade**
Hero xuất hiện trước, rồi nav, rồi các elements khác stagger vào. Natural, không overwhelming.

**Logo morph**
Logo hoặc brand element animate từ center ra, rồi settle vào vị trí. Branded experience.

**Blur in**
Toàn trang bắt đầu blur, quickly sharpen. Fast - không quá 0.5s.

### Between pages (nếu SPA hoặc có transitions)

**Fade through**
Page cũ fade out, page mới fade in. Safe, smooth.

**Slide**
Page cũ slide ra, page mới slide vào. Directional, good for flows.

**Zoom**
Click vào element, element zoom to full screen và morph thành page mới. Dramatic, cần execution tốt.

**Shared element**
Một element (image, card) morph từ vị trí cũ sang vị trí mới ở page tiếp. Smooth, connected.

---

## MICRO-INTERACTIONS

### Buttons

**Press down**
Khi click (active state), button nhấn xuống nhẹ và shadow giảm. Physical feedback.

**Ripple**
Material design style - ripple effect từ điểm click lan ra. Familiar, satisfying.

**Loading state**
Text đổi thành spinner hoặc dots animation. User knows something is happening.

**Success state**
Sau submit, button có thể: đổi màu xanh, icon check xuất hiện, text đổi thành "Done!".

### Forms

**Label float**
Label ở trong input, float lên trên khi focus hoặc có value. Space-efficient.

**Shake on error**
Input shake ngang khi validation fail. Clear error signal.

**Border/underline animate**
Border hoặc underline grow từ center hoặc từ trái khi focus.

**Character counter**
Counter đếm characters, có thể đổi màu khi gần limit.

### Cards/Items

**Expand preview**
Hover hoặc click để card expand và show thêm info. Có thể inline hoặc modal.

**Flip**
Card flip để show mặt sau với info khác. Playful, good for profiles hoặc features.

**Stack peek**
Trong một stack, cards peek out để hint có nhiều items.

### Navigation

**Menu slide**
Mobile menu slide từ bên hoặc từ trên. Content chính có thể push hoặc overlay.

**Hamburger morph**
3 lines morph thành X khi open. Satisfying, clear state.

**Active indicator**
Indicator (dot, line, background) animate giữa menu items khi switch.

**Scroll progress**
Line ở top of page grow để indicate scroll progress.

---

## MATCHING GUIDE

### Theo design vibe

**Minimal/Clean:**
- Hover: Subtle (opacity, underline grow)
- Scroll: Fade in, gentle rise
- Transitions: Simple fades
- Micro: Minimal, functional only

**Modern/Startup:**
- Hover: Standard (lift & shadow, background fill)
- Scroll: Rise up with stagger
- Transitions: Content cascade
- Micro: Smooth, polished

**Bold/Creative:**
- Hover: Bold (scale, tilt, color invert)
- Scroll: Mix of effects, parallax
- Transitions: Dramatic reveals
- Micro: Playful, surprising

**Editorial/Luxury:**
- Hover: Elegant (slow transitions, refined movement)
- Scroll: Smooth parallax, sticky storytelling
- Transitions: Theatrical, intentional
- Micro: Restrained but perfect

**Playful/Fun:**
- Hover: Bouncy, wiggly, colorful
- Scroll: Scatter, random delays
- Transitions: Energetic
- Micro: Easter eggs, surprises

### Theo content type

**Portfolio:** Scroll reveals for projects, smooth image transitions, subtle UI
**Landing page:** Hero animation, scroll storytelling, CTA emphasis
**Blog/Content:** Minimal, focus on readability, subtle scroll progress
**App showcase:** Device mockup animations, feature reveals, interactive demos
**Agency site:** Impressive effects, creative transitions, memorable moments

---

## PERFORMANCE NOTES

**Animate these (cheap):**
- transform (translate, scale, rotate)
- opacity

**Avoid animating (expensive):**
- width, height
- top, left, right, bottom
- margin, padding
- box-shadow (có thể fake bằng pseudo-element)

**General rules:**
- Dùng `will-change` cho elements animate nhiều
- Throttle scroll events
- Use Intersection Observer thay vì scroll listener
- Test trên mid-range devices
- Cung cấp `prefers-reduced-motion` fallback

---

## IMPLEMENTATION HINTS

Đây là hints, không phải code để copy. AI nên tự implement phù hợp với context.

**Scroll trigger:** Intersection Observer là standard. Threshold 0.1-0.2 để trigger sớm một chút.

**Stagger:** CSS animation-delay hoặc JS loop với setTimeout. Gap 0.1-0.15s feels natural.

**Parallax:** Transform translateY dựa trên scroll position. Factor 0.1-0.3 cho subtle, 0.5+ cho dramatic.

**Smooth scroll:** CSS `scroll-behavior: smooth` hoặc library như Lenis cho buttery smooth.

**Page transitions:** Có thể fake với CSS nếu không phải SPA. Real transitions cần Barba.js hoặc tương tự.

---

## QUICK REFERENCE

Chọn nhanh dựa trên yêu cầu:

**"Cần subtle/professional"**
→ Hover: opacity, underline. Scroll: fade in. No fancy stuff.

**"Cần modern/polished"**
→ Hover: lift & shadow. Scroll: rise up + stagger. Load: content cascade.

**"Cần impressive/wow"**
→ Layer nhiều effects. Parallax. Sticky sections. Custom transitions.

**"Cần playful/fun"**
→ Bouncy easings. Wobble/wiggle. Bright colors on hover. Easter eggs.

**"Cần fast/performant"**
→ Chỉ opacity và transform. Minimal JS. No parallax on mobile.
