# Mission Reflection

This activity helped me understand why choosing the right storage type is important for an application. If a system needs to store millions of photos, Object Storage is more suitable than depending only on a traditional block storage hard drive. Photos are unstructured data, and Object Storage is designed to handle large collections of this kind of content.

Using Docker made the MinIO deployment easier because the storage server could be started through a command instead of installing and configuring everything separately. I was able to provide the required ports, credentials, container name, and server settings during the deployment. This also helped me understand how Docker can be used for services other than a simple web application.

Creating the `client-photos` bucket made the meaning of a bucket clearer to me. It works as a container where objects can be stored and organized. After uploading a sample file, I was able to see how an object is actually placed inside cloud storage instead of only learning about it through a definition.

For large companies, keeping important information on only one physical server can create a problem if that server fails. Redundancy can help by maintaining copies of data on multiple servers or locations. Backup and replication can also help keep stored information available during hardware problems.

I am becoming more familiar with the Linux command line as I complete more laboratory activities. I still need to read commands carefully, but I now understand more of the output from Git and Docker. This activity also gave me more practice solving small problems instead of immediately starting the entire process again when something did not work.
