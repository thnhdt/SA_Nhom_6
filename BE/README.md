
## 🛠 Công nghệ sử dụng (Tech Stack)

* **Ngôn ngữ:** Java (JDK 25)
* **Framework:** Spring Boot 4.0.5
* **Quản lý thư viện:** Maven

---

## 📂 Cấu trúc dự án (Project Structure)

[cite_start]Dự án áp dụng kiến trúc 4 tầng riêng biệt để đảm bảo tính module hóa và dễ bảo trì[cite: 37, 42]:

```text
src/main/java/com/irms/orderingservice/
│
├── presentation/      # Tầng 1: Chứa các REST Controller tiếp nhận HTTP Request từ API Gateway/Tablet.
├── service/           # Tầng 2: Chứa Business Logic (Quy tắc nghiệp vụ của hệ thống).
├── persistence/       # Tầng 3: Chứa các Interface giao tiếp dữ liệu (Repository) và DTOs.
├── database/          # Tầng 4: Chứa các Entity (JPA) và triển khai kết nối Database thực tế.
│
└── OrderingServiceApplication.java  # File khởi chạy chính của Spring Boot
```

## Chạy source
./mvnw spring-boot:run