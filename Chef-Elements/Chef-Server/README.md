# Chef Server

The Chef Server is the "central" element that manages communication in Chef. It is written in Erlang. 

### Key Features

**Configuration Policies**

Chef Server acts as a central repository of configuration policies for nodes and cookbooks.

**Metadata**

Chef Server stores detailed metadata of the registered components, the components that register with the Chef server. 

**Storage and Search**

Chef server uses PostgreSQL as a data storage repository. 
It uses indexing to maintain search indexes which facilitates in searching any type of data. 
