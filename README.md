# yunseongApps Documentation

Private documentation for managing multiple Android apps.

## Apps Overview

| App Name | Package ID | Version | Status |
|----------|-----------|---------|--------|
| [lottomate](apps/lottomate/README.md) | com.yunseong.lottomate | 1.0.0 | Active |
| [lunar](apps/lunar/README.md) | com.yun.lunarphase | 1.3.2 | Active |

## Quick Links

- [App Template](templates/app-template.md) - Use this template when adding a new app
- [Apps Directory](apps/) - Individual app documentation

## Structure

```
yunseongApps-docs/
├── README.md              # This file
├── apps/                  # Individual app docs
│   ├── lottomate/
│   │   └── README.md
│   └── lunar/
│       └── README.md
└── templates/
    └── app-template.md    # Template for new apps
```

## Adding a New App

1. Copy `templates/app-template.md` to `apps/[app-name]/README.md`
2. Fill in the app details
3. Update this README.md with the new app entry
4. Commit and push

---

**Note**: This repository contains sensitive information (API keys). Keep it private.
