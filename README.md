# Axelor Open Suite

**Axelor Open Suite** یک نرم‌افزار جامع **ERP، CRM و مدیریت پروژه** است که برای **اتوماسیون کسب‌وکارها** و **بهینه‌سازی فرآیندهای سازمانی** طراحی شده است. این پلتفرم **متن‌باز** بوده و امکان **سفارشی‌سازی کامل** را فراهم می‌کند.

## ویژگی‌ها
- **مدیریت ارتباط با مشتری (CRM)**: پیگیری سرنخ‌ها، فرصت‌ها و مدیریت ارتباطات.
- **مدیریت پروژه و وظایف**: تعریف پروژه‌ها، وظایف، تعیین مسئولیت‌ها و پیگیری پیشرفت.
- **اتوماسیون فرآیندها**: ایجاد گردش‌کارهای سفارشی برای بهینه‌سازی عملیات سازمانی.
- **مدیریت منابع انسانی**: نظارت بر کارمندان، مرخصی‌ها و حقوق و دستمزد.
- **مدیریت مالی و حسابداری**: صدور فاکتور، کنترل بودجه و حسابداری کامل.
- **پشتیبانی از APIهای REST و GraphQL**: یکپارچه‌سازی آسان با سایر سیستم‌ها.

## نصب و راه‌اندازی

### پیش‌نیازها
- **Java 11+**
- **Maven 3+**
- **PostgreSQL 12+**
- **Docker (اختیاری، برای استقرار در محیط کانتینری)**

### مراحل نصب
1. دریافت کد منبع Axelor Open Suite:
   ```sh
   git clone https://github.com/axelor/axelor-open-suite.git
   cd axelor-open-suite
   ```
2. ساخت پروژه:
   ```sh
   mvn clean install
   ```
3. اجرای نرم‌افزار:
   ```sh
   mvn jetty:run
   ```
4. مرورگر خود را باز کرده و به آدرس `http://localhost:8080` بروید.

## نحوه استفاده
- **مدیریت پروژه**: ایجاد و پیگیری پروژه‌ها و وظایف با قابلیت تخصیص منابع.
- **CRM و فروش**: پیگیری مشتریان، صدور فاکتور و پیش‌بینی فروش.
- **حسابداری و مالی**: مدیریت فاکتورها، هزینه‌ها و صورت‌حساب‌ها.
- **منابع انسانی**: مدیریت کارکنان، حقوق و مزایا.

## مستندات
برای مطالعه مستندات کامل، به [مستندات Axelor](https://docs.axelor.com) مراجعه کنید.

## مشارکت در توسعه
مشارکت شما در توسعه این ابزار ارزشمند است! برای همکاری، مخزن را **Fork** کرده و درخواست **Pull Request** ارسال کنید.

## مجوز
Axelor Open Suite تحت **مجوز GNU Affero General Public License v3.0** منتشر شده است. برای جزئیات بیشتر، به فایل LICENSE مراجعه کنید.

---

# Axelor Open Suite (English)

**Axelor Open Suite** is a comprehensive **ERP, CRM, and project management software** designed for **business process automation** and **enterprise optimization**. It is an **open-source** platform with **full customization capabilities**.

## Features
- **Customer Relationship Management (CRM)**: Track leads, opportunities, and manage interactions.
- **Project & Task Management**: Define projects, assign tasks, and monitor progress.
- **Process Automation**: Create custom workflows to optimize business operations.
- **Human Resource Management**: Monitor employees, leaves, and payroll.
- **Financial & Accounting Management**: Invoice management, budget control, and full accounting.
- **REST & GraphQL APIs**: Easy integration with other systems.

## Installation & Setup

### Prerequisites
- **Java 11+**
- **Maven 3+**
- **PostgreSQL 12+**
- **Docker (optional, for containerized deployment)**

### Setup Steps
1. Clone the Axelor Open Suite repository:
   ```sh
   git clone https://github.com/axelor/axelor-open-suite.git
   cd axelor-open-suite
   ```
2. Build the project:
   ```sh
   mvn clean install
   ```
3. Run the application:
   ```sh
   mvn jetty:run
   ```
4. Open `http://localhost:8080` in your browser.

## Usage
- **Project Management**: Create and track projects and tasks with resource allocation.
- **CRM & Sales**: Track customers, issue invoices, and forecast sales.
- **Accounting & Finance**: Manage invoices, expenses, and financial statements.
- **HR Management**: Handle employee data, payroll, and benefits.

## Documentation
For detailed documentation, visit [Axelor Docs](https://docs.axelor.com).

## Contributing
We welcome contributions! Fork the repository and submit a pull request.

## License
Axelor Open Suite is released under the **GNU Affero General Public License v3.0**. See the LICENSE file for details.
