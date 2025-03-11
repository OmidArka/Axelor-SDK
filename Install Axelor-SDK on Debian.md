# Axelor Open Suite

**Axelor Open Suite** یک نرم‌افزار جامع **ERP، CRM و مدیریت پروژه** است که برای **اتوماسیون کسب‌وکارها** و **بهینه‌سازی فرآیندهای سازمانی** طراحی شده است. این پلتفرم **متن‌باز** بوده و امکان **سفارشی‌سازی کامل** را فراهم می‌کند.

## ویژگی‌ها
- **مدیریت ارتباط با مشتری (CRM)**: پیگیری سرنخ‌ها، فرصت‌ها و مدیریت ارتباطات.
- **مدیریت پروژه و وظایف**: تعریف پروژه‌ها، وظایف، تعیین مسئولیت‌ها و پیگیری پیشرفت.
- **اتوماسیون فرآیندها**: ایجاد گردش‌کارهای سفارشی برای بهینه‌سازی عملیات سازمانی.
- **مدیریت منابع انسانی**: نظارت بر کارمندان، مرخصی‌ها و حقوق و دستمزد.
- **مدیریت مالی و حسابداری**: صدور فاکتور، کنترل بودجه و حسابداری کامل.
- **پشتیبانی از APIهای REST و GraphQL**: یکپارچه‌سازی آسان با سایر سیستم‌ها.

## نصب و راه‌اندازی در Debian

### پیش‌نیازها
- **Java 11+**
- **Maven 3+**
- **PostgreSQL 12+**
- **Node.js (برای رابط کاربری اختیاری)**

### مراحل نصب
#### 1. به‌روزرسانی بسته‌ها و نصب پیش‌نیازها
```sh
sudo apt update && sudo apt upgrade -y
sudo apt install -y openjdk-11-jdk maven postgresql postgresql-contrib
```

#### 2. پیکربندی PostgreSQL
- وارد محیط PostgreSQL شوید:
```sh
sudo -u postgres psql
```
- ایجاد یک پایگاه داده و کاربر مخصوص Axelor:
```sql
CREATE DATABASE axelor;
CREATE USER axelor WITH ENCRYPTED PASSWORD 'axelor_password';
GRANT ALL PRIVILEGES ON DATABASE axelor TO axelor;
\q
```

#### 3. دریافت کد منبع و ساخت پروژه
```sh
git clone https://github.com/axelor/axelor-open-suite.git
cd axelor-open-suite
mvn clean install
```

#### 4. تنظیمات پایگاه داده در `application.properties`
فایل `src/main/resources/application.properties` را ویرایش کرده و مقدار زیر را تنظیم کنید:
```properties
# تنظیمات پایگاه داده PostgreSQL
db.default.driver=org.postgresql.Driver
db.default.url=jdbc:postgresql://localhost:5432/axelor
db.default.user=axelor
db.default.password=axelor_password
```

#### 5. اجرای نرم‌افزار
```sh
mvn jetty:run
```

#### 6. دسترسی به رابط کاربری
پس از اجرای موفق، می‌توانید نرم‌افزار را از طریق **`http://localhost:8080`** در مرورگر خود مشاهده کنید.

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

## Installation on Debian

### Prerequisites
- **Java 11+**
- **Maven 3+**
- **PostgreSQL 12+**
- **Node.js (optional for UI)**

### Installation Steps
#### 1. Update Packages and Install Dependencies
```sh
sudo apt update && sudo apt upgrade -y
sudo apt install -y openjdk-11-jdk maven postgresql postgresql-contrib
```

#### 2. Configure PostgreSQL
- Access PostgreSQL shell:
```sh
sudo -u postgres psql
```
- Create a database and user for Axelor:
```sql
CREATE DATABASE axelor;
CREATE USER axelor WITH ENCRYPTED PASSWORD 'axelor_password';
GRANT ALL PRIVILEGES ON DATABASE axelor TO axelor;
\q
```

#### 3. Clone the Repository and Build the Project
```sh
git clone https://github.com/axelor/axelor-open-suite.git
cd axelor-open-suite
mvn clean install
```

#### 4. Configure Database in `application.properties`
Edit the file `src/main/resources/application.properties` and set:
```properties
# PostgreSQL Database Settings
db.default.driver=org.postgresql.Driver
db.default.url=jdbc:postgresql://localhost:5432/axelor
db.default.user=axelor
db.default.password=axelor_password
```

#### 5. Run the Application
```sh
mvn jetty:run
```

#### 6. Access the Web Interface
Once successfully running, access the application via **`http://localhost:8080`** in your browser.

## Documentation
For full documentation, visit [Axelor Docs](https://docs.axelor.com).

## Contributing
We welcome contributions! Fork the repository and submit a pull request.

## License
Axelor Open Suite is released under the **GNU Affero General Public License v3.0**. See the LICENSE file for details.
