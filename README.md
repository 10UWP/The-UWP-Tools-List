# The-UWP-Tools-List

UWP - Universal Windows Platform for Windows 10 Desktop, Windows 10 Tablets, Windows 10 Mobile Phones, Windows 10 Pixelsense, Windows 10 IOT, Windows Server, Windows 10 HoloLens, and Windows 10 Xbox.

Some of the PCL based libraries also work with Android and Apple IOS via Xamarin. PCL targeted at .NET 3 also work with Unity 3D as another way of targeting Android and IOS. This List is currently focused on Windows 10 devices but I'll try to call out other targets.

On a Windows 10 Desktop or Tablet, a UWP App is typically deployed to a safe sandboxed environment via the Windows Store but the App can also be easily sideloaded to access legacy Windows 10 Desktop features and services with the ![BCTemplates](https://github.com/lancecontreras/BCTemplates)  project being an example of one approach.

This is extensive list (in progress) of potentially useful UWP Tools, Libraries, Samples etc to help make your UWP development more awesome. The list is non-curated (but with opininated comments when available). The ultimate objective is to provide a broad starting point for UWP development to perhaps help to offset the currently chaotic and sporadic information that is generally available.

All contributions are welcome. No guidlines other than Title, Link, Description. Adding an GitHub Issue might be your least effort way to add something here. I'll even try to insert any comments you might have to make this document a bit more interesting to read over and above a rather dry list of projects.




# Information
![awesome-uwp](https://github.com/tomzorz/awesome-uwp) Awesome UWP resources - inspired by Awesome .NET. - It appears to be a "curated" list whereas ![The-UWP-Tools-List](https://github.com/10UWP/The-UWP-Tools-List) is an attempt to include all possibly useful UWP tools and code.

# Frameworks

![MVVM-Sidekick](https://github.com/waynebaby/MVVM-Sidekick) A Modern light-weight MVVM framework based on RX and Await

![MugenMvvmToolkit](https://github.com/MugenMvvmToolkit/MugenMvvmToolkit) Mugen MVVM Toolkit makes it easier to develop cross-platform application using the Model-View-ViewModel design pattern. The Mugen MVVM Toolkit makes extensive use of Portable Class Libraries to provide maintainable cross platform C# native applications.

![mvvmlight](https://github.com/timdetering/mvvmlight) Git mirror of GalaSoft MVVM Light Toolkit (https://mvvmlight.codeplex.com/)

![Prism](https://github.com/PrismLibrary/Prism) Prism is a framework for building loosely coupled, maintainable, and testable XAML applications in WPF, Windows 10 UWP, and Xamarin Forms.

![Caliburn.Micro](https://github.com/Caliburn-Micro/Caliburn.Micro) A small, yet powerful framework, designed for building applications across all XAML platforms. Its strong support for MV* patterns will enable you to build your solution quickly, without the need to sacrifice code quality or testability. http://caliburnmicro.com/

![Okra App Framework](https://github.com/OkraFramework/Okra.Core) The Okra App Framework is designed to support the development of .Net Windows Store applications, in particular those following the MVVM pattern. http://okraframework.github.io

# Data

![EntityFramework](https://github.com/aspnet/EntityFramework) Microsoft's recommended data access technology for new applications in .NET. The ONLY UWP option is SQLite and ![it is a mess](http://ef.readthedocs.org/en/latest/providers/sqlite/limitations.html). ![Getting Started on Universal Windows Platform](http://ef.readthedocs.org/en/latest/platforms/uwp/getting-started.html) (Opinionated Note: "Microsoft's recommended data access technology" should not be reporting to ASP.NET which leads to the brain damaged situation of SQLite being the ONLY supported target for Microsoft's main thing, the Universal Windows Platform. The insanely stupid SQLite FK mess means that Entity Framework's Magic Unicorn (Migrations) becomes a useless broken technology on the One Microsoft platform that should count as the highest priority effort. UWP without an easy robust Microsoft supported data platform is a Microsoft blind spot that has been a drag on the success of the Win RT platform from the beginning. Or maybe I'm wrong and after 3 years of thinking, Microsoft re-defines easy and robust as "You can workaround some of these limitations by manually writing code in your migrations to perform a table rebuild. A table rebuild involves renaming the existing table, creating a new table, copying data to the new table, and dropping the old table. You will need to use the Sql(string) method to perform some of these steps." (https://github.com/aspnet/EntityFramework/issues/329) Or maybe you could help these "Lost Boys" with an ![ESENT database provider](https://github.com/aspnet/EntityFramework/issues/4423))  

![ESENT](https://msdn.microsoft.com/EN-US/library/gg269181%28v=exchg.10%29.aspx) Extensible Storage Engine is built into and is available for use on every Windows computer and has been an approved DLL for Windows Store since Windows 8.0. Updates to the database are implemented with a transaction in order to ensure secure operations. ESE enables simultaneous access to multiple databases, including transaction-log file databases that can be used for system recovery. ESE is scalable to large or small applications. ![ESENT Managed Interop](https://managedesent.codeplex.com/) it is not clear if the .NET wrapper is UWP compatible.

![BrightstarDB](https://github.com/BrightstarDB/BrightstarDB) BrightstarDB is a native .NET RDF triple store. It uses dotNetRDF to provide support for a wide range of RDF syntaxes as well as SPARQL query support. In addition to providing a raw RDF-based API, BrightstarDB also provides support for binding RDF resources to .NET dynamic objects; and a contract-first entity framework that enables the use of LINQ rather than SPARQL for query purposes.

![SQLite](http://www.sqlite.org/) SQLite is a software library that implements a self-contained, serverless, zero-configuration, transactional SQL database engine. SQLite is the most widely deployed database engine in the world. The source code for SQLite is in the public domain. Microsoft uses SQLite as a core component of Windows 10, and in individual numerous products. ![System.Data.SQLite](https://system.data.sqlite.org/index.html/doc/trunk/www/index.wiki) System.Data.SQLite is an ADO.NET provider for SQLite.  Development and maintenance work is now mostly performed by the SQLite Development Team. The SQLite team is committed to supporting System.Data.SQLite long-term. ![git mirror of SQLite](https://github.com/mackyle/sqlite) - ![DB Browser for SQLite](https://github.com/sqlitebrowser/sqlitebrowser) Official home of the DB Browser for SQLite (DB4S) project. Previously known as "SQLite Database Browser" and "Database Browser for SQLite". Website at: http://sqlitebrowser.org

![sqlite-net](https://github.com/praeclarum/sqlite-net) sqlite-net is an open source, minimal library to allow .NET and Mono applications to store data in SQLite 3 databases. It is written in C# and is meant to be simply compiled in with your projects. It was first designed to work with MonoTouch on the iPhone, but has grown up to work on all the platforms (Mono for Android, .NET, Silverlight, WP7, WinRT, Azure, etc.). Very simple methods for executing CRUD operations and queries safely (using parameters) and for retrieving the results of those query in a strongly typed fashion. Works with your data model without forcing you to change your classes. (Contains a small reflection-driven ORM layer.)

![YAWL.Serialization](https://github.com/YAWL/YAWL.Serialization) Serialization helper library for Windows applications

![ObservableSettings](https://github.com/joseangelmt/ObservableSettings) Create a Settings class for UWP (Universal Windows Platform) that is observable, strongly typed and with default values.

![MarcelloDB](https://github.com/markmeeus/MarcelloDB) .net/mono/xamarin/winrt in-process object database. MarcelloDB is a mobile NoSql database. It is very light-weight with minimal memory footprint. MarcelloDB saves plain C# objects, including child objects, lists and collections. Not having to map your objects to the relational model can save you hundreds of lines of code. MarcelloDB is a pure C# implementation, so there is no need to package other binaries.

![DynamicDataTemplate](https://github.com/kompiuter/DynamicDataTemplate) An example of how to dynamically select a data template based on the data type of an item, including examples in WPF & UWP.

# Templates

![Template10](https://github.com/Windows-XAML/Template10) Making Windows 10 apps awesome

![2016MVA-Template10](https://github.com/Windows-XAML/2016MVA-Template10)

![HamburgerTemplateUWP](https://github.com/StefanJanssen95/HamburgerTemplateUWP) A Hamburger Template for Visual Studio 2015 UWP

![UWP-Attached-ViewModel-Behavior-Template](https://github.com/espenrl/UWP-Attached-ViewModel-Behavior-Template)

![BCTemplates](https://github.com/lancecontreras/BCTemplates) Brokered Component Templates for UWP. These template includes client, server and proxy project and a starterkit which is a solution that contains those three projects. These are the basic projects needed to create a brokered component application. 


![WAT-UWP](https://github.com/sozercan/WAT-UWP) Web App Template (WAT) is Visual Studio 2015 project that lets developers create Universal Windows Platform (UWP) apps based on existing web content. Used in the right way, WAT can facilitate the creation of compelling extensions to your web content for Windows users.

![UWPNavBasics](https://github.com/kbfoot/UWPNavBasics) A replication of the Windows navigation sample for UWP with some tweaks to create a basic template

![UWPAppSkeleton](https://github.com/dkackman/UWPAppSkeleton) Project Template for an MMVM Light universal app that will create the skeleton of an app that looks and feels a lot like the built in Microsoft Windows 10 app (Weather, NFL etc). It's got all the basic stuff plumbed out like navigation and a navigation control, a settings page, Theme switch etc.

![UWPProjectTemplates](https://github.com/mspviraj/UWPProjectTemplates) Visual Studio 2015 Project Templates for Universal Windows Platform - UWPSimpleTemplate - bare bones MVVM support, UWPShellTemplate - provides a Hamburger navigation type AppShell with 4 different types of sample Views, PrismSimpleTemplate - bare bones using Prism 6 for UWP, PrismShellTemplate - same as UWPShellTemplate but using Prism 6 for UWP


![UWPTemplate](https://github.com/pablovargan/UWPTemplate)

![UWP_Application_Template](https://github.com/programmersommer/UWP_Application_Template) UWP template with pin/unpin secondary tile, share contract, rate and review and toast function

![UWP10template](https://github.com/mapaux/UWP10template) UWP template using MVVM pattern

# Composition
![Windows.UI.Composition WinRT API](https://github.com/Microsoft/composition) We are pleased to announce that as of Windows 10 Build 10586 and SDK Version 1511 the Windows.UI.Composition API is now fully public. Many thanks to all of those who contibuted feedback to on the API during it's preview phase to make it that much better. This repository contains code samples created with the Windows.UI.Composition WinRT API. Samples contained in this repository created by the Microsoft Composition team or contributors



![UWPCompositionDemos](https://github.com/clarkezone/UWPCompositionDemos) I work on the Composition team at Microsoft that builds the Windows.UI.Composition APIs for the Universal Windows Platform. This project is where I'll be putting demos of the API's functionality when I get time :-)

![Continuity](https://github.com/JustinXinLiu/Continuity) A project that aims to provide some cool animations, transitions and controls, built on top of the new Windows Composition API.

![StickyHeader_WindowsComposition](https://github.com/JustinXinLiu/StickyHeader_WindowsComposition)

![PullToRefreshUWP_WindowsComposition](https://github.com/JustinXinLiu/PullToRefreshUWP_WindowsComposition)

![WinCompositionPlayground](https://github.com/WaltRitscher/WinCompositionPlayground)

![CompositionAnimations](https://github.com/crb9826/CompositionAnimations) A wrapper PCL for the Windows.UI.Composion animations

![WinCompositionTiltEffect](https://github.com/r2d2rigo/WinCompositionTiltEffect) A behavior for adding a tilt effect to any UWP control, implemented using Windows Composition.

![UWP-Composition-Radial-Gauge](https://github.com/XamlBrewer/UWP-Composition-Radial-Gauge) A XAML Radial Gauge Custom Control for UWP that is partially drawn by the Composition API. It uses the release version of Composition API, so this requires Requires Visual Studio 2015 update 1 and Windows 10 10586 SDK on your side. A blog post that explains the code is right here: https://xamlbrewer.wordpress.com/2016/01/23/building-a-custom-uwp-control-with-xaml-and-the-composition-api/.

![CompositionHelper](https://github.com/higankanshi/CompositionHelper)

![CompositionAPI](https://github.com/agangal/CompositionAPI)

# Controls

![Radial Menu](https://github.com/CatalystCode/radial-menu) A Radial Menu for Windows UWP Applications, as made popular by the first versions of the modern OneNote App for Windows. Create radial menus floating op top of your application. The control supports variable numbers of buttons, toggle & radio buttons, a selector for long lists, and a fancy metered menu for intuitive selection of numbers.

![UWP-Radial-Gauge-Sample](https://github.com/XamlBrewer/UWP-Radial-Gauge-Sample) Demonstrates using the WinRT XAML Toolkit Radial Gauge on the Universal Windows Platform

![RadialSlider](https://github.com/galazzo/RadialSlider) A radial Slider for Windows 10 Universal Windows Platform (UWP)

![SplitViewMenuUWP](https://github.com/deanchalk/SplitViewMenuUWP) A custom control for a split view (hamburger) left menu for windows 10 univeral apps

![UWP-UniformGrid-Control](https://github.com/rickapps/UWP-UniformGrid-Control) The missing UniformGrid control from WPF ported to UWP

![Windows App Studio Libraries](https://github.com/wasteam/waslibs) This repository contains the source code of the libraries used by Windows App Studio in the generated apps. There are three libraries: utility classes to create XAML applications, all the data sources available in Windows App Studio apps, and XAML controls for Windows 10 apps only.

![ExpanderUWP](https://github.com/deanchalk/ExpanderUWP) Expander Control for Microsoft UWP

![Kimono](https://github.com/Amrykid/Kimono) A Windows 10 UWP (.NET) library with a set of UI controls

![WinUX-UWP-Toolkit](https://github.com/jamesmcroft/WinUX-UWP-Toolkit) A collection of core XAML controls and extensions to use in your personal universal Windows apps http://jamescroft.co.uk/blog/uwp/introducing-croft-core-for-universal-windows-apps/

![comet](https://github.com/nmetulev/comet) Universal Windows Platform (UWP) toolkit library. Contains controls for creating great user experiences for Universal Windows Applications

![WinRTXamlToolkit](https://github.com/xyzzer/WinRTXamlToolkit) A set of controls, extensions and helper classes for Windows Runtime XAML applications.

![Naylah.Toolkit.UWP](https://github.com/NaylahProject/Naylah.Toolkit.UWP) Naylah SDK for Universal Windows Plataform http://naylahproject.github.io/Naylah.UWP/ Contain useful libraries, controls, helpers, architecture, etc. The intent is create a community for developers focusing in deliver better-beatiful apps. To create next generation of apps.

![Coding4FunToolkit](https://github.com/Coding4FunProjects/Coding4FunToolkit) This is where Coding4Fun will house all our cool controls and tools that we come up with

![UwpProjects](https://github.com/LanceMcCarthy/UwpProjects) A set of UWP controls and utilities. 
    BusyIndicators in UwpHelpers.Controls.BusyIndicators (cool custom busy indicator)
    AdaptiveGridView in UwpHelpers.Controls.ListControls (maintains aspect ratio of items as it scales for column width)
    BlurElementAsync in UwpHelpers.Examples.Helpers (converts any UIElement into a blurred BitmapImage)
    IncrementalLoadingCollection in UwpHelpers.Controls.Common (demo in Examples)
    NetworkImage in UwpHelpers.Controls.ImageControls (an Image control that shows download progress)


# UI
![ReactiveUI](https://github.com/reactiveui/ReactiveUI) A MVVM framework that integrates with the Reactive Extensions for .NET to create elegant, testable User Interfaces that run on any mobile or desktop platform. Supports Xamarin.iOS, Xamarin.Android, Xamarin.Mac, Xamarin Forms, WPF, Windows Forms, Windows Phone 8, Windows Store and Universal Windows Platform (UWP). http://www.reactiveui.net

![userdialogs](https://github.com/aritchie/userdialogs) A cross platform library that allows you to call for standard user dialogs from a shared/portable library, Actionsheets, alerts, confirmations, loading, login, progress, prompt, toast... async just for fun. Supports Android, iOS, Windows Phone 8.0 (silverlight), and Unified Windows Platform (UWP, UAP)

![BlendrocksToolkit](https://github.com/deanihansen/BlendrocksToolkit) Windows UWP toolkit that which enabled insanely cool page transitions and easier navigation and app handling.

![Monolith](https://github.com/ThatLousyGuy/Monolith) Monolith is a Windows library that lets you create animations in codebehind in a fluent, somewhat straightforward manner. It's a wrapper around the Windows.UI.Xaml.Media.Animation library that removes as much of the setup as possible. (Thanks to ![Awesome UWP resources list](https://github.com/tomzorz/awesome-uwp) for the head's up on this interesting project.

![WindowsStateTriggers](https://github.com/dotMorten/WindowsStateTriggers) A collection of custom visual state triggers


# Libs

![Groves](https://github.com/tomzorz/Groves) A UWP library by the author of the ![Awesome UWP resources list](https://github.com/tomzorz/awesome-uwp) 

![YAWL.Composition](https://github.com/YAWL/YAWL.Composition) Composable building blocks for MVVM based Windows 10 applications

![observable-vector](https://github.com/jamesqo/observable-vector) A no-frills implementation of IObservableVector for Windows 10 apps.

![Shims.Xaml](https://github.com/jamesqo/Shims.Xaml) Easily create libraries that work on both WPF and Windows 10.

![XamlBehaviors](https://github.com/Microsoft/XamlBehaviors) This is the official home for XAML Behaviors on GitHub. XAML Behaviors is an easy-to-use means of adding common and reusable interactivity to your Windows UWP applications with minimal code. It is available for both native and managed applications.

![Portable.Xaml](https://github.com/cwensley/Portable.Xaml) Portable .NET library for reading/writing xaml files. This is intended to be used to read Xaml on desktop, mobile, and CoreCLR platforms.

![typed-xaml](https://github.com/jamesqo/typed-xaml) Advanced generics support for WPF and Windows 10.

![uwp-chrome](https://github.com/RReverser/uwp-chrome) Experimental chrome API shim for Universal Windows Platform (UWP / WinRT)

![UWP-Helpers](https://github.com/EdiWang/UWP-Helpers) Helpers and Utils for UWP Projects

![MyToolkit](https://github.com/MyToolkit/MyToolkit) MyToolkit for .NET http://mytoolkit.io MyToolkit is a set of .NET libraries containing lots of useful classes for various .NET platforms like UWP/WinRT (Universal Windows Apps), Windows Phone and WPF. The goal is to provide missing or replace existing classes to support the development of high-quality Windows and Windows Phone applications. For example, the library provides often used MVVM infrastructure classes, missing UI controls, IoC classes, additional LINQ extension methods and much more.

![Cimbalino-Toolkit](https://github.com/Cimbalino/Cimbalino-Toolkit) Cimbalino Toolkit http://cimbalino.org Cimbalino Toolkit is a set of useful and powerful tools that will help you build your Windows Platform applications.

![cadru](https://github.com/scottdorman/cadru) A Microsoft .NET Framework toolkit http://scottdorman.github.io/cadru Cadru is a utility framework containing new APIs and extensions to the core .NET Framework to help complete your developer toolbox. It is designed to be portable first, which means that the majority of the library is available as a Portable Class Library (PCL) 

![Windows-task-snippets](https://github.com/Microsoft/Windows-task-snippets) This repo collects snippets of ready-to-use code that accomplish small but useful tasks of interest to Universal Windows Platform (UWP) app developers. These snippets represent simple solutions to common problems, and simple recipes to help you implement new app features. 

![UWP-Networking-Essentials](https://github.com/SvenEV/UWP-Networking-Essentials) Simple and lightweight networking (including RPC) for Universal Windows Platform apps

# Graphics 2D
![Win2D](https://github.com/Microsoft/Win2D) Win2D is an easy-to-use Windows Runtime API for immediate mode 2D graphics rendering with GPU acceleration. It is available to C# and C++ developers writing Windows apps for Windows 8.1, Windows Phone 8.1 and Windows 10. It utilizes the power of Direct2D, and integrates seamlessly with XAML and CoreWindow. http://microsoft.github.io/Win2D (https://github.com/Microsoft/Win2D-Samples)

![SvgForXaml](https://github.com/mntone/SvgForXaml) Draw image from svg file with Win2D

![XamlAnimatedGif](https://github.com/XamlAnimatedGif/XamlAnimatedGif) A simple library to display animated GIF images in XAML apps (WPF, WinRT, Windows Phone)

![WriteableBitmapEx](https://github.com/teichgraf/WriteableBitmapEx) The WriteableBitmapEx library is a collection of extension methods for the WriteableBitmap. The WriteableBitmap class is available for all XAML flavors including Windows Phone, WPF, WinRT Windows Store XAML, (Windows 10) UWP and Silverlight. It was even ported to Windows Embedded. WriteableBitmapEx allows the direct manipulation of a bitmap and can be used for image manipulation, to generate fast procedural images by drawing directly to a bitmap and more. The WriteableBitmap API is very minimalistic and there's only the raw Pixels array for such operations. The WriteableBitmapEx library tries to compensate that with extensions methods that are easy to use like built in methods and offer GDI+ like functionality. The library extends the WriteableBitmap class with elementary and fast (2D drawing) functionality, conversion methods and functions to combine (blit) WriteableBitmaps. The extension methods are grouped into different C# files using a partial class approach. It is possible to include just a few methods by using the specific source code files directly or the full functionality via the built binaries. 

# Graphics 3D
![SharpDX](https://github.com/sharpdx/SharpDX)

![DirectXTK](https://github.com/Microsoft/DirectXTK) The DirectX Tool Kit (aka DirectXTK) is a collection of helper classes for writing DirectX 11.x code in C++ http://blogs.msdn.com/b/chuckw/archive/2012/03/02/directxtk.aspx

![DirectXTex](https://github.com/Microsoft/DirectXTex) DirectXTex texture processing library http://blogs.msdn.com/b/chuckw/archive/2011/10/28/directxtex.aspx

![DirectX-Graphics-Samples](https://github.com/Microsoft/DirectX-Graphics-Samples) This repo contains the DirectX Graphics samples that demonstrate how to build graphics intensive applications on Windows.

![DXUT](https://github.com/Microsoft/DXUT) DXUT is a "GLUT"-like framework for Direct3D 11.x Win32 desktop applications; primarily samples, demos, and prototypes. http://blogs.msdn.com/b/chuckw/archive/2013/09/16/dxut-for-win32-desktop-update.aspx

![FX11](https://github.com/Microsoft/FX11) Effects for Direct3D 11 (FX11) is a management runtime for authoring HLSL shaders, render state, and runtime variables together. http://blogs.msdn.com/b/chuckw/archive/2012/10/23/effects-for-direct3d-11-update.aspx


![UVAtlas](https://github.com/Microsoft/UVAtlas) UVAtlas isochart texture atlas http://blogs.msdn.com/b/chuckw/archive/2014/11/14/uvatlas-return-of-the-isochart.aspx

![DirectXMesh](https://github.com/Microsoft/DirectXMesh) DirectXMesh geometry processing library http://blogs.msdn.com/b/chuckw/archive/2014/06/27/directxmesh.aspx performing various geometry
content processing operations including generating normals and tangent frames, triangle
adjacency computations, and vertex cache optimization.


# Language

![The Visual F# compiler and tools](https://github.com/Microsoft/visualfsharp) F# is a mature, open source, cross-platform, functional-first programming language which empowers users and organizations to tackle complex computing problems with simple, maintainable, and robust code. F# is used in a wide range of application areas and is supported by Microsoft and other industry-leading companies providing professional tools, and by an active open community. You can find out more about F# at http://fsharp.org.

# Testing

Opinionated Note: Testing is valuable but Unit Testing is a social meme associated with the always hard to pin down Agile movement but despite my dislike of meme-driven-development, I'll include UWP focused Unit Testing since you need to jump thru extra hoops on top of the already rediculous monkey hoops and various perversions of Object Design in order to make your CI robot lamp glow green on UWP...

![myweather](https://github.com/fernandoescolar/myweather) This is a demo of unit testing in UWP. It contains a T4 template to generate all the Spies, Stubs and Mocks of all the interfdaces found in your solution.

![xUnit.net](https://github.com/xunit/xunit) xUnit.net is a free, open source, community-focused unit testing tool for the .NET Framework. Written by the original inventor of NUnit v2, xUnit.net is the latest technology for unit testing C#, F#, VB.NET and other .NET languages. xUnit.net works with ReSharper, CodeRush, TestDriven.NET and Xamarin. It is part of the ASP.NET Open Source Gallery under the Outercurve Foundation, licensed under Apache 2 (an OSI approved license). ![Getting Started with xUnit.net (Universal Windows Apps)](http://xunit.github.io/docs/getting-started-uwp.html)

![xunit-performance](https://github.com/Microsoft/xunit-performance) Provides extensions over xUnit to author performance tests.

![FluentAssertions](https://github.com/dennisdoomen/FluentAssertions) Fluent Assertions is a set of .NET extension methods that allow you to more naturally specify the expected outcome of a TDD or BDD-style test. We currently use it in all our internal and client projects, and it is used in many open-source projects. It runs on .NET 4.0, 4.5, 4.6, CoreClr, .NET Native, Windows 8.1, Silverlight 5, Windows Phone 8.0… http://www.fluentassertions.com

![FluentAssertionsEx](https://github.com/hivepeople/FluentAssertionsEx) Extensions for FluentAssertions.

![FluentAssertions.Autofac](https://github.com/awesome-inc/FluentAssertions.Autofac) Fluent Assertions extensions for Autofac

![Shouldly](https://github.com/shouldly/shouldly) Should testing for .net - the way Asserting *Should* be! http://shouldly.readthedocs.org/en/latest




# Samples
![ComposableAdaptiveTriggerDemo](https://github.com/LocalJoost/ComposableAdaptiveTriggerDemo) Demo of a AdaptiveTrigger that works with a StateTrigger inside a CompositeStateTrigger from WindowsStateTriggers

![YAWL.Common](https://github.com/YAWL/YAWL.Common) Common library for all new Windows Phone/Store/UWP/Mobile and Xamarin applications

![Windows-universal-samples](https://github.com/Microsoft/Windows-universal-samples) Official API samples for the Universal Windows Platform.

![ImagingUWP](https://github.com/asiertarancon/ImagingUWP) UWP app with Lumia Imaging SDK

![HealthClinic.biz](https://github.com/Microsoft/HealthClinic.biz) The samples contained in this repo are used to present an end-to-end demo scenario based on a fictitious B2B and multitenant system, named “HealthClinic.biz” that provides different websites, mobile apps, desktop apps, wearable apps, and services running on the latest Microsoft and open technologies aligned with announcements to showcase during … http://aka.ms/Connect

![UWPQuickStart](https://github.com/Microsoft/UWPQuickStart) Building a Universal Windows app in Visual Studio is quick and easy. We've provided a sample app that you can download and learn how the various pieces fit together. We even encourage you to customize and send a version of this app to the Windows Store!

![Windows-appsample-quizgame](https://github.com/Microsoft/Windows-appsample-quizgame) A peer-to-peer trivia game sample for the Universal Windows Platform (UWP). 
