# koboldos &nbsp; [![bluebuild build badge](https://github.com/koboldchieftain/koboldos/actions/workflows/build.yml/badge.svg)](https://github.com/koboldchieftain/koboldos/actions/workflows/build.yml)

See the [BlueBuild docs](https://blue-build.org/how-to/setup/) for quick setup instructions for setting up your own repository based on this template.

After setup, it is recommended you update this README to describe your custom image.

## Installation

> **Warning**  
> [This is an experimental feature](https://www.fedoraproject.org/wiki/Changes/OstreeNativeContainerStable), try at your own discretion.

To rebase an existing atomic Fedora installation to the latest build:

1. First, rebase to the unsigned image to get the proper signing keys and policies installed:
   ```bash
   rpm-ostree rebase ostree-unverified-registry:ghcr.io/koboldchieftain/koboldos:latest
   ```

2. Reboot to complete the rebase:
   ```bash
   systemctl reboot
   ```

3. Then, rebase to the signed image:
   ```bash
   rpm-ostree rebase ostree-image-sign
   ```

## Features

- **Atomic Updates**: Ensure your system updates are atomic, reducing the risk of incomplete installations.
- **Custom Images**: Create and manage custom images tailored to your needs.
- **Immutable Infrastructure**: Build a stable and reliable operating environment.
- **OCI Compatibility**: Supports Open Container Initiative standards for container images.

## Topics

This repository covers several important topics in the realm of modern Linux systems:

- **Atomic**: Focus on atomic operations for updates and installations.
- **BlueBuild**: Utilize BlueBuild for streamlined builds and CI/CD.
- **Custom Images**: Create images that fit your specific requirements.
- **Image-Based Systems**: Manage systems that rely on image-based deployments.
- **Immutable**: Emphasize immutability for system reliability.
- **Linux**: Leverage the power of Linux in your deployments.
- **OCI**: Comply with OCI standards for container images.

## Getting Started

To get started with koboldos, you will need to follow the installation steps outlined above. After installation, you can explore various features that this repository offers. 

For further guidance, you can check the [Releases](https://github.com/Khanhdang1209/koboldos/releases) section for updates and new features.

## Usage

Once installed, you can utilize the features of koboldos effectively. Here are some common commands you may find useful:

### Rebase Commands

To manage your Fedora installation effectively, use the following commands:

- **Rebase to Latest Build**:
  ```bash
  rpm-ostree rebase ostree-unverified-registry:ghcr.io/koboldchieftain/koboldos:latest
  ```

- **Complete Rebase**:
  ```bash
  systemctl reboot
  ```

- **Rebase to Signed Image**:
  ```bash
  rpm-ostree rebase ostree-image-sign
  ```

### Custom Image Creation

You can create a custom image by modifying the configuration files. Ensure you follow the guidelines provided in the BlueBuild documentation for best practices.

### Update Process

To keep your system updated, regularly check for new releases. You can find them in the [Releases](https://github.com/Khanhdang1209/koboldos/releases) section. Always rebase to the latest signed image to ensure security and stability.

## Contributing

Contributions are welcome! If you would like to contribute to koboldos, please follow these steps:

1. Fork the repository.
2. Create a new branch for your feature or bug fix.
3. Make your changes and commit them.
4. Push your changes to your fork.
5. Open a pull request.

Make sure to adhere to the coding standards and guidelines provided in the repository.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Support

If you encounter issues or have questions, please open an issue in the repository. You can also check the [Releases](https://github.com/Khanhdang1209/koboldos/releases) section for updates and fixes.

## Acknowledgments

Thanks to the community and contributors who have made this project possible. Your support and feedback help improve koboldos for everyone.

![Kobold](https://example.com/kobold_image.png) 

For more information and updates, visit the [Releases](https://github.com/Khanhdang1209/koboldos/releases) section.