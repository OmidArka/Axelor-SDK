# Axelor SDK


Axelor SDK یک کیت توسعه نرم‌افزاری است که برای ساخت برنامه‌های سازمانی بر پایه **Axelor Open Platform** طراحی شده است. این ابزار یک محیط توسعه یکپارچه برای ایجاد، تست و استقرار برنامه‌های اکسلور فراهم می‌کند.

## ویژگی‌ها
- **محیط توسعه یکپارچه (IDE)**: محیطی از پیش پیکربندی شده برای توسعه برنامه‌های اکسلور.
- **تولید کد خودکار**: کاهش وظایف تکراری برنامه‌نویسی.
- **بارگذاری آنی (Hot Reloading)**: مشاهده تغییرات به‌صورت لحظه‌ای بدون نیاز به راه‌اندازی مجدد.
- **معماری ماژولار**: امکان سفارشی‌سازی و گسترش از طریق ماژول‌ها.
- **پشتیبانی از APIهای REST و GraphQL**: یکپارچه‌سازی آسان با سایر سیستم‌ها.

## نصب و راه‌اندازی

### پیش‌نیازها
- **Java 11+**
- **Maven 3+**
- **PostgreSQL 12+**
- **Docker (اختیاری، برای استقرار در محیط کانتینری)**

### مراحل نصب
1. دریافت کد منبع Axelor SDK:
   ```sh
   git clone https://github.com/axelor/axelor-sdk.git
   cd axelor-sdk
   ```
2. ساخت پروژه:
   ```sh
   mvn clean install
   ```
3. اجرای SDK:
   ```sh
   mvn jetty:run
   ```
4. مرورگر خود را باز کرده و به آدرس `http://localhost:8080` بروید تا به محیط SDK دسترسی پیدا کنید.

## نحوه استفاده
- ایجاد برنامه‌های جدید اکسلور با استفاده از قالب‌های از پیش تعریف شده.
- تعریف مدل‌ها، نماها و گردش‌های کاری با کمترین نیاز به کدنویسی.
- استفاده از **Axelor Studio** برای مدل‌سازی بصری و توسعه سریع.

## مستندات
برای مطالعه مستندات کامل، به [مستندات Axelor](https://docs.axelor.com) مراجعه کنید.

## مشارکت در توسعه
مشارکت شما در توسعه این ابزار ارزشمند است! برای همکاری، مخزن را **Fork** کرده و درخواست **Pull Request** ارسال کنید.

## مجوز
Axelor SDK تحت **مجوز GNU Affero General Public License v3.0** منتشر شده است. برای جزئیات بیشتر، به فایل LICENSE مراجعه کنید.



Axelor SDK is a development toolkit designed for building enterprise applications using the Axelor Open Platform. It provides a streamlined development environment for creating, testing, and deploying Axelor-based applications.

## Features
- **Integrated Development Environment**: Pre-configured environment for Axelor application development.
- **Code Generation**: Automates repetitive coding tasks.
- **Hot Reloading**: Allows developers to see changes in real-time.
- **Modular Architecture**: Supports customization and extension through modules.
- **REST & GraphQL APIs**: Built-in API support for seamless integration.

## Installation

### Prerequisites
- Java 11+
- Maven 3+
- PostgreSQL 12+
- Docker (optional, for containerized deployment)

### Setup
1. Clone the Axelor SDK repository:
   ```sh
   git clone https://github.com/axelor/axelor-sdk.git
   cd axelor-sdk
   ```
2. Build the project:
   ```sh
   mvn clean install
   ```
3. Run the SDK:
   ```sh
   mvn jetty:run
   ```
4. Open `http://localhost:8080` in your browser to access the SDK.

## Usage
- Create new Axelor applications using the provided templates.
- Define models, views, and workflows with minimal coding.
- Use the Axelor Studio for visual modeling.

## Documentation
For detailed documentation, visit [Axelor Docs](https://docs.axelor.com).

## Contributing
Contributions are welcome! Please fork the repository and submit pull requests.

## License
Axelor SDK is released under the GNU Affero General Public License v3.0. See the LICENSE file for details.
