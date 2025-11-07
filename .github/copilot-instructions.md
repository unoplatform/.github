# GitHub Copilot Instructions for Uno Platform

Welcome to Uno Platform development! I'm here to help you build cross-platform applications using Uno Platform.

## About Uno Platform

Uno Platform is a cross-platform UI framework that allows you to build applications for WebAssembly, iOS, Android, macOS, Linux, and Windows using a single codebase with C# and XAML. It follows the MVVM (Model-View-ViewModel) pattern and implements WinUI 3 APIs with UWP compatibility.

## Working with Views and ViewModels

When working with Uno Platform, you'll frequently interact with:

### Views (XAML)
- **Pages**: Use `Page` for full-screen views
- **UserControls**: Use `UserControl` for reusable UI components
- **Custom Controls**: Extend `Control` for templatable controls
- **Location**: Typically in `Views/` or project root with `.xaml` extension

### ViewModels
- **Pattern**: Follow MVVM pattern with INotifyPropertyChanged
- **Base Classes**: Consider using `ObservableObject` or community MVVM libraries
- **Location**: Typically in `ViewModels/` folder with `ViewModel` suffix
- **Data Binding**: Use `{x:Bind}` for compiled bindings (WinUI/UWP style) or `{Binding}` for runtime bindings

## How I Can Help You

### Creating New Components
When you ask me to create a new View or ViewModel, I will:
1. Create the View file (`.xaml` and `.xaml.cs`) following Uno Platform conventions
2. Create the corresponding ViewModel with proper INotifyPropertyChanged implementation
3. Set up proper data binding between View and ViewModel
4. Include necessary using statements and namespaces
5. Follow Uno Platform best practices for cross-platform compatibility

### Common Tasks I Can Assist With

**View Development:**
- Creating XAML layouts using WinUI/UWP controls
- Implementing responsive designs for different form factors
- Setting up navigation between pages
- Creating reusable UserControls
- Implementing platform-specific UI adjustments

**ViewModel Development:**
- Implementing INotifyPropertyChanged pattern
- Creating commands for user interactions
- Managing application state
- Implementing data validation
- Handling async operations

**Platform-Specific Code:**
- Using `#if __ANDROID__`, `#if __IOS__`, `#if __WASM__` conditional compilation
- Implementing platform-specific features
- Handling platform differences

**Data Binding:**
- Setting up two-way bindings
- Using converters
- Implementing collection bindings with ObservableCollection
- Event binding with x:Bind

## Best Practices

1. **Use WinUI 3 APIs**: Uno Platform primarily implements WinUI 3 APIs with UWP compatibility, so refer to Microsoft's WinUI documentation
2. **Test on Multiple Platforms**: Code should work across WebAssembly, iOS, Android, and desktop platforms
3. **Follow MVVM Pattern**: Keep business logic in ViewModels, UI in Views
4. **Leverage Uno Extensions**: Consider using Uno.Extensions for MVVM, Navigation, Dependency Injection, Configuration, and Reactive programming
5. **Cross-Platform Compatibility**: Test platform-specific code thoroughly

## Uno Platform Renderers

Uno Platform supports two rendering approaches:
- **Native Renderer**: Uses native platform controls (default)
- **Skia Renderer**: Uses SkiaSharp for consistent cross-platform rendering

When providing solutions, I'll consider which renderer you're using if it affects the implementation.

## Getting Started with Common Scenarios

**To create a new page with ViewModel:**
Ask me: "Create a new [Name]Page with a [Name]ViewModel for [purpose]"

**To implement navigation:**
Ask me: "Implement navigation from [SourcePage] to [DestinationPage]"

**To add data binding:**
Ask me: "Add data binding between [property] and [control]"

**To implement a command:**
Ask me: "Create a command for [action] in [ViewModel]"

**To handle platform-specific code:**
Ask me: "Implement [feature] with platform-specific code for [platforms]"

## Additional Resources

- [Uno Platform Documentation](https://platform.uno/docs/)
- [WinUI 3 Documentation](https://learn.microsoft.com/windows/apps/winui/)
- [MVVM Pattern](https://learn.microsoft.com/dotnet/architecture/maui/mvvm)

I'm ready to help you build amazing cross-platform applications with Uno Platform! What would you like to work on?
