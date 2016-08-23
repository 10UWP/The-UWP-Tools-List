# The-UWP-Tools-List

UWP - Universal Windows Platform for Windows 10 Desktop, Windows 10 Tablets, Windows 10 Mobile Phones, Windows 10 Pixelsense, Windows 10 IOT, Windows Server, Windows 10 HoloLens, and Windows 10 Xbox.

Some UWP libraries are PCL based and should also work with Android and Apple IOS via Xamarin. PCL targeted at .NET 3 also work with Unity 3D as another way of targeting Android and IOS. This List is currently focused on Windows 10 devices but I'll try to call out other targets. The introduction of .NET Core should also help in this area.

On a Windows 10 Desktop or Tablet, a UWP App is typically deployed to a safe sandboxed environment via the Windows Store but the App can also be easily sideloaded to access legacy Windows 10 Desktop features and services with the ![BCTemplates](https://github.com/lancecontreras/BCTemplates)  project being an example of one approach. This process has become very convenient with the Anniversary Update and is a simple setting in "Update & security" which makes a Windows 10 Tablet and Windows 10 Mobile device a very convenient deployment device for all kinds of touch based applications out in the "Real World"

This is extensive list (in progress) of potentially useful UWP Tools, Libraries, Samples etc to help make your UWP development more awesome. The list is non-curated (but with opininated comments when available). The ultimate objective is to provide a broad starting point for UWP development to perhaps help to offset the currently chaotic and sporadic information that is generally available.

All contributions are welcome. Try to include a Title, Link, Description but any comment is welcome. Adding an GitHub Issue is another low effort way to add something here. I'll even try to insert any editorial type comments you might want to share in order to make this document a bit more interesting to read over and above a rather dry list of projects.


# Microsoft

Note that current Microsoft Emulators are based on Hyper-V which is a low overhead VM technology. To painlessly fire up emulators, you need both a modern CPU that supports SLAT instructions and the "Pro" version of Windows 10.

### ![Microsoft Downloads and tools for Windows 10](https://developer.microsoft.com/en-us/windows/downloads)

![Windows App Certification Kit](https://developer.microsoft.com/en-us/windows/develop/app-certification-kit) This is an often overlooked gem. If you have a .NET libary etc and want to know how much of you code depends on non UWP API, this tool can help.

![Windows 10 SDK](https://developer.microsoft.com/en-us/windows/downloads/windows-10-sdk) This is required, but included with VS 2015. 
![Mobile Emulator](https://msdn.microsoft.com/windows/uwp/debug-test-perf/test-with-the-emulator)

![HoloLens](https://developer.microsoft.com/en-us/windows/holographic/development_overview) Get the tools you need to build apps for Windows, including holographic apps. There is no separate SDK for HoloLens; holographic app development uses Visual Studio 2015 Update 3 with the Windows 10 SDK (version 1511 or later). Don't have a HoloLens? You can install the ![HoloLens emulator](https://developer.microsoft.com/en-us/windows/holographic/using_the_hololens_emulator) to build holographic apps without a HoloLens. We also recommend installing the Unity game engine as an easy way to get started creating holographic apps.

![Multilingual app toolkit](https://developer.microsoft.com/en-us/windows/develop/multilingual-app-toolkit)

![Badges](https://developer.microsoft.com/en-us/store/badges) create the HTML and get the artwork needed to promote your apps and content

![Microsoft Store Services SDK](https://visualstudiogallery.msdn.microsoft.com/229b7858-2c6a-4073-886e-cbb79e851211) Create A/B tests that you can run and manage in Dev Center. Launch Feedback Hub so customers can submit feedback and upvotes that you can review in Dev Center. Use the advertising APIs to display banner ads and video interstitial ads.

![OneDrive API 2.0](https://dev.onedrive.com/index.htm)

![Azure-adding a cloud backend to your mobile app](https://azure.microsoft.com/en-us/documentation/services/app-service/mobile/)

![Where is the DirectX SDK?](https://msdn.microsoft.com/library/windows/desktop/ee663275.aspx) DirectX is now a fundamental part of Windows.Starting with Windows 8, the DirectX SDK is included as part of the Windows SDK. We originally created the DirectX SDK as a high-performance platform for game development on top of Windows. As DirectX technologies matured, they became relevant to a broader range of applications. Today, the availability of Direct3D hardware in computers drives even traditional desktop applications to use graphics hardware acceleration. In parallel, DirectX technologies are more integrated with Windows. 

![Microsoft Lumia SDKs](https://developer.microsoft.com/en-us/windows/featured/lumia) SensorCore SDK 1.2 Preview & Imaging SDK 3.0

![VM - Get a Windows 10 development environment](https://developer.microsoft.com/en-us/windows/downloads/virtual-machines) Run this VM on your current Mac or PC for an evaluation of the Universal Windows Platform tools and technologies

![Windows 10 IoT Core](https://developer.microsoft.com/en-us/windows/iot/Downloads.htm#Win8)




### ![Code samples](https://developer.microsoft.com/en-us/windows/samples)

![Windows Universal Samples](http://github.com/Microsoft/Windows-universal-samples)This is is the main repo of Microsoft UWP samples. A multitude of tiny code bits showing every part of UWP.

![Windows.UI.Composition](https://github.com/Microsoft/WindowsUIDevLabs) With the deceptive name of "Windows UI dev labs" this repo contains code samples, demos, experiments, prototypes, and preview explorations that show how to use Windows.UI.Xaml and Windows.UI.Composition to make beautiful UWP applications. 

![Win2D](https://github.com/Microsoft/Win2D/archive/master.zip) Win2D is an easy-to-use Windows Runtime API for immediate mode 2D graphics rendering with GPU acceleration. It is available to C# and C++ developers, and utilizes the power of Direct2D, integrating seamlessly with XAML and CoreWindow.

![DirectX 12 graphics samples](https://github.com/Microsoft/DirectX-Graphics-Samples) DirectX 12 Graphics samples that demonstrate how to build graphics intensive applications on Windows.

![Windows task snippets](https://github.com/Microsoft/Windows-task-snippets) Snippets of ready-to-use code that accomplish small, but useful, tasks of interest to UWP app developers. These snippets show simple solutions to common problems, and simple recipes to help you implement new app features.

![Photo Sharing App](https://github.com/Microsoft/Appsample-Photosharing) UWP app sample that demonstrates real-world social media experiences around photo sharing.

![Rss Reader](https://github.com/Microsoft/Windows-appsample-rssreader) A UWP app sample for retrieving RSS feeds and viewing articles, demonstrating adaptive layout and hierarchical navigation patterns.

![Family notes](https://github.com/Microsoft/Windows-appsample-familynotes)


![Hue light controller](https://github.com/Microsoft/Windows-appsample-huelightcontroller)


![Traffic app](https://github.com/Microsoft/Windows-appsample-trafficapp)


![Network helper](https://github.com/Microsoft/Windows-appsample-networkhelper)


![Marble Maze](https://github.com/microsoft/Windows-appsample-marble-maze)


![Office 365 code samples](http://dev.office.com/code-samples) integrating Office 365 data and services into your app

![UWP Community Toolkit](https://aka.ms/uwptoolkit) See description in Controls section


# Information
![awesome-uwp](https://github.com/tomzorz/awesome-uwp) Awesome UWP resources - inspired by Awesome .NET. - It appears to be a normal "awesome-style" "curated" list whereas ![The-UWP-Tools-List](https://github.com/10UWP/The-UWP-Tools-List) is an attempt to include all possibly useful UWP tools and code. Over time, I hope to have just about everything I can find on GitHub and anywhere else so examine all code carefully before using (but the great glory of open source is that the code speaks for itself) and make sure it has a license you are happy with.  

# Frameworks

![MVVM-Sidekick](https://github.com/waynebaby/MVVM-Sidekick) A Modern light-weight MVVM framework based on RX and Await

![MugenMvvmToolkit](https://github.com/MugenMvvmToolkit/MugenMvvmToolkit) Mugen MVVM Toolkit makes it easier to develop cross-platform application using the Model-View-ViewModel design pattern. The Mugen MVVM Toolkit makes extensive use of Portable Class Libraries to provide maintainable cross platform C# native applications.

![mvvmlight](https://github.com/timdetering/mvvmlight) Git mirror of GalaSoft MVVM Light Toolkit (https://mvvmlight.codeplex.com/)

![Prism](https://github.com/PrismLibrary/Prism) Prism is a framework for building loosely coupled, maintainable, and testable XAML applications in WPF, Windows 10 UWP, and Xamarin Forms.

![Caliburn.Micro](https://github.com/Caliburn-Micro/Caliburn.Micro) A small, yet powerful framework, designed for building applications across all XAML platforms. Its strong support for MV* patterns will enable you to build your solution quickly, without the need to sacrifice code quality or testability. http://caliburnmicro.com/

![Okra App Framework](https://github.com/OkraFramework/Okra.Core) The Okra App Framework is designed to support the development of .Net Windows Store applications, in particular those following the MVVM pattern. http://okraframework.github.io

# Database

![EntityFramework](https://github.com/aspnet/EntityFramework) Microsoft's recommended data access technology for new applications in .NET. The ONLY UWP option is SQLite and ![it is a mess](http://ef.readthedocs.org/en/latest/providers/sqlite/limitations.html). ![Getting Started on Universal Windows Platform](http://ef.readthedocs.org/en/latest/platforms/uwp/getting-started.html) (Opinionated Note: "Microsoft's recommended data access technology" has somehow ended up in the damaged situation of SQLite being the ONLY supported target for Microsoft's main thing, the Universal Windows Platform. The insanely stupid SQLite FK mess means that Entity Framework's Magic Unicorn (Migrations) becomes a useless broken technology on the One Microsoft platform that should count as the highest priority effort. UWP without an easy robust Microsoft supported data platform is a Microsoft blind spot that has been a drag on the success of the Win RT platform from the beginning. "You can workaround some of these limitations by manually writing code in your migrations to perform a table rebuild. A table rebuild involves renaming the existing table, creating a new table, copying data to the new table, and dropping the old table. You will need to use the Sql(string) method to perform some of these steps." (https://github.com/aspnet/EntityFramework/issues/329) There is an explanation in this issue: ![ESENT database provider](https://github.com/aspnet/EntityFramework/issues/4423) which probably translates to "please hold" for another few months)  



![SQLite](http://www.sqlite.org/) SQLite is a software library that implements a self-contained, serverless, zero-configuration, transactional SQL database engine. SQLite is the most widely deployed database engine in the world. The source code for SQLite is in the public domain. Microsoft uses SQLite as a core component of Windows 10, and in individual numerous products. ![System.Data.SQLite](https://system.data.sqlite.org/index.html/doc/trunk/www/index.wiki) System.Data.SQLite is an ADO.NET provider for SQLite.  Development and maintenance work is now mostly performed by the SQLite Development Team. The SQLite team is committed to supporting System.Data.SQLite long-term. ![git mirror of SQLite](https://github.com/mackyle/sqlite) - ![DB Browser for SQLite](https://github.com/sqlitebrowser/sqlitebrowser) Official home of the DB Browser for SQLite (DB4S) project. Previously known as "SQLite Database Browser" and "Database Browser for SQLite". Website at: http://sqlitebrowser.org

![Microsoft.Data.Sqlite](https://github.com/aspnet/Microsoft.Data.Sqlite) SQLite implementations of the System.Data.Common interfaces

![sqlite-net](https://github.com/praeclarum/sqlite-net) sqlite-net is an open source, minimal library to allow .NET and Mono applications to store data in SQLite 3 databases. It is written in C# and is meant to be simply compiled in with your projects. It was first designed to work with MonoTouch on the iPhone, but has grown up to work on all the platforms (Mono for Android, .NET, Silverlight, WP7, WinRT, Azure, etc.). Very simple methods for executing CRUD operations and queries safely (using parameters) and for retrieving the results of those query in a strongly typed fashion. Works with your data model without forcing you to change your classes. (Contains a small reflection-driven ORM layer.)

![SQLitePCL.raw](https://github.com/ericsink/SQLitePCL.raw) SQLitePCL.raw is a Portable Class Library (PCL) for low-level (raw) access to SQLite. This library is designed to be the common portable layer upon which friendlier wrappers can be built. Right now, every C# SQLite library writes their own P/Invoke and COM and marshaling and stuff. Build on this library instead and focus more on the upper layer and its goal of providing a pleasant, easy-to-use API for app developers. When people ask me to recommend a friendlier SQLite wrapper, sqlite-net is the one that I usually recommend. SQLitePCL.pretty is another friendly SQLite API wrapper. 

![SQLitePCL.pretty](https://github.com/bordoley/SQLitePCL.pretty) This library wraps the C like SQLiteAPI provided by SQLitePCL.raw with a friendly C# object oriented API. It adds an Async API. SQLitePCL.pretty has a very simple table mapping ORM, available in the SQLitePCL.pretty.Orm package on nuget. It supports inserting both new and existing objects, and finding and deleting objects by primary key, from SQLite database tables. Notably, the ORM is designed to make working with immutable data types much easier by supporting the builder pattern for deserializing database objects. Ineresting features include the ability to iterate through query result sets using LINQ, support for binary streaming of data in and out of SQLite using .NET streams, and a powerful async API built on the RX framework."

![ESENT](https://msdn.microsoft.com/EN-US/library/gg269181%28v=exchg.10%29.aspx) Extensible Storage Engine is built into and is available for use on every Windows computer and has been an approved DLL for Windows Store since Windows 8.0. Updates to the database are implemented with a transaction in order to ensure secure operations. ESE enables simultaneous access to multiple databases, including transaction-log file databases that can be used for system recovery. ESE is scalable to large or small applications. ![ESENT Managed Interop](https://managedesent.codeplex.com/) it is not clear if the .NET wrapper is UWP compatible."It is clear. ESENT Managed Interop is compatible with UWP. Not all nuget package are, but core Interop package on nuget is compatible with UWP, I tested it myself and it work." Thanks to ![Opiumtm](https://github.com/Opiumtm) for testing that.

![BrightstarDB](https://github.com/BrightstarDB/BrightstarDB) BrightstarDB is a native .NET RDF triple store. It uses dotNetRDF to provide support for a wide range of RDF syntaxes as well as SPARQL query support. In addition to providing a raw RDF-based API, BrightstarDB also provides support for binding RDF resources to .NET dynamic objects; and a contract-first entity framework that enables the use of LINQ rather than SPARQL for query purposes.

![MarcelloDB](https://github.com/markmeeus/MarcelloDB) .net/mono/xamarin/winrt in-process object database. MarcelloDB is a mobile NoSql database. It is very light-weight with minimal memory footprint. MarcelloDB saves plain C# objects, including child objects, lists and collections. Not having to map your objects to the relational model can save you hundreds of lines of code. MarcelloDB is a pure C# implementation, so there is no need to package other binaries.

![Couchbase](https://github.com/couchbase/couchbase-lite-net) - http://www.couchbase.com/ - http://developer.couchbase.com/mobile/ - The NoSQL database solution for mobile — everything you need to build always-available apps that work online & offline. Couchbase Lite is
a fully functional, on-device, lightweight, native, embedded NoSQL database. With Couchbase Lite, you have the full power of a Couchbase database locally on the device. You can create, update, delete, query, sync and much, much more.

#### Note:
Based on this GitHub issue: https://github.com/couchbase/couchbase-lite-net/issues/535 - Couchbase Lite for .NET will be available soon for UWP. "my goal is to still have it in 2016. After the 1.3 release we are going to assess platform support going forward (including the possibility of dropping some, which would free up time for UWP)."

![LiteDB](https://github.com/mbdavid/LiteDB) - http://www.litedb.org/-LiteDB - A .NET NoSQL Document Store in a single data file

####Note:
Based on this GitHub issue: https://github.com/mbdavid/LiteDB/issues/146 - LiteDB is coming for UWP but probably not for quite a while.

![DBreeze](https://github.com/hhblaze/DBreeze) - http://dbreeze.codeplex.com/ - Professional, open-source, NoSql (embedded Key / Value storage), transactional, ACID-compliant, multi-threaded, object database management system for
.NET 3.5> / XAMARIN MONO / .NET Core / UWP (Universal Windows Platform). Written in C# .






#Data Other

![YAWL.Serialization](https://github.com/YAWL/YAWL.Serialization) Serialization helper library for Windows applications

![ObservableSettings](https://github.com/joseangelmt/ObservableSettings) Create a Settings class for UWP (Universal Windows Platform) that is observable, strongly typed and with default values.

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

![CompositionAnimations](https://github.com/Sergio0694/UICompositionAnimations) A wrapper PCL for the Windows.UI.Composion animations

![WinCompositionTiltEffect](https://github.com/r2d2rigo/WinCompositionTiltEffect) A behavior for adding a tilt effect to any UWP control, implemented using Windows Composition.

![UWP-Composition-Radial-Gauge](https://github.com/XamlBrewer/UWP-Composition-Radial-Gauge) A XAML Radial Gauge Custom Control for UWP that is partially drawn by the Composition API. It uses the release version of Composition API, so this requires Requires Visual Studio 2015 update 1 and Windows 10 10586 SDK on your side. A blog post that explains the code is right here: https://xamlbrewer.wordpress.com/2016/01/23/building-a-custom-uwp-control-with-xaml-and-the-composition-api/.

![CompositionHelper](https://github.com/higankanshi/CompositionHelper)

![CompositionAPI](https://github.com/agangal/CompositionAPI)

# Controls

![UWPCommunityToolkit](https://github.com/Microsoft/UWPCommunityToolkit) Microsoft has assembled a few Controls, many of them from other projects on this list, and other misc helper libs for UWP programming. At the moment, it is far less ambitious in scope than their Template 10 project, yet for some reason they have heavily promoted this Community Toolkit both with press releases and featuring on their ![Developer website](https://developer.microsoft.com/en-us/windows/samples). The ![UWPCommunityToolkit-docs](https://github.com/Microsoft/UWPCommunityToolkit-docs) is a separate GitHub project which feeds this ![Microsoft.com Windows Dev site](https://developer.microsoft.com/en-us/windows/uwp-community-toolkit). There is a ![Sample App in Windows Store](https://www.microsoft.com/store/apps/9nblggh4tlcq) that allows you to see exactly what is in the kit. 

There is no mention of any Blend specific features or add-ons but there is an instruction on ![how to add the kit to the VS 2015 Designer Toolbox](https://developer.microsoft.com/en-us/windows/uwp-community-toolkit/toolbox).

For some reason Windows Composition is missing in action for this kit. IMO, both Windows Composition and Win2D are unique Microsoft UWP technologies that can make the platform exciting and are natural candidates for this Microsoft showcase.

Controls:

    AdaptiveGridView
    HamburgerMenu
    HeaderedTextBlock
    ImageEx
    PullToRefreshListView
    RadialGauge
    RangeSelector
    RotatorTile
    SlideableListItem


![UniversalMarkdown](https://github.com/QuinnDamerell/UniversalMarkdown) A markdown parsing and rendering library for C# and Windows Universal Apps http://baconit.quinndamerell.com/ Universal Markdown is your one-stop-shop for all of your markdown needs in C#. Universal markdown was built for the open source reddit app Baconit, but hopefully it will be adopted by others and improved by the community. 

![WinRT-StandardDateFormatPicker](https://github.com/ignacy130/WinRT-StandardDateFormatPicker) Simple control based on ComboBoxes to pick date in common in Europe and most of the world format dd-mm-yyyy. Wiki: https://github.com/ignacy130/WinRT-StandardDateFormatPicker/wiki

![RichTextBlock.Html2Xaml](https://github.com/MacawNL/WinRT-RichTextBlock.Html2Xaml) The WinRT RichTextBlock control serves to display read-only rich formatted text. However, it supports a limited subset of XAML, and no HTML. In scenario's where you want to display a field that contains HTML rich formatted text (e.g. when you have clients on multiple platforms, such as web, WinRT, iOS and Android), this package offers an alternative to using an embedded browser control. Using a browser control impacts performance and limits the UI experience (e.g. the WebView control does not support transparency). RichTextBlock.Html2Xaml adds an Html extension property to RichTextBlock controls, that you can set (or data bind) to a string containing an Html snippet.

![Mntone WinRT Library](https://github.com/mntone/WinRtLibrary) This is my useful library for UWP and Windows Store app - UI.Xaml.Controls - TypedDataTemplateSelector - VisualTreeHelper2


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

![WinRT_Calendar](https://github.com/bak301/WinRT_Calendar)

# UI
![ReactiveUI](https://github.com/reactiveui/ReactiveUI) A MVVM framework that integrates with the Reactive Extensions for .NET to create elegant, testable User Interfaces that run on any mobile or desktop platform. Supports Xamarin.iOS, Xamarin.Android, Xamarin.Mac, Xamarin Forms, WPF, Windows Forms, Windows Phone 8, Windows Store and Universal Windows Platform (UWP). http://www.reactiveui.net

![userdialogs](https://github.com/aritchie/userdialogs) A cross platform library that allows you to call for standard user dialogs from a shared/portable library, Actionsheets, alerts, confirmations, loading, login, progress, prompt, toast... async just for fun. Supports Android, iOS, Windows Phone 8.0 (silverlight), and Unified Windows Platform (UWP, UAP)

![BlendrocksToolkit](https://github.com/deanihansen/BlendrocksToolkit) Windows UWP toolkit that which enabled insanely cool page transitions and easier navigation and app handling.

![Monolith](https://github.com/ThatLousyGuy/Monolith) Monolith is a Windows library that lets you create animations in codebehind in a fluent, somewhat straightforward manner. It's a wrapper around the Windows.UI.Xaml.Media.Animation library that removes as much of the setup as possible. (Thanks to ![Awesome UWP resources list](https://github.com/tomzorz/awesome-uwp) for the head's up on this interesting project.

![WindowsStateTriggers](https://github.com/dotMorten/WindowsStateTriggers) A collection of custom visual state triggers


# Libs UWP

Libraries that may support UWP specific features.

![Groves](https://github.com/tomzorz/Groves) A UWP library by the author of the ![Awesome UWP resources list](https://github.com/tomzorz/awesome-uwp) 

![YAWL.Composition](https://github.com/YAWL/YAWL.Composition) Composable building blocks for MVVM based Windows 10 applications

![observable-vector](https://github.com/jamesqo/observable-vector) A no-frills implementation of IObservableVector for Windows 10 apps.

![Shims.Xaml](https://github.com/jamesqo/Shims.Xaml) Easily create libraries that work on both WPF and Windows 10.

![XamlBehaviors](https://github.com/Microsoft/XamlBehaviors) This is the official home for XAML Behaviors on GitHub. XAML Behaviors is an easy-to-use means of adding common and reusable interactivity to your Windows UWP applications with minimal code. It is available for both native and managed applications.

![Portable.Xaml](https://github.com/cwensley/Portable.Xaml) Portable .NET library for reading/writing xaml files. This is intended to be used to read Xaml on desktop, mobile, and CoreCLR platforms.

![typed-xaml](https://github.com/jamesqo/typed-xaml) Advanced generics support for WPF and Windows 10.

![uwp-chrome](https://github.com/RReverser/uwp-chrome) Experimental chrome API shim for Universal Windows Platform (UWP / WinRT)

![UWP-Helpers](https://github.com/EdiWang/UWP-Helpers) Helpers and Utils for UWP Projects

![Kulman.UWP](https://github.com/igorkulman/Kulman.UWP) Collection of utilities and services for UWP apps

![MyToolkit](https://github.com/MyToolkit/MyToolkit) MyToolkit for .NET http://mytoolkit.io MyToolkit is a set of .NET libraries containing lots of useful classes for various .NET platforms like UWP/WinRT (Universal Windows Apps), Windows Phone and WPF. The goal is to provide missing or replace existing classes to support the development of high-quality Windows and Windows Phone applications. For example, the library provides often used MVVM infrastructure classes, missing UI controls, IoC classes, additional LINQ extension methods and much more.

![Cimbalino-Toolkit](https://github.com/Cimbalino/Cimbalino-Toolkit) Cimbalino Toolkit http://cimbalino.org Cimbalino Toolkit is a set of useful and powerful tools that will help you build your Windows Platform applications.

![cadru](https://github.com/scottdorman/cadru) A Microsoft .NET Framework toolkit http://scottdorman.github.io/cadru Cadru is a utility framework containing new APIs and extensions to the core .NET Framework to help complete your developer toolbox. It is designed to be portable first, which means that the majority of the library is available as a Portable Class Library (PCL) 

![Windows-task-snippets](https://github.com/Microsoft/Windows-task-snippets) This repo collects snippets of ready-to-use code that accomplish small but useful tasks of interest to Universal Windows Platform (UWP) app developers. These snippets represent simple solutions to common problems, and simple recipes to help you implement new app features. 

![UWP-Networking-Essentials](https://github.com/SvenEV/UWP-Networking-Essentials) Simple and lightweight networking (including RPC) for Universal Windows Platform apps

![ComposableAdaptiveTriggerDemo](https://github.com/LocalJoost/ComposableAdaptiveTriggerDemo) Demo of a AdaptiveTrigger that works with a StateTrigger inside a CompositeStateTrigger from WindowsStateTriggers

![YAWL.Common](https://github.com/YAWL/YAWL.Common) Common library for all new Windows Phone/Store/UWP/Mobile and Xamarin applications

![WinRT.IncrementalLoadingCollection](https://github.com/AhmedMabrouck/WinRT.IncrementalLoadingCollection) A Windows Runtime custom collection that supports observability and incremental loading out of the box.

![inflatable-toolkit](https://github.com/inflatablefriends/inflatable-toolkit) Stuff we use a lot in WinRT apps

![bigint-winrt](https://github.com/robpaveza/bigint-winrt) A Windows Runtime API for big integers. The source BigInteger implementation is forked from https://github.com/kurmasz/bigint which is based on the bigint library by Matt McCutchen. 

![MetroLog](https://github.com/onovotny/MetroLog) MetroLog is a lightweight logging framework designed for Windows Store and Windows Phone 8 apps. Although the API is based on NLog and log4net, the intention is that it's a very basic logging system. 
The need for it to be basic comes from the fact that the Windows Store apps API surface area intentionally limited for very specific applications. This project came out of the fact that porting NLog to Windows Store apps is difficult because of it's incredibly rich feature set, most of which is not workable in Windows Store apps.

![WinRTTimeZones](https://github.com/onovotny/WinRTTimeZones) Simple Time Zone conversion for WinRT, Windows Store and Windows Phone 8 apps

# Libs General

Libraries that are compatible with UWP but don't provide UWP specific feature support.


![Bex](https://github.com/ScottIsAFool/Bex) A PCL for accessing the MS Health Web APIs. For usage and an overview, please go to http://metronuggets.com/2015/07/10/introducing-bex-a-pcl-library-for-the-ms-health-apis/

![Shim](https://github.com/cureos/shim) Shim provides reduced or dummy implementations of .NET Framework types that are currently not represented in PCL, thereby expanding the ability to create Portable Class Libraries from legacy code.

![InternalContainer.cs](https://github.com/dshe/InternalContainer.cs) A simple IoC container in a single C# 6.0 portable class library (PCL) source file.

![Portable WebDAV Library](https://github.com/DecaTec/Portable-WebDAV-Library) Portable WebDAV Library is a fully RFC 4918 compliant WebDAV client library which is implemented das portable class library (PCL) for use on desktop environments as well as mobile devices. https://decatec.de

![Websockets.PCL](https://github.com/NVentimiglia/Websockets.PCL) C# Websockets for all platforms using native bridges

![sockets-for-pcl](https://github.com/rdavisau/sockets-for-pcl) Cross-platform socket API for Xamarin iOS/Android/Forms, Xamarin.Mac/MonoMac, Windows Phone 8/8.1, Windows Store and Windows Desktop.

![Polly](https://github.com/App-vNext/Polly) Polly is a .NET 3.5 / 4.0 / 4.5 / PCL library that allows developers to express transient exception handling policies such as Retry, Retry Forever, Wait and Retry or Circuit Breaker in a fluent manner.

![PCLStorage](https://github.com/dsplaisted/PCLStorage) PCL Storage provides a consistent, portable set of local file IO APIs for .NET, Windows Phone, Windows Store, Xamarin.iOS, Xamarin.Android, and Silverlight. This makes it easier to create cross-platform .NET libraries and apps.

![PCLCrypto](https://github.com/AArnott/PCLCrypto) PCLCrypto is an open source library that provides portable class library authors with cryptographic APIs that invoke platform-specific crypto automatically.

![BouncyCastle-PCL](https://github.com/onovotny/BouncyCastle-PCL) PCL Version of BouncyCastle targetting .NET, SL, WP, WinRT, .NET Core and CoreCLR. The Bouncy Castle Crypto package is a C# implementation of cryptographic algorithms and protocols, it was developed by the Legion of the Bouncy Castle, a registered Australian Charity, with a little help! The Legion, and the latest goings on with this package, can be found at http://www.bouncycastle.org. In addition to providing basic cryptography algorithms, the package also provides support for CMS, TSP, X.509 certificate generation and a variety of other standards such as OpenPGP.

![BCLExtensions](https://github.com/csMACnz/BCLExtensions) Base Class Library Extensions for C# base class library classes, across .Net, Silverlight, WinRT. You can view the list if extensions available and future extensions to come on the ![Extensions Wiki Page](https://github.com/csMACnz/BCLExtensions/wiki/Extensions).

![ExcelReader-WinRT](https://github.com/BananaScheriff/ExcelReader-WinRT) Excel sheets reader for Uniwersal Windows Platform

![ValidatableBase](https://github.com/scionwest/ValidatableBase) Model Validation for Universal WinRT Apps through delegate method invocation per-property or DataAnnotation styled attribute validation. Added validation interception support. You may now have the built-in validation rules invoke a delegate method. This provides you with a little more flexibility when performing validation. You may piggy back on top of existing rules for minor checks instead of resorting to a full delegate validation method. By letting your model inherit from ValidatableBase, you can force validation checks on a model from within your view model. Binding to the view is really easy, using one of the two provided converters. The library comes with support for validating minimum and maximum numeric values, ranges of numeric values, string length, null objects, empty collections, empty or null strings and custom delegate method invocation. If you want to write your own attribute validation, you just need to implement IValidationRule and then decorate your object.


# Media
![MediaFoundation](https://github.com/AndrewGaspar/MediaFoundation) Some helper functions for WinRT for getting media information about some URL

![FFMPEGHelper](https://github.com/krishnan-unni/FFMPEGHelper) Windows 10 Universal WinRT component for FFMPEG library

# Graphics 2D
![Win2D](https://github.com/Microsoft/Win2D) Win2D is an easy-to-use Windows Runtime API for immediate mode 2D graphics rendering with GPU acceleration. It is available to C# and C++ developers writing Windows apps for Windows 8.1, Windows Phone 8.1 and Windows 10. It utilizes the power of Direct2D, and integrates seamlessly with XAML and CoreWindow. http://microsoft.github.io/Win2D (https://github.com/Microsoft/Win2D-Samples)

![SvgForXaml](https://github.com/mntone/SvgForXaml) Draw image from svg file with Win2D

![XamlAnimatedGif](https://github.com/XamlAnimatedGif/XamlAnimatedGif) A simple library to display animated GIF images in XAML apps (WPF, WinRT, Windows Phone)

![GifImageSource](https://github.com/sskodje/GifImageSource) GifImageSource is a Windows Runtime Component for WinRT projects, made for rendering GIF images in a resource efficient way using Direct2D.


![WriteableBitmapEx](https://github.com/teichgraf/WriteableBitmapEx) The WriteableBitmapEx library is a collection of extension methods for the WriteableBitmap. The WriteableBitmap class is available for all XAML flavors including Windows Phone, WPF, WinRT Windows Store XAML, (Windows 10) UWP and Silverlight. It was even ported to Windows Embedded. WriteableBitmapEx allows the direct manipulation of a bitmap and can be used for image manipulation, to generate fast procedural images by drawing directly to a bitmap and more. The WriteableBitmap API is very minimalistic and there's only the raw Pixels array for such operations. The WriteableBitmapEx library tries to compensate that with extensions methods that are easy to use like built in methods and offer GDI+ like functionality. The library extends the WriteableBitmap class with elementary and fast (2D drawing) functionality, conversion methods and functions to combine (blit) WriteableBitmaps. The extension methods are grouped into different C# files using a partial class approach. It is possible to include just a few methods by using the specific source code files directly or the full functionality via the built binaries. 

![ImagingUWP](https://github.com/asiertarancon/ImagingUWP) UWP app with Lumia Imaging SDK

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

# Game Dev

![MonoGame](https://github.com/mono/MonoGame) One framework for creating powerful cross-platform games. http://www.monogame.net MonoGame is an open source implementation of the Microsoft XNA 4.x Framework. Our goal is to make it easy for XNA developers to create cross-platform games with extremely high code reuse.

![MonoGame.Extended](https://github.com/craftworkgames/MonoGame.Extended) MonoGame.Extended is a portable class library designed to build on top of MonoGame. It may work also with XNA/FNA (not confirmed) and it should work on other platforms like Xamarin Android or iOS. If you do use it on another platform please let us know!

![FarseerPhysics.Portable](https://github.com/craftworkgames/FarseerPhysics.Portable) This is a fork of the Farseer Physics Engine found on codeplex with a few minor changes to make it work as a Portable Class Library (PCL) with the PCL version of MonoGame.

![Xenko Game Engine](https://github.com/SiliconStudio/xenko) Xenko is a powerful cross-platform game engine. Enjoy the latest features of .NET 4.6 and C#6 to write stunning games efficiently! Import your assets and build your world using the Game Studio. Create scripts with Microsoft Visual Studio and bring your game to life! Xenko is available for free using a dual license system and its source code is available on GitHub. ![Xenko.com](http://xenko.com/) - ![Xenko Samples](https://github.com/SiliconStudio/xenko-samples) - ![Features](http://xenko.com/features/) -  ![Platforms](http://xenko.com/features/platforms/)

![Unity](https://unity3d.com/)  - ![Get Unity](https://unity3d.com/get-unity) -  ![Platforms](https://unity3d.com/unity/multiplatform) Also supports Microsoft Hololens.

# Language

![The Visual F# compiler and tools](https://github.com/Microsoft/visualfsharp) F# is a mature, open source, cross-platform, functional-first programming language which empowers users and organizations to tackle complex computing problems with simple, maintainable, and robust code. F# is used in a wide range of application areas and is supported by Microsoft and other industry-leading companies providing professional tools, and by an active open community. You can find out more about F# at http://fsharp.org.

# Testing

Opinionated Note: Testing is valuable but Unit Testing is a social meme associated with the always hard to pin down Agile movement but despite my dislike of meme-driven-development, I'll include UWP focused Unit Testing since you need to jump thru extra hoops on top of the already rediculous monkey hoops and various perversions of Object Design in order to make your CI robot lamp glow green on UWP...

![myweather](https://github.com/fernandoescolar/myweather) This is a demo of unit testing in UWP. It contains a T4 template to generate all the Spies, Stubs and Mocks of all the interfdaces found in your solution.

![xUnit.net](https://github.com/xunit/xunit) xUnit.net is a free, open source, community-focused unit testing tool for the .NET Framework. Written by the original inventor of NUnit v2, xUnit.net is the latest technology for unit testing C#, F#, VB.NET and other .NET languages. xUnit.net works with ReSharper, CodeRush, TestDriven.NET and Xamarin. It is part of the ASP.NET Open Source Gallery under the Outercurve Foundation, licensed under Apache 2 (an OSI approved license). ![Getting Started with xUnit.net (Universal Windows Apps)](http://xunit.github.io/docs/getting-started-uwp.html)

![xunit-performance](https://github.com/Microsoft/xunit-performance) Provides extensions over xUnit to author performance tests.

![PCLMock](https://github.com/kentcb/PCLMock) PCLMock is a simple mocking framework in a Portable Class Library. Existing mocking frameworks, such as Moq, do not work on platforms running a limited subset of the .NET framework. Writing mocks without the aid of a framework is laborious, error-prone, and results in inconsistent code. PCLMock aims to reduce this pain.

![FluentAssertions](https://github.com/dennisdoomen/FluentAssertions) Fluent Assertions is a set of .NET extension methods that allow you to more naturally specify the expected outcome of a TDD or BDD-style test. We currently use it in all our internal and client projects, and it is used in many open-source projects. It runs on .NET 4.0, 4.5, 4.6, CoreClr, .NET Native, Windows 8.1, Silverlight 5, Windows Phone 8.0… http://www.fluentassertions.com

![FluentAssertionsEx](https://github.com/hivepeople/FluentAssertionsEx) Extensions for FluentAssertions.

![FluentAssertions.Autofac](https://github.com/awesome-inc/FluentAssertions.Autofac) Fluent Assertions extensions for Autofac

![Shouldly](https://github.com/shouldly/shouldly) Should testing for .net - the way Asserting *Should* be! http://shouldly.readthedocs.org/en/latest




# Samples


![Windows-universal-samples](https://github.com/Microsoft/Windows-universal-samples) Official API samples for the Universal Windows Platform.

![HealthClinic.biz](https://github.com/Microsoft/HealthClinic.biz) The samples contained in this repo are used to present an end-to-end demo scenario based on a fictitious B2B and multitenant system, named “HealthClinic.biz” that provides different websites, mobile apps, desktop apps, wearable apps, and services running on the latest Microsoft and open technologies aligned with announcements to showcase during … http://aka.ms/Connect

![UWPQuickStart](https://github.com/Microsoft/UWPQuickStart) Building a Universal Windows app in Visual Studio is quick and easy. We've provided a sample app that you can download and learn how the various pieces fit together. We even encourage you to customize and send a version of this app to the Windows Store!

![Windows-appsample-quizgame](https://github.com/Microsoft/Windows-appsample-quizgame) A peer-to-peer trivia game sample for the Universal Windows Platform (UWP). 

# Samples That Don't Hurt Your Eyeballs

There are lots of UWP App samples but most of them look like crap either because they are meant to demo a Windows 10 UWP feature or else total lack of aesetic sense. This section will give you some hope that one day the Windows Store won't be full of junk.

![Baconit](https://github.com/QuinnDamerell/Baconit) A beatiful, powerful, reddit client for Windows 10. https://www.reddit.com/r/BaconitDev/ The highest rated reddit client for Windows Phone has been rewritten from the ground up and is now available for all Windows 10 devices. Now with a dynamic new UI, faster speeds, and features you have been asking for. Welcome to the new Baconit. We know you’re going to love it.

