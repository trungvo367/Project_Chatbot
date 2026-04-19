# Project_Chatbot
# 🤖 AI Travel Guide Chatbot - Smart Trip Planner

Dự án xây dựng hệ thống Chatbot hướng dẫn du lịch thông minh, có khả năng tự động lập lịch trình chi tiết dựa trên nhu cầu cá nhân của người dùng bằng cách kết hợp sức mạnh của **Large Language Models (LLMs)** và dữ liệu thực tế (**RAG**).

## 🌟 Ý tưởng cốt lõi
Hệ thống nhận các tham số đầu vào (Input) cụ thể để xuất ra một kế hoạch du lịch (Output) toàn diện, tối ưu hóa theo ngân sách và sở thích cá nhân.

### 📥 Input (Yêu cầu người dùng)
* **Loại hình:** Thắng cảnh, tâm linh, biển, sông nước, khu du lịch, trong nước/ngoài nước...
* **Thời gian:** 1 ngày, 2 ngày 1 đêm, 1 tuần...
* **Ngân sách:** 1 triệu, 10 triệu, 50 triệu...
* **Số lượng:** Đi đơn lẻ, cặp đôi, gia đình hoặc nhóm bạn.
* **Sở thích:** Ẩm thực, yên tĩnh, náo nhiệt, trải nghiệm văn hóa bản địa.

### 📤 Output (Lịch trình dự kiến)
* **Danh sách:** Địa điểm tham quan, lưu trú (Khách sạn/Homestay), ăn uống.
* **Chi tiết tài chính:** Ước tính chi phí cho từng hạng mục để khớp với ngân sách tổng.
* **Thời gian biểu:** Lịch trình chi tiết từng mốc giờ (Timeline).
* **Kiến thức bản địa:** Cung cấp thông tin về văn hóa, con người và lịch sử tại điểm đến.

---

## 🏗 Kiến trúc hệ thống (Tech Stack)
Dự án được triển khai trên nền tảng Python, tối ưu cho việc chạy nội bộ (Local) để đảm bảo tốc độ và bảo mật:

* **Bộ não (LLM):** `Qwen2.5-0.5B` hoặc `1.5B` chạy qua **Ollama**.
* **Kỹ thuật xử lý:** **RAG (Retrieval-Augmented Generation)** để truy xuất dữ liệu du lịch chính xác.
* **Cơ sở dữ liệu:** **MongoDB** lưu trữ thông tin địa điểm, giá vé và đánh giá.
* **Ngôn ngữ:** **Python** (Sử dụng thư viện LangChain để kết nối dữ liệu và AI).

---

## 📝 Ví dụ kịch bản (Use Case)
**Yêu cầu:** 2 ngày 1 đêm tại Cần Thơ - Ngân sách 1.5 triệu - Sở thích: Sông nước, Ẩm thực.

**Kết quả từ Chatbot:**
* **05:30:** Tham quan Chợ nổi Cái Răng (Chi phí: 150k tàu). *Kiến thức: Tìm hiểu văn hóa giao thương trên sông.*
* **08:00:** Ăn sáng hủ tiếu (Chi phí: 50k).
* **12:00:** Check-in Homestay ven sông (Chi phí: 400k/đêm).
* ... (Lịch trình tiếp tục cho đến khi kết thúc chuyến đi)





© 2026 - Nhóm Phát Triển Chatbot AI - CTU
