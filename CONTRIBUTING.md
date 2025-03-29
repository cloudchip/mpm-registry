# Contributing to MPM Registry

Thank you for considering contributing to the **MPM Registry**! Your contributions help expand the ecosystem of microcontroller libraries and make development easier for everyone.

---

## How to Contribute

### 1. Adding a New Library
To add a library to the registry, follow these steps:

1. **Create a GitHub Issue**:
    - Open an issue in this repository with the following details:
      ```
      **Library Name**: <Library Name>
      **Version**: <Latest Version>
      **Description**: <Brief Description>
      **Repository**: <Repository URL>
      **Platforms**: <Supported Platforms (e.g., esp32, avr, stm32)>
      ```

2. **Wait for Review**:
    - The registry maintainers will review the issue for accuracy and relevance.

3. **Registry Update**:
    - Once approved, the maintainers will add the library to the `registry.json` file.

4. **Issue Closure**:
    - The issue will be closed once the library is added to the registry.

### Example Issue Template:
```
**Library Name**: DHT11
**Version**: 1.0.0
**Description**: Driver for the DHT11 IMU sensor
**Repository**: https://github.com/author/DHT11-driver
**Platforms**: esp32, avr, stm32
```

---

### 2. Updating an Existing Library
To update a library already in the registry (e.g., new version or additional platforms):

1. **Create a GitHub Issue**:
    - Open an issue in this repository with the following details:
      ```
      **Library Name**: <Library Name>
      **Current Version**: <Current Version>
      **New Version**: <New Version>
      **Changes**: <Description of Changes>
      **Platforms**: <Updated Platforms, if any>
      ```

2. **Wait for Review**:
    - The registry maintainers will review the update request.

3. **Registry Update**:
    - Once approved, the maintainers will update the `registry.json` file.

4. **Issue Closure**:
    - The issue will be closed once the updates are applied.

---

## Guidelines

### General Guidelines
- Ensure the library is publicly accessible.
- The library must be compatible with at least one microcontroller platform.
- Provide accurate and complete information in the issue template.

### Naming Conventions
- Use clear and descriptive names for libraries.
- Avoid duplicate names. If a name is already taken, consider using a unique identifier (e.g., `libraryname-author`).

---

## Getting Help

If you have questions or need assistance, feel free to open an issue or contact the maintainers through this repository.

---

## Code of Conduct

By contributing to this project, you agree to abide by our [Code of Conduct](CODE_OF_CONDUCT.md).

---

Thank you for your contributions and support!

