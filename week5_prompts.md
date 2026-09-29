# AI Prompts Used - Week 5 (Refactoring Performance & Animations)

This file documents the AI prompts and instructions used to generate and optimize the CSS animations for the Week 5 assignment.

## Objective:
Enhance the portfolio with performant animations adhering to the 6 homework exercises. 

## Prompts & AI Directives:

1. **Floating Action Button (Pulse Effect):**
   *Prompt:* "Nút tròn 'Liên hệ' cố định góc màn hình với pulse animation phập phồng thu hút sự chú ý. Tối ưu hiệu năng bằng box-shadow và transform."

2. **Card Flip Effect:**
   *Prompt:* "Thẻ nhân sự lật rotateY(180deg) khi hover để hiện thông tin liên hệ ở mặt sau. Sử dụng `preserve-3d` và `backface-visibility`."

3. **Typing Effect:**
   *Prompt:* "Chữ tự gõ 'Tôi là một Web Developer...' bằng CSS thuần — không dùng JavaScript. Dùng `steps()` và `overflow: hidden`."

4. **Parallax Image:**
   *Prompt:* "Banner với ảnh nền di chuyển chậm hơn nội dung khi cuộn — dùng `background-attachment: fixed`."

5. **Hamburger Menu (X toggle):**
   *Prompt:* "Biến đổi 3 gạch ngang thành dấu 'X' mượt mà bằng CSS Transitions khi mở menu mobile."

6. **Skill Bar Animation:**
   *Prompt:* "Thanh kỹ năng (HTML 90%, CSS 85%...) chạy từ 0% đến giá trị đích khi trang tải xong. Animation phải chạy mượt mà theo `cubic-bezier`."

7. **Performance Optimization Guidance:**
   *User Provided Concept:* "Thay đổi top/left kích hoạt Layout Reflow... Transform và opacity được GPU xử lý riêng — không gây Reflow, không gây Repaint."
   *AI Action Taken:* Configured all hover animations and loading spinners to rely strictly on `transform` (`translateY`, `scale`, `rotateY`) and `opacity` to avoid layout reflows, ensuring maximum 60FPS performance on low-end devices.

## Requirements Checked Off:
- [x] All 6 homework activities completed.
- [x] No `margin`, `top`, or `left` used for animation. Exclusively used `transform` and `opacity`.
- [x] Includes Hover (Card Flip, FAB hover), Keyframes (Typing, Skill bars, FAB Pulse), and Scroll (AOS animations).
- [x] Prompts logged in `week5_prompts.md`.
- [x] Code pushed to `feature/animations` branch.
