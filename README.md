# IWindowPrivate
RE'd for you so you can enable window transparency for (UWP) XAML Islands

If you are using Windows Runtime Projectors **(C#/WinRT (.NET 5), C++/WinRT, Rust/WinRT, etc..)** use **IWindowsPrivate.winmd**.

For **.NET Core 3.0 or older** (including "UWP .NET") use **IWindowsPrivate.cs**. 
This is because you can't use winmd that has namespaces that starts with "Windows.".

Usage example:
((Window.Current as object) as IWindowPrivate).TransparentBackground = true;
