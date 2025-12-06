# Lunar Phase

## Basic Information

- **App Name**: Lunar Phase
- **Package ID**: `com.yun.lunarphase`
- **Version Code**: 7
- **Version Name**: 1.3.2
- **Min SDK**: 29
- **Target SDK**: 36
- **Status**: Active

## Description

Lunar Phase is an app that displays moon phase information using external lunar data API. Built with Jetpack Compose and following MVVM architecture pattern.

## API Keys & Credentials

### Required Environment Variables

Add these to `local.properties` in the root project:

```properties
# Lunar Phase API Key
LUNAR_API_KEY=your_lunar_api_key_here
```

### Key Details

| Key Name | Purpose | Where to get it | Notes |
|----------|---------|-----------------|-------|
| LUNAR_API_KEY | Access lunar phase data | [Lunar API Provider] | Required for fetching moon phase information |

## Features

- **Moon Phase Display**: View current moon phase
- **Phase Database**: Local caching of moon phase data
- **Date Handling**: Accurate date-based phase calculations

## Dependencies

### Feature Modules
- `:feature:moon:common` - Shared moon functionality
- `:feature:moon:phase` - Moon phase display
- `:feature:moon:database` - Local data persistence

### Key Libraries
- **Hilt**: Dependency injection
- **Joda-Time**: Date and time handling (v2.10.6)
- **Kotlin Coroutines**: Asynchronous operations
- **Jetpack Compose**: Modern UI toolkit

## Build Configuration

### Build Commands

```bash
# Debug build
./gradlew :app:lunar:assembleDebug

# Release build
./gradlew :app:lunar:assembleRelease

# Install on device
./gradlew :app:lunar:installDebug
```

## Testing

```bash
# Unit tests
./gradlew :app:lunar:test

# Instrumented tests
./gradlew :app:lunar:connectedAndroidTest
```

## Architecture

- **Pattern**: MVVM (Model-View-ViewModel)
- **UI Framework**: Jetpack Compose
- **DI**: Hilt
- **Async**: Kotlin Coroutines
- **Date Library**: Joda-Time for reliable date calculations
- **Build System**: Convention Plugins

## Release Notes

### v1.3.2 (Current)
- MVVM architecture implementation
- Multi-module structure with moon feature modules
- Improved date handling with Joda-Time

### Previous Versions
- Version history from v1 to v1.3.1

## Notes

- Uses Joda-Time instead of Java Date/Calendar for better reliability
- ProGuard enabled for release builds
- Local database for caching moon phase data
- LUNAR_API_KEY must be set in `local.properties` before building
