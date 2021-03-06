# Compute Resource Consolidation Pattern

This document describes the Compute Resource Consolidation Pattern example from the guide [Cloud Design Patterns](http://aka.ms/Cloud-Design-Patterns).

## System Requirements
* Microsoft .NET Framework version 4.5
* Microsoft Visual Studio 2015 Community, Enterprise, or Professional
* Windows Azure SDK for .NET version 2.9

## Before you start

Ensure that you have installed all of the software prerequisites.

The example demonstrates operational aspects of applications running in Windows Azure. Therefore, you will need to use the diagnostics tools in order to understand how the code sample works. You must ensure that the web and worker roles in the solution are configured to use the diagnostics mechanism. If not, you will not see the trace information generated by the example.

## About the Example

This example shows how you can consolidate several separate and distinct tasks into a single worker role.


## Running the Example

You can run this example locally in the Visual Studio Windows Azure emulator. You can also run this example by deploying it to a Windows Azure Cloud Service.

 
* Start Visual Studio using an account that has Administrator privileges ("Run as Administrator").
* Open the solution you want to explore from the subfolders where you downloaded the examples.
* Right-click the role in Solution Explorer, select Properties, and ensure that is configured to generate diagnostic information.

* If you want to run the example in the local Windows Azure emulator:
	* Press F5 in Visual Studio to start the example running. 
	* Open the Windows Azure Compute Emulator UI from the icon in the notification area.
	* Select the role and view the diagnostic information generated by Trace statements in the code.
* If you want to run the example on Windows Azure:
	* Provision a Windows Azure Cloud Service and deploy the application to it from Visual Studio. 
	* Open the Server Explorer Window in Visual Studio and expand the Windows Azure entry.
	* Expand Cloud Services and then expand the entry for the solution you deployed.
	* Right-click the role instance and select View Diagnostics Data to see the diagnostic information generated by Trace statements in the code. This is written to the WADLogsTable in the Storage/Development/Tables section.

