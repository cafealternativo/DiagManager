# What is Pssdiag/Sqldiag Manager?
[![licence badge]][licence]
[![stars badge]][stars]
[![forks badge]][forks]
[![issues badge]][issues]

[licence badge]:https://img.shields.io/badge/license-MIT-blue.svg
[stars badge]:https://img.shields.io/github/stars/Microsoft/DiagManager.svg
[forks badge]:https://img.shields.io/github/forks/Microsoft/DiagManager.svg
[issues badge]:https://img.shields.io/github/issues/Microsoft/DiagManager.svg

[licence]:https://github.com/Microsoft/DiagManager/blob/master/LICENSE.md
[stars]:https://github.com/Microsoft/DiagManager/stargazers
[forks]:https://github.com/Microsoft/DiagManager/network
[issues]:https://github.com/Microsoft/DiagManager/issues

Pssdiag/Sqldiag Manager is a graphic interface that provides customization capabilities to collect data for SQL Server using sqldiag collector engine. The data collected can be used by [SQL Nexus tool](http://sqlnexus.codeplex.com/)  which help you troubleshoot SQL Server performance problems.  This is the same tool Microsoft SQL Server support engineers use to for data collection to troubleshoot customer's performance problems.

## Current Release
 https://aka.ms/get-pssdiag


### What's New
This version support SQL Server 2016, 2017, 2019 as well previous versions
[More in wiki...](https://github.com/Microsoft/DiagManager/wiki/What's-New)


### **Requirements**
1. Diag Manager requirements
  - Windows 7 or Windows 10 (32 or 64 bit)
  - .NET 4.5 
2. Data collection
  - The collector can only run on a machine that has SQL Server with targeted version (either client tools only or full version) installed


### **Installation**
Download it from release tab or [click here](https://github.com/microsoft/DiagManager/releases/) to download.  Source files are also included in the release tab.

### **Known Issues**
[see known issues wiki](Known Issues)

## **How to use DiagManager**
[See getting started wiki](https://github.com/Microsoft/DiagManager/wiki/Getting-Started)

## How it works
This tool lets you customize what you want to collect and then let you create a data collection package. You extract the package and run SQLdiag data collector engine on the SQL Server you are troubleshooting.

## Feature Highlights

1. **Powerful data collection capabilities:** The tool relies on SQLdiag collector engine to provide collection of perfmon, profiler trace, msinfo32, errorlogs, Windows event logs, TSQL script output and registry exports.
2. **Default templates/scenarios:** You can choose SQL Server version and platform (32 bit or 64 bit). The tool will automatically choose a default template for the combination. This will have default set of perfmon counters, profiler traces.
3. **Shipped with ready to use Custom collectors:** Most commonly used [custom collectors](https://github.com/Microsoft/DiagManager/wiki/Custom-Collector) include SQL Server 2005, 2008 or 2008 R2 performance collector.
4. **Customization/Extensibility:** You can customize what perfmon and profiler trace events you want to collect. Additionally, you can create your own custom collectors with TSQL Scripts, batch files and utilities.   See [customization guide](https://github.com/Microsoft/DiagManager/wiki/Creating-Custom-Collectors).
5. **Packaging:** With a single click of save, the tool will package all your files into a single cab so that you can ship to the machine where you intend to execute it.
6. **Integration with SQL Nexus** :  The custom collectors shipped will collect data that can be analyzed by [SQL Nexus Tool](https://github.com/Microsoft/SqlNexus).


## Common Tasks

1. [Gettting Started](https://github.com/Microsoft/DiagManager/wiki/Getting-Started): This page tells you how to use the tool including installation, configuration and running the tool
2. [Customization guide](http://diagmanager.codeplex.com/wikipage?title=Creating%20Custom%20Collectors): This page tells you how you can create you own custom collector to use in addition to default collectors shipped.
4. [Frequently Asked Questions (FAQ](http://diagmanager.codeplex.com/wikipage?title=FAQ)): This page will answer most commonly asked questions.
5. [Common Issues](https://github.com/Microsoft/DiagManager/wiki/Known-Issues): This page will document most commonly encountered issues and errors

## License Agreement

[MIT License](/license.md)