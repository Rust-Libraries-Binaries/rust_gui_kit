# rust_gui_kit

**rust_gui_kit** is a cross-platform graphical user interface (GUI) framework for Rust. This library aims to simplify the creation of desktop applications that run smoothly on Windows, macOS, and Linux. With a simple API, rust_gui_kit enables developers to build beautiful and responsive GUIs with ease.

## Features

- **Cross-Platform Support**: Create GUIs that work seamlessly on Windows, macOS, and Linux.
- **Simple API**: Intuitive and easy-to-use API for rapid development.
- **Basic Widgets**: Includes foundational widgets such as windows and buttons, with more to come.
- **Event Handling**: Basic event handling to manage user interactions.
- **Open-Source**: Encourage community contributions to expand and improve the library.

## Getting Started

### Installation

Add `rust_gui_kit` to your `Cargo.toml`:

```toml
[dependencies]
rust_gui_kit = "0.1.0"
```
Usage
Here is a simple example to get you started:
```use rust_gui_kit::{window::Window, button::Button};

fn main() {
    // Initialize the library (if needed)
    rust_gui_kit::initialize();

    // Create a new window
    let window = Window::new("Hello, GUI!", 800, 600);
    window.show();

    // Create a new button
    let button = Button::new("Click Me");
    button.on_click(|| {
        println!("Button was clicked!");
    });
}
```
## Examples
Check out the examples directory for more usage examples. To run an example, use:
```cargo run --example example_name
```
## Roadmap
Phase 1: Basic framework with window and button components.

Phase 2: Add more widgets such as text inputs, labels, and checkboxes.

Phase 3: Improve event handling and introduce theming support.

Ongoing: Regular updates based on community feedback and contributions.

## Contributing
We welcome contributions! If you’d like to contribute, please fork the repository and use a feature branch. Pull requests are warmly welcome.

Fork the repo and create your branch from main.

If you’ve added code that should be tested, add tests.

If you’ve changed APIs, update the documentation.

Ensure the test suite passes.

Make sure your code lints.

## License
This project is licensed under the MIT License. See the LICENSE file for more details.

## Author
Ben Santora <bensatlantik@gmail.com>

## Donate
If my Rust libraries have added value to your projects, consider supporting my work with a small donation. Thank you! [Donate Here](https://bensatlantik.github.io/donate.html)