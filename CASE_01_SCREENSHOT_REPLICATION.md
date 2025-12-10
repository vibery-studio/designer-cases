# SCREENSHOT REPLICATION WORKFLOW

> Replicate design từ screenshot - workflow thực tế, từng bước

---

## NGUYÊN TẮC

1. **Đừng làm hết một lần** - Chia nhỏ, build từng section
2. **Giữ code đã đúng** - Paste lại code cũ mỗi lần yêu cầu section mới
3. **Fix cụ thể** - Chỉ ra chính xác cần sửa gì

---

## WORKFLOW

### Bước 1: Phân tích trước

```
Nhìn screenshot này và liệt kê các sections từ trên xuống.
Mỗi section cho tôi biết: tên, layout chính, elements chính.
Chưa cần code.

[Attach full screenshot]
```

→ Kết quả: Danh sách sections để build

---

### Bước 2: Build từng section

**Section đầu tiên:**

```
Code section [TÊN] này bằng HTML + Tailwind.

[Attach cropped screenshot của section đó]
```

**Các section tiếp theo:**

```
Tiếp tục code section [TÊN].

[Attach cropped screenshot]

Code đã có (giữ nguyên):
[Paste code các sections trước]
```

→ Mỗi section xong, test, rồi mới tiếp section sau

---

### Bước 3: Fix nếu cần

```
Sửa đúng những chỗ này, giữ nguyên phần còn lại:

1. [Mô tả cụ thể vấn đề 1]
2. [Mô tả cụ thể vấn đề 2]

Code hiện tại:
[Paste code]
```

---

## VÍ DỤ THỰC TẾ

**Lần 1:**

```
Nhìn screenshot này, liệt kê sections.
[Full screenshot]
```

**Lần 2:**

```
Code phần Navigation.
[Crop screenshot nav]
```

**Lần 3:**

```
Code phần Hero.
[Crop screenshot hero]

Code đã có:
<nav>...</nav>
```

**Lần 4:**

```
Code phần Features.
[Crop screenshot features]

Code đã có:
<nav>...</nav>
<section class="hero">...</section>
```

**Fix:**

```
Sửa 2 chỗ này:
1. Nav: logo cần to hơn (text-2xl → text-3xl)
2. Hero: button cần rounded hơn

Code:
[paste]
```

---

## TIPS

- **Crop screenshot rõ ràng** - Đúng section, không thừa thiếu
- **Paste code cũ mỗi lần** - Để AI không "quên" và làm hỏng
- **Fix cụ thể** - "Button cần rounded-full" thay vì "button chưa đẹp"
- **Một vài sections/lần** - 2-3 sections đơn giản có thể gộp, phức tạp thì tách

---

## KHI NÀO DÙNG

- Screenshot dài, nhiều sections
- Cần độ chính xác cao
- AI làm hỏng sections khi fix

Nếu screenshot đơn giản (1-2 sections), cứ làm một lần bình thường.

## Khi replicate, chú ý:

### Layout:

- Grid vs Flex vs Position
- Số columns, column widths
- Container max-width
- Element alignment (center, start, end, space-between)
- Stacking order (z-index)

### Spacing:

- Section padding (thường py-16 đến py-24)
- Container padding (px-4 đến px-8)
- Gap giữa elements
- Margin giữa text blocks
- Whitespace tổng thể (tight vs generous)

### Colors:

- Background colors (solid, gradient, image overlay)
- Text colors (heading vs body vs muted)
- Accent colors (buttons, links, highlights)
- Border colors
- Shadow colors và opacity

### Typography:

- Font families (serif vs sans-serif vs mono)
- Heading sizes (thường text-3xl đến text-6xl)
- Body text size (text-base đến text-lg)
- Font weights (normal, medium, semibold, bold)
- Line height (leading-tight, normal, relaxed)
- Letter spacing nếu có
- Text transform (uppercase, capitalize)

### Shapes & Effects:

- Border radius (none, sm, md, lg, full)
- Shadows (sm, md, lg, custom)
- Borders (width, style)
- Blur effects (backdrop-blur)
- Opacity levels

### Images:

- Aspect ratio
- Object-fit (cover, contain)
- Border radius
- Overlays

### Interactive hints:

- Button styles
- Link styles
- Hover states có thể đoán được
