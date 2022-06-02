## Azure Blobs

## Introduction to Azure Blob storage
Azure Blob storage is Microsoft's item stockpiling answer for the cloud. Blob stockpiling is upgraded for putting away enormous measures of unstructured information. Unstructured data is data that does not adhere to a specific data model or definition, like text or binary data.


## What Does Blob Storage Mean?
Blob storage is a feature in Microsoft Azure that lets developers store unstructured data in Microsoft's cloud platform. This data can be accessed from anywhere in the world and can include audio, video and text. Blobs are grouped into "containers" that are tied to user accounts. Blobs can be manipulated with .NET code.


## How Does Blob Storage Work
If you are still confused about the Blob storage meaning, don’t worry. Here we draw a picture to explain how does Blob storage work. It comprises 3 different types of storage resources: Storage Account, Container, and Blob.

Storage Account: It is a unique namespace in Microsoft Azure for storing your data. That is to say, each object that your store in Blob Storage has an address that contains your unique account name.
Container: Similar to a directory in File Explorer, the Container organizes a set of blobs. A storage account can contain an unlimited number of containers and a container can store an unlimited number of blobs.
Blob: There are 3 types of blobs, including Block blobs, Append blobs and Page blobs. Each type has different storage supports. For example, the Block blobs can store text and binary data, while the Page blobs store random access files like

![blob-storage-1](https://user-images.githubusercontent.com/98957434/171705923-1881db6e-c54a-4ae4-896d-64a6b4747ebb.jpg)


## Usually, you can use it in the following several scenarios:

1. Serving documents or images directly to a browser
2. Streaming audio and video
3. Writing to log files
4. Storing files for distributed access
5. Storing data for backup and restore, and disaster recovery
6. Storing data for analysis by Azure-hosted service or Azure-hosted service
7. Accessing objects in Blob storage via HTTP/HTTPS from anywhere in the world

