# 🚀 Modern C++ Learning Checklist (For Novice to Intermediate Programmers)

A structured guide to learning and applying **Modern C++ (C++11 through C++23)** — minimal, efficient, and powerful.

---

## 📘 Language Fundamentals

| Feature            | Description                                      | ✅ |
|--------------------|--------------------------------------------------|----|
| `auto`             | Type inference for cleaner code                  | ☐  |
| `nullptr`          | Type-safe null pointer                           | ☐  |
| `enum class`       | Scoped, strongly-typed enums                     | ☐  |
| `override`, `final`| Safer inheritance and method overrides           | ☐  |
| Uniform Init `{}`  | Prevents narrowing, consistent init              | ☐  |
| `constexpr`        | Compile-time computation                         | ☐  |
| `noexcept`         | Signals that a function doesn’t throw            | ☐  |
| `[[nodiscard]]`    | Warn when a return value is ignored              | ☐  |
| Range-based `for`  | Cleaner and safer looping                        | ☐  |
| Structured Bindings| Unpack tuples or structs easily                  | ☐  |
| `if constexpr`     | Compile-time branching in templates              | ☐  |
| Concepts (C++20)   | Type constraints in templates                    | ☐  |

---

## 📦 Standard Library Types

| Feature             | Description                                      | ✅ |
|---------------------|--------------------------------------------------|----|
| `std::vector`       | Dynamic arrays                                   | ☐  |
| `std::array`        | Fixed-size array with better safety              | ☐  |
| `std::string_view`  | Lightweight non-owning string                    | ☐  |
| `std::span` (C++20) | Safe view over arrays or containers              | ☐  |
| `std::optional`     | Safe way to express "maybe a value"              | ☐  |
| `std::variant`      | Type-safe union                                  | ☐  |
| `std::any`          | Hold any type (use sparingly)                    | ☐  |
| `std::chrono`       | Time durations and clocks                        | ☐  |
| `std::filesystem`   | Portable file handling                           | ☐  |
| `std::thread`       | Basic multithreading                             | ☐  |
| `std::jthread` (C++20)| Automatically joining thread                   | ☐  |
| `std::format` (C++20)| Clean, type-safe formatting                     | ☐  |

---

## 🧰 Third-Party Libraries (Recommended)

| Library             | Use Case                                | ✅ |
|---------------------|------------------------------------------|----|
| [`fmt`](https://github.com/fmtlib/fmt)             | Better formatting (used by `std::format`) | ☐  |
| [`spdlog`](https://github.com/gabime/spdlog)       | High-performance logging                  | ☐  |
| [`tl::expected`](https://github.com/TartanLlama/expected) | Error handling instead of exceptions | ☐  |
| [`nlohmann/json`](https://github.com/nlohmann/json)| Modern JSON handling                      | ☐  |
| [`cxxopts`](https://github.com/jarro2783/cxxopts)  | Command-line argument parser              | ☐  |
| [`doctest`](https://github.com/doctest/doctest) or [`Catch2`](https://github.com/catchorg/Catch2) | Unit testing frameworks | ☐  |
| [`GSL`](https://github.com/microsoft/GSL)          | Safer span, not_null, contracts           | ☐  |

---

## 🛠 Practice Ideas

| Project Idea                         | Focus Areas                            | ✅ |
|--------------------------------------|-----------------------------------------|----|
| Safe config file parser              | `optional`, `string_view`, JSON         | ☐  |
| CLI tool with logging                | `spdlog`, `chrono`, `format`            | ☐  |
| Timer utility                        | `chrono`, `constexpr`, `thread`         | ☐  |
| Memory-safe vector wrapper           | `unique_ptr`, `span`, `GSL`             | ☐  |
| Plugin-style system with `variant`   | `variant`, `visit`, `any`               | ☐  |
| Compile-time math lib                | `constexpr`, `if constexpr`, concepts   | ☐  |

---

## 🧩 Notes

- **Use `auto` carefully** — don’t lose readability.
- **Avoid raw `new/delete`** — prefer `unique_ptr` or stack objects.
- **Use `string_view` or `span`** for zero-copy APIs.
- **Avoid template abuse** — prefer concepts and clear constraints.
- **Format, test, and log** like a professional.

---

✅ _Tip: Track your progress and experiment with each feature in isolation before combining them into projects._

