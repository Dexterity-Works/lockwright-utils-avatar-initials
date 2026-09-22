# lockwright-utils-avatar-initials

A simple utility to generate initials for an avatar.

Site: [lockwright.dexterity.works](https://lockwright.dexterity.works)

Community fork of PearPass (Apache 2.0). Not affiliated with or endorsed by Tether Data or the Pears project.

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

The package name is `lockwright-utils-avatar-initials`.

## Installation

```bash
npm install git+https://github.com/Dexterity-Works/lockwright-utils-avatar-initials.git
```

## Usage Examples

```javascript
import { generateAvatarInitials } from 'lockwright-utils-avatar-initials';

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

- [lockwright-app-mobile](https://github.com/Dexterity-Works/lockwright-app-mobile) - Lockwright for mobile
- [lockwright-app-desktop](https://github.com/Dexterity-Works/lockwright-app-desktop) - Lockwright for desktop
- [tether-dev-docs](https://github.com/Dexterity-Works/tether-dev-docs) - Documentations and guides for developers

## License

This project is licensed under the Apache License, Version 2.0. See the [LICENSE](./LICENSE) file for details.
