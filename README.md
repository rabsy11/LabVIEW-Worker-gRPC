# LabVIEW Worker and gRPC

This repository contains the project that use LabVIEW Worker framework to build gRPC server and client.

**LabVIEW Version**

LabVIEW source is saved with LabVIEW 2023 Q1.

**Dependencies**

* LabVIEW Worker  
The example is based on Worker 5.0: [https://www.vipm.io/package/.delacor_lib_dqmh_toolkit/](https://www.vipm.io/package/sc_workers/)

* gRPC LabVIEW libraries and template.  
You need both the base libraries and the server libraries to run the gRPC code. If you’d like to experiment further with the code and modify the proto file, you’ll also need the template package. A archive containing all the required packages is available on this github release [https://github.com/ni/grpc-labview/releases](https://github.com/ni/grpc-labview/releases).

* Protobuf  
The example relies on several of Protocol Buffers’ well-known data types. When re-compiling the gRPC code, these data types must be available. To include them, download and add the Protobuf repository (in Import Path) during the compiling process.You can acceess Protobuf repository in [https://github.com/protocolbuffers/protobuf](https://github.com/protocolbuffers/protobuf).

<div align="center">
<figure>
  <img src="Images/Import Paths Protobuf.png" alt="Import Path" width="400">
  <figcaption>Import Path</figcaption>
</figure>
</div>

**Steps to Run the Worker gRPC Example**

1. Open the LabVIEW projects located in the *Worker gRPC Server* and *Worker gRPC Client* folders.
2. In each project, open and run the *Launcher – xxx.vi* file. This will start all workers.
3. In the gRPC Server program, click *Start* to launch the gRPC server.
4. In the gRPC Client program, click *Start* to connect the gRPC client.
5. Use the *Signal Type*, *Signal Config*, and *Sampling Config* settings to update the configuration on the gRPC Server.
6. Click *Start Acq* to begin the acquisition process.