# connect-csharp-samples
Samples of using [Connect Open API](https://connect.spotware.com/documentation/section/api-reference) in C#

## How to get started your own app in C#:
* Download or clone this example
* Open [TradingAPI_samples.sln](https://github.com/spotware/connect-csharp-samples/blob/master/TradingAPI_samples.sln) using MS Visual Studio 2013.
* Restore NuGet dependencies
* Build and run the application

## How to create C# classes from proto files:
* Download C# classes generator from Protocol Buffer sources from here: https://code.google.com/p/protobuf-csharp-port/downloads/list. For this example we used the following pakage: [protobuf-csharp-port-2.4.1.521-release-binaries.zip](https://protobuf-csharp-port.googlecode.com/files/protobuf-csharp-port-2.4.1.521-release-binaries.zip)
* Extract files to your local drive
* Download the latest version of Trading API .proto sources from our online guide: [open-api-proto-lib.zip](https://connect.spotware.com/uploads/open-api-proto-lib.zip)
* Extract them to the same location you have extracted ProtoBuf tools
* Execute "gen_csharp_src.bat" to generate C# sources (.cs files)
* Copy newly generated files to your project. Alternatively you can create a class library project within your solution and copy the .cs files there.
* Link the .cs files to the project adding them to it and/or setting dependencies between your project and the proto library project (in case you have created the library). Add Reference of the Class Library project (if you have it) to your main project.
* Add Reference on "Google.ProtocolBuffers" to the Class Library project (or your main project if you do not have the Class Library project)

