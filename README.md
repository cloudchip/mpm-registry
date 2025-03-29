# MPM Registry

The **MPM Registry** is the central repository for managing microcontroller libraries compatible with the **Microcontroller Package Manager (MPM)**. It acts as a source for downloading, updating, and tracking libraries for various microcontroller platforms, ensuring easy integration and dependency management.

---

## Repository Structure

This repository contains the following structure:

```
mpm-registry/
├── registry.json
└── CONTRIBUTING.md
```

### Key Files
- **`registry.json`**: The master list of all library repository links in the registry. This file includes metadata such as library names, versions, descriptions, and source URLs.

---

## `registry.json` Format

The `registry.json` file serves as the central index of all available libraries.

### Example Format:
```json
{
    "libraries": {
        "mpu6050": {
            "name": "MPU6050",
            "version": "1.0.0",
            "description": "Driver for the MPU6050 IMU sensor",
            "repository": "https://github.com/author/mpu6050-driver",
            "platforms": ["esp32", "avr", "stm32"]
        },
        "ssd1306": {
            "name": "SSD1306",
            "version": "2.1.3",
            "description": "OLED display driver",
            "repository": "https://github.com/author/ssd1306-driver",
            "platforms": ["esp32", "stm32"]
        }
    }
}
```

### Key Fields:
- **`name`**: Library name (unique identifier).
- **`version`**: Latest version of the library.
- **`description`**: Brief description of the library.
- **`repository`**: URL to the library's GitHub or other VCS repository.
- **`platforms`**: Supported microcontroller platforms (e.g., `esp32`, `avr`, `stm32`).

---

## Adding a Library

To add a library to the registry:

1. **Create a GitHub Issue**: Library creators should open an issue in this repository with the following details:
    - Library name
    - Version
    - Description
    - Repository URL
    - Supported platforms

    Example:
    ```
    **Library Name**: MPU6050
    **Version**: 1.0.0
    **Description**: Driver for the MPU6050 IMU sensor
    **Repository**: https://github.com/author/mpu6050-driver
    **Platforms**: esp32, avr, stm32
    ```

2. **Registry Maintainers Update**: Once the issue is reviewed and approved, the registry maintainers will update the `registry.json` file with the provided information.

3. **Issue Closure**: After updating the registry, the issue will be closed.

---

## Contributing

We welcome contributions to the MPM Registry. Please see the [CONTRIBUTING.md](CONTRIBUTING.md) file for guidelines on how to contribute new libraries or improve existing ones.

---

## Usage with MPM CLI

To use the MPM Registry with the **MPM CLI Tool**:

1. Install the MPM CLI tool.
2. Search and install libraries from the registry:
   ```bash
   mpm install mpu6050
   ```
3. The library will be downloaded into the `lib/` folder of your project.

---

## License

This repository is licensed under the MIT License. See [LICENSE](LICENSE) for more details.

