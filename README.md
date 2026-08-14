> [!WARNING]
> 🍐 PearPass is currently paused from active development, so please use at your own caution until further notice.

# pear-apps-utils-avatar-initials

A simple utility to generate initials for an avatar.

## Table of Contents

- [Features](#features)
- [Security Notice](#security-notice)
- [Installation](#installation)
- [Usage Examples](#usage-examples)
- [Dependencies](#dependencies)
- [Related Projects](#related-projects)

## Features

- Generates initials from names for use in avatars
- Handles single names by returning first two characters
- For multiple names, returns first letter of each of the first two names
- Properly handles edge cases like null, undefined, or empty strings
- Consistently returns uppercase initials

## Security Notice

1. To ensure the security and integrity of your projects, please note that official PearPass packages are distributed exclusively through our GitHub organization.
2. Any packages with similar names found on the npm registry or other third-party package managers are not affiliated with PearPass and should be strictly avoided. We recommend installing directly from this repository to ensure you are using the verified, open-source version.

## Installation

```bash
npm install git+https://github.com/tetherto/pear-apps-utils-avatar-initials.git
```

## Usage Examples

```javascript
import { generateAvatarInitials } from '@tetherto/pear-apps-utils-avatar-initials';

// Single name
generateAvatarInitials('John'); // Returns 'JO'

// Multiple names
generateAvatarInitials('John Doe'); // Returns 'JD'
generateAvatarInitials('John Doe Smith'); // Returns 'JD' (only uses first two names)

// Edge cases
generateAvatarInitials(''); // Returns ''
generateAvatarInitials(null); // Returns ''
generateAvatarInitials(undefined); // Returns ''
```

## Dependencies

This package has no external dependencies, making it lightweight and easy to include in any project.

## Related Projects

- [@tetherto/pearpass-app-mobile](https://github.com/tetherto/pearpass-app-mobile) - A mobile app for PearPass, a password manager
- [@tetherto/pearpass-app-desktop](https://github.com/tetherto/pearpass-app-desktop) - A desktop app for PearPass, a password
- [@tetherto/tether-dev-docs](https://github.com/tetherto/tether-dev-docs) - Documentations and guides for developers

## License

This project is licensed under the Apache License, Version 2.0. See the [LICENSE](./LICENSE) file for details.
