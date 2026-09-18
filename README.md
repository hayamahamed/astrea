> [!NOTE]
> It is currently in alpha.

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="docs/astrea.svg" width = 300>
  <source media="(prefers-color-scheme: light)" srcset="docs/astrea-inverse.svg" width = 300>
  <img alt="Project Logo" src="docs/astrea.svg" width = 300>
</picture>

# Astrea

## Introduction - Astrea Linux

Astrea is a clean, secure, and highly usable operating system.
It comes with just a terminal, settings app, and files manager and still as fully omptimized for container oriented practices.

### Installation

To rebase an existing atomic Fedora installation to the latest build:

- First rebase to the unsigned image, to get the proper signing keys and policies installed:
  ```
  rpm-ostree rebase ostree-unverified-registry:ghcr.io/hayamahamed/astrealinux:latest
  ```
- Reboot to complete the rebase:
  ```
  reboot
  ```
- Then rebase to the signed image, like so:
  ```
  rpm-ostree rebase ostree-image-signed:docker://ghcr.io/hayamahamed/astrealinux:latest
  ```
- Reboot again to complete the installation
  ```
  reboot
  ```


> <img alt="Project Logo" src="docs/astrea-inverse.svg" width = 200>
>
> _Astrea - From Greek, The Star Maiden._
>
> _Astrea, depicted as the goddess of justice, innocence, and purity, became associated with the general spirit of renewal of culture occurred during the European Renaissance. The name _Astrea_ deriviated from a greek word. aster, "The Star", giving the reference "as The Star Maiden"._<br>
> _Astrea gives the chance to reflect the goal from the very name._


**Supported Platforms:**

Support is available for both x86_64 systems and ARM aarch64 systems.

### Credits
Like all the other projects, Astrea utilizes third party components. 
As an operating system, there might be too many third party components or dependency to list but, few of them could be considered what makes the most of the OS.

- Fedora: Fedora's fedora silverblue is used as the base.

- Bluebuild: Fedora silverblue is rebuilt as astrea with development parrallel to silverblue in almost all OS stack.

- Gnome: Gnome desktop environment is already clean and polished enough on its own. Using it is rational and practical.

### License
Astrea is licensed under _GNU AFFERO GENERAL PUBLIC LICENSE_. See [LICENSE](LICENSE).

- fedora is subject to this [LICENSE](https://docs.fedoraproject.org/en-US/legal/fedora-linux-license/).
- blue-build is subject to this [LICENSE](https://github.com/blue-build/github-action/blob/main/LICENSE). 
- Gnome is subject to this [LICENSE](https://help.gnome.org/papers/license.html).

As stated already, Components originated outside of these three might also be present.
