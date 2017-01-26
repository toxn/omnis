# omnis
Object-oriented Multi-Node Information System

## Concept
Omnis is an environment/plateform meant to bring various technical paradigms to the general user with no specific regard to compatibility with older OSes. Let's review those paradigms.

### 1. Object-Oriented
Omnis doesn't provide applications directly to the user. Programs are a result of a programmer&nbsp;/&nbsp;mathematician approach. In a real-life approach, one will put the project before the tool. In respect to this point of view, the user will be presented with data (projects, objects, resources) instead of programs.

   This paradigm offers many advantages for the user:

#### Branding is masked
User doesn't have to choose between several softwares with varying advantages, Uis or licencing. He want's to create an image; he just selects 'Create new Image'. He wants to modify a video; he just searches for the video and selects 'Modify'. In fact branding is defered to the administrator, who will choose the default class to be used for this or that, install new modules, choose or modify the default UI for each type of datum. More to that, the user doesn't have to remember which program/command does what (please note that this doesn't forbid having data such as 'Command-line session with interpreter X').

#### Software price is reduced to added value
As standard APIs evolve, the administrator needs just buy the classes that really had some value over free software that become intergrated in the standard APIs. No need to spend money or resources on software that is already available for free and is open and community maintain. Software vendors are incited to provide added value on the object and service levels, which spurs innovation rather than imitation.

#### Lower code duplicity
Objects can be reused, reducing the need to duplicate code, while system-wide inheritanceand polymorphism limit the need to resort to forking.
    
### 2. Persistent
A deep implementation of persistency has a very wide influence on how objects are stored and how the user views them and the whole system.

#### Persistent storage vs volatile
The user often deal with problem relative to memory/storage type. Most of these problems can be seen when dealing when working with users having low or inexistant technical background. But those problems can also affect IT professionals.

##### _Where are my data?_
That's a question frequently asked to technical assistance operators. Wether an application was closed while the changes were not saved, or old data have been erased and can't be retrieved (because of backup policy, change history is presented as linear, etc), or location of saved data is ambiguous or unknown (location forgoetten or masked by a locally mounted shared disk or working on remote display).

##### _Where is my program?_
Many environments tend to hide the launched state of a program, resulting in data losses at extinction, higher energy/battery consumption, multiple launches errors.

##### Omnis provides an elegant solution to all those problems.
* **Data is stored on disk as an object-oriented database**. The legacy hierarchy of directories is replaced with tags and metadata, thus permitting on-the-fly indexation.

* **RAM is only used as a cache**. There is no launched status for a program (programs don't exist anymore), no openned or saved status for a file, no loaded status for a class. The user finds his session on boot as he left it previously, he doesn't need to worry about data being saved or not. Booting is super-fast as every object is automatically persisted to disk when cache is emptied.

* **Copy-on-write mechanism offers a perfect hierarchical undo/redo**. Every change, by every user is persisted as would be in a versioning system and retrievable until a garbage collector redeems the disk space.

### 3. Multi-Node
For a long time information system have been viewed and administered as a collection of separate and self-sufficient boxes. Since the 2000's, this model as exploded with the arrival of three-tiered architecture, ditributing a service on mutliple and redundant servers, of virtual-machines, virtualization and containers, permitting multiple virtual computers to run on the same machine with several degrees of containement.

Omnis proposes to intergrate these advancements in multiple ways.

#### Mutiple presentations
Omnis can be used as a full-fledged operating system, but also as a container, fully isaolated from it's parent system, or as a virtual machine, thus providing a full and standardized access to the functions of the parent system.

#### Data and code sharing
Objects and classes can be shared or duplicated between nodes thus providing replication to ensure data security, and sharing of processing power and storage capacity. Code can be transfered inside a class or in a message as bytecode, thus ensuring compatibility between different architectures on the same network. Shared classes permit the transparent execution of code over a network, providing a perfect balance of computing power repartition.

### 4. Scalable
Evolution of computing tends to promote portable devices. Omnis' multi-node and memory architecture avails running on any hardware environment, ranging from embedded or portable device to workstation to powerfull server.
