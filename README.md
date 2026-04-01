# 🌤️ Avalonia Weather App

![.NET](https://img.shields.io/badge/.NET-9.0-512BD4?style=for-the-badge&logo=dotnet)
![Avalonia UI](https://img.shields.io/badge/Avalonia_UI-purple?style=for-the-badge)
![ReactiveUI](https://img.shields.io/badge/ReactiveUI-pink?style=for-the-badge)

A modern, responsive desktop weather application built with **C#**, **.NET 9**, and **Avalonia UI**. **This project was created primarily for educational purposes** to demonstrate practical desktop development, clean MVVM architecture, and custom XAML controls. 

The weather API key is securely integrated, allowing the application's source code to be explored and built out of the box without requiring external configurations.

## Key Features

* **Custom Animated Theming:** Features a fully custom Light/Dark mode toggle switch built from scratch. It utilizes Avalonia's `Transitions` and `DynamicResource` dictionaries for smooth, instant UI repainting.
* **Dynamic Weather Backgrounds:** The application UI automatically adapts to the current weather. A dedicated helper class parses weather descriptions (e.g., clear, rain, snow) and generates real-time `LinearGradientBrush` backgrounds.
* **Reactive MVVM Architecture:** Built entirely on **ReactiveUI**. Uses `ReactiveCommand.CreateFromTask` to handle asynchronous network requests, ensuring the main UI thread never freezes during data fetching.
* **Smart Location Selection:** Implements a cascading data structure (nested dictionaries) to efficiently filter and display countries and cities in the settings modal and search bar.


## Educational Value

As an educational project, this repository serves as an excellent reference for learning modern C# desktop development. It provides practical examples of:
* Overriding default Control Templates (e.g., modifying the `ContentPresenter` to remove default hover states for custom buttons).
* Handling nullable reference types safely when deserializing external JSON data.
* Structuring XAML for complex, responsive, and adaptive layouts using Grids.
* Separating UI logic from ViewModels using dedicated static helper classes.
