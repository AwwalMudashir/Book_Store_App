# Book Store App

A cross-platform Book Store application built with [Flutter](https://flutter.dev/) for Android, iOS, Web, Windows, macOS, and Linux.  
The backend is powered by a Spring Boot REST API.

## Features

- User authentication (register, login, Google sign-in)
- Browse book catalog (all, bestsellers, new arrivals)
- Book details with reviews and ratings
- Search and filter books
- Shopping cart and checkout flow
- Wishlist management
- Order history
- User profile management
- Admin dashboard for managing books, users, and orders

## Project Structure

- `lib/` — Main Flutter/Dart source code
- `android/`, `ios/`, `web/`, `windows/`, `macos/`, `linux/` — Platform-specific code
- `assets/` — Images and other static assets
- `test/` — Unit and widget tests

## Getting Started

### Prerequisites

- [Flutter SDK](https://docs.flutter.dev/get-started/install)
- [Dart SDK](https://dart.dev/get-dart)
- Backend: [Spring Boot Book Store API](https://spring.io/projects/spring-boot) (must be running, see API URL in [`lib/core/constants.dart`](lib/core/constants.dart))

### Setup

1. **Clone this repository:**
   ```sh
   git clone <repo-url>
   cd book_store_app
   ```

2. **Install dependencies:**
   ```sh
   flutter pub get
   ```

3. **Configure API endpoint:**
   - Update the `apiBaseUrl` in [`lib/core/constants.dart`](lib/core/constants.dart) if your backend is not running at `http://10.0.2.2:8080/api`.

4. **Run the app:**
   ```sh
   flutter run
   ```

   - For web: `flutter run -d chrome`
   - For desktop: `flutter run -d windows` (or `macos`, `linux`)

## Testing

Run all tests with:
```sh
flutter test
```

## Customization

- UI themes: [`lib/core/theme.dart`](lib/core/theme.dart)
- Add assets: Place images in `assets/` and update `pubspec.yaml`.

## License

This project is for educational purposes.

---

**Backend:** Spring Boot REST API (not included in this repo)
