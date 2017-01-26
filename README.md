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

Omnis provides an elegant solution to all those problems.
* Data is stored on disk as an object-oriented database. The legacy hierarchy of directories is replaced with tags and metadata, thus permitting on-the-fly indexation.

* RAM is only used as a cache. There is no launched status for a program (programs don't exist anymore), no openned or saved status for a file, no loaded status for a class. The user finds his session on boot as he left it previously, he doesn't need to worry about data being saved or not. Booting is super-fast as every object is automatically persisted to disk when cache is emptied.

### 3. Multi-Node

### 4. Scalable
