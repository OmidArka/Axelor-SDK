# Axelor SDK

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
