# Software Requirements Specification
# For  `<project name>`
Version `<version>`
Prepared by
`<author>`
`<organization>`
`<date created>`

# Revision History
| Name  | Date    | Reason For Changes  | Version   |
| ----  | ------- | ------------------- | --------- |
|  Sameer Pradhan &nbsp; | May 2, 2018 &nbsp;| Initial version derived from the  &nbsp; | &nbsp; 0.1 |
| |                        | IEEE Std. 830 (1998) &nbsp;              |  |

<div class="padding"></div>

# 1. Introduction

The introduction of the SRS should provide an overview of the entier SRS.

## 1.1 Purpose

- Delineat the purpose of the SRS
- Specify the intended audience of the SRS.

## 1.2 Scope

- Identify the software being produced by name (Host DBMS, Report Generator, etc.);
- Explain what the software being specified will, and necessarily will _not_ do;
- Describe the application of the software being specified including relevant benefits, objectives, and goals;
- Be consistent in similar statements in higher-level specifications (e.g., the system requirements specification), if they exist.

## 1.3 Definitions, acronyms and abbreviations

This subsection should provide the definitions of all terms, acronyms, and abbreviations required to properly interpret the SRS. This information may be provided by reference to one or more appendixes in the SRS or by reference to other documents.

## 1.4 References

This subsection should

- Provide a complete list of all documents referenced elsewhere in the SRS;
- Identify each document by title, report number (if applicable), date, and    publishing organization;
- Specify the sources from which the references can be obtained.

This information may be provided by reference to an appendix or to another document.


## 1.5 OVerview

This subsection should

- Describe what the rest of the SRS contains;
- Explain how the SRS is organized.

# 2 Overall Description

This section of the SRS should describe the general factors that affect the product and its requirements. This section does not state specific requirements. Instead, it provides a background for those requirements, which are defined in detail in Section 3 of the SRS, and makes them easier to understand.

## 2.1 Product Perspective

This subsection of the SRS should put the product into perspective with other related products. If the product is independent and totally self-contained, it should be so stated here. If the SRS defines a product that is a component of a larger system, as frequently occurs, then this subsection should relate the requirements of that larger system to functionality of the software and should identify interfaces between that system and the software.
A block diagram showing the major components of the larger system, interconnections, and external interfaces can be helpful.

This subsection should also describe how the software operates inside various constraints. For example, these constraints could include the following subsections:

- System interfaces;
- User interfaces;
- Hardware interfaces;
- Software interfaces;
- Communications interfaces;
- Memory;
- Operations;
- Site adaptation requirements.


### 2.1.1 System interfaces

This should list each system interface and identify the functionality of the software to accomplish the system requirement and the interface description to match the system.

### 2.1.2 User interfaces

This should specify the following:

- _The logical characteristics of each interface between the software product and its users._

    This includes those configuration characteristics (e.g., required screen formats, page or window layouts, content of any reports or menus, or availability of programmable function keys) necessary to accomplish the software requirements.
- _All the aspects of optimizing the interface with the person who must use the system._

    This may simply comprise a list of do's and don'ts on how the system will appear to the user. One example may be a requirement for the option of long or short error messages. Like all others, these requirements should be verifiable, e.g., "a clerk typist grade 4 can do function X in Z min after 1 h of training" rather than "a typist can do function X." (This may also be specified in the Software System Attributes under a section titled Ease of Use.)

### 2.1.3 Hardware interfaces

This should specify the logical characteristics of each interface between the software product and the hardware components of the system. This includes configuration characteristics (number of ports, instruction sets, etc.). It also covers such matters as what devices are to be supported, how they are to be supported, and protocols. For example, terminal support may specify full-screen support as opposed to line-by-line support.

### 2.1.4 Software interfaces

This should specify the use of other required software products (e.g., a data management system, an operating system, or a mathematical package), and interfaces with other application systems (e.g., the linkage between an accounts receivable system and a general ledger system). For each required software product, the following should be provided:

- Name;
- Mnemonic;
- Specification number;
- Version number;
- Source.

For each interface, the following should be provided:

- Discussion of the purpose of the interfacing software as related to this software product.
- Definition of the interface in terms of message content and format. It is not necessary to detail any well-documented interface, but a reference to the document defining the interface is required.

### 2.1.5 Communications interfaces

This should specify the various interfaces to communications such as local network protocols, etc.

### 2.1.6 Memory constraints

This should specify any applicable characteristics and limits on primary and secondary memory.

### 2.1.7 Operations

This should specify the normal and special operations required by the user such as

- The various modes of operations in the user organization (e.g., user-initiated  operations);
- Periods of interactive operations and periods of unattended operations;
- Data processing support functions;
- Backup and recovery operations.

NOTE: This is sometimes specified as part of the User Interfaces section.

### 2.1.8 Site adaptation requirements

This should

- Define the requirements for any data or initialization sequences that are specific to a given site, mission, or operational mode (e.g., grid values, safety limits, etc.);

- Specify the site or mission-related features that should be modified to adapt the software to a particular installation.


## 2.2 Product functions

This subsection of the SRS should provide a summary of the major functions that the software will perform. For example, an SRS for an accounting program may use this part to address customer account maintenance, customer statement, and invoice preparation without mentioning the vast amount of detail that each of those functions requires.

Sometimes the function summary that is necessary for this part can be taken directly from the section of the higher-level specification (if one exists) that allocates particular functions to the software product. Note that for the sake of clarity

- The functions should be organized in a way that makes the list of functions understandable to the customer or to anyone else reading the document for the first time.
- Textual or graphical methods can be used to show the different functions and their relationships. Such a diagram is not intended to show a design of a product, but simply shows the logical relationships among variables.


## 2.3 User characteristics

This subsection of the SRS should describe those general characteristics of the intended users of the product including educational level, experience, and technical expertise. It should not be used to state specific requirements, but rather should provide the reasons why certain specific requirements are later specified in Section 3 of the SRS.

## 2.4 Constraints

This subsection of the SRS should provide a general description of any other items that will limit the developerÕs options. These include

- Regulatory policies;
- Hardware limitations (e.g., signal timing requirements);
- Interfaces to other applications;
- Parallel operation;
- Audit functions;
- Control functions;
- Higher-order language requirements;
- Signal handshake protocols (e.g., XON-XOFF, ACK-NACK);
- Reliability requirements;
- Criticality of the application;
- Safety and security considerations.

## 2.5 Assumptions and dependencies

This subsection of the SRS should list each of the factors that affect the requirements stated in the SRS. These factors are not design constraints on the software but are, rather, any changes to them that can affect the requirements in the SRS. For example, an assumption may be that a specific operating system will be available on the hardware designated for the software product. If, in fact, the operating system is not available, the SRS would then have to change accordingly.


## 2.6 Apportioning of requirements

This subsection of the SRS should identify requirements that may be delayed until future versions of the system.

# 3 Specific requirements

This section of the SRS should contain all of the software requirements to a level of detail sufficient to enable designers to design a system to satisfy those requirements, and testers to test that the system satisfies those requirements. Throughout this section, every stated requirement should be externally perceivable by users, operators, or other external systems. These requirements should include at a minimum a description of every input (stimulus) into the system, every output (response) from the system, and all functions performed by the system in response to an input or in support of an output. As _this is often the largest and most important part of the SRS_, the following principles apply:

- Specific requirements should be stated in conformance with all the characteristics described in 4.3.
- Specific requirements should be cross-referenced to earlier documents that relate.
- All requirements should be uniquely identifiable.
- Careful attention should be given to organizing the requirements to maximize readability.

Before examining specific ways of organizing the requirements it is helpful to understand the various items that comprise requirements as described in 3.1 through 3.7.


## 3.1 External interfaces

This should be a detailed description of all inputs into and outputs from the software system. It should complement the interface descriptions in 5.2 and should not repeat information there.

It should include both content and format as follows:

- Name of item;
- Description of purpose;
- Source of input or destination of output;
- Valid range, accuracy, and/or tolerance;
- Units of measure;
- Timing;
- Relationships to other inputs/outputs;
- Screen formats/organization;
- Window formats/organization;
- Data formats;
- Command formats;
- End messages.


## 3.2 Functions

Functional requirements should define the fundamental actions that must take place in the software in accepting and processing the inputs and in processing and generating the outputs. These are generally listed as "shall" statements starting with "The system shall"

These include

- Validity checks on the inputs
- Exact sequence of operations
- Responses to abnormal situations, including
  - Overflow
  - Communication facilities
  - Error handling and recovery
- Effect of parameters
- Relationship of outputs to inputs, including
  - Input/output sequences
  - Formulas for input to output conversion

It may be appropriate to partition the functional requirements into subfunctions or subprocesses. This does not imply that the software design will also be partitioned that way.

## 3.3 Performance requirements

This subsection should specify both the static and the dynamic numerical requirements placed on the software or on human interaction with the software as a whole. Static numerical requirements may include the following:

- The number of terminals to be supported;
- The number of simultaneous users to be supported;
- Amount and type of information to be handled.

Static numerical requirements are sometimes identified under a separate section entitled Capacity.

Dynamic numerical requirements may include, for example, the numbers of transactions and tasks and the amount of data to be processed within certain time periods for both normal and peak workload conditions.

All of these requirements should be stated in measurable terms.

For example,

_95% of the transactions shall be processed in less than 1 s._

rather than,

_An operator shall not have to wait for the transaction to complete._

NOTE: Numerical limits applied to one specific function are normally specified as part of the processing subparagraph description of that function.


## 3.4 Logical database requirements

This should specify the logical requirements for any information that is to be placed into a database. This may include the following:

- Types of information used by various functions;
- Frequency of use;
- Accessing capabilities;
- Data entities and their relationships;
- Integrity constraints;
- Data retention requirements.


## 3.5 Design constraints

This should specify design constraints that can be imposed by other standards, hardware limitations, etc.


## 3.6 Software system attributes

There are a number of attributes of software that can serve as requirements. It is important that required attributes be specified so that their achievement can be objectively verified. Subclauses 3.6.1 through 3.6.5 provide a partial list of examples.

### 3.6.1 Reliability

This should specify the factors required to establish the required reliability of the software system at time of delivery.

### 3.6.2 Availability

This should specify the factors required to guarantee a defined availability level for the entire system such as checkpoint, recovery, and restart.

### 3.6.3 Security

This should specify the factors that protect the software from accidental or malicious access, use, modification, destruction, or disclosure. Specific requirements in this area could include the need to

- Utilize certain cryptographical techniques;
- Keep specific log or history data sets;
- Assign certain functions to different modules;
- Restrict communications between some areas of the program;
- Check data integrity for critical variables.

### 3.6.4 Maintainability

This should specify attributes of software that relate to the ease of maintenance of the software itself. There may be some requirement for certain modularity, interfaces, complexity, etc. Requirements should not be placed here just because they are thought to be good design practices.

### 3.6.5 Portability

This should specify attributes of software that relate to the ease of porting the software to other host machines and/or operating systems. This may include the following:

- Percentage of components with host-dependent code;
- Percentage of code that is host dependent;
- Use of a proven portable language;
- Use of a particular compiler or language subset;
- Use of a particular operating system.

## 3.7 Organizing the specific requirements

For anything but trivial systems the detailed requirements tend to be extensive. For this reason, it is recommended that careful consideration be given to organizing these in a manner optimal for understanding. There is no one optimal organization for all systems. Different classes of systems lend themselves to different organizations of requirements in Section 3 of the SRS. Some of these organizations are described in 3.7.1 through 3.7.7.


### 3.7.1 System mode

Some systems behave quite differently depending on the mode of operation. For example, a control system may have different sets of functions depending on its mode: training, normal, or emergency. When organizing this section by mode, the outline in A.1 or A.2 should be used. The choice depends on whether interfaces and performance are dependent on mode.


### 3.7.2 User class

Some systems provide different sets of functions to different classes of users. For example, an elevator control system presents different capabilities to passengers, maintenance workers, and fire fighters. When organizing this section by user class, the outline in A.3 should be used.

### 3.7.3 Objects

Objects are real-world entities that have a counterpart within the system. For example, in a patient monitoring system, objects include patients, sensors, nurses, rooms, physicians, medicines, etc. Associated with each object is a set of attributes (of that object) and functions (performed by that object). These functions are also called services, methods, or processes. When organizing this section by object, the outline in A.4 should be used. Note that sets of objects may share attributes and services. These are grouped together as classes.

### 3.7.4 Feature

A feature is an externally desired service by the system that may require a sequence of inputs to effect the desired result. For example, in a telephone system, features include local call, call forwarding, and conference call. Each feature is generally described in a sequence of stimulus-response pairs. When organizing this section by feature, the outline in A.5 should be used.

### 3.7.5 Stimulus

Some systems can be best organized by describing their functions in terms of stimuli. For example, the functions of an automatic aircraft landing system may be organized into sections for loss of power, wind shear, sudden change in roll, vertical velocity excessive, etc. When organizing this section by stimulus, the outline in A.6 should be used.

### 3.7.6 Response

Some systems can be best organized by describing all the functions in support of the generation of a response. For example, the functions of a personnel system may be organized into sections corresponding to all functions associated with generating paychecks, all functions associated with generating a current list of employees, etc. The outline in A.6 (with all occurrences of stimulus replaced with response) should be used.

### 3.7.7 Functional hierarchy

When none of the above organizational schemes prove helpful, the overall functionality can be organized into a hierarchy of functions organized by either common inputs, common outputs, or common internal data access. Data flow diagrams and data dictionaries can be used to show the relationships between and among the functions and data. When organizing this section by functional hierarchy, the outline in A.7 should be used.

## 3.8 Additional comments

Whenever a new SRS is contemplated, more than one of the organizational techniques given in 3.7.7 may be appropriate. In such cases, organize the specific requirements for multiple hierarchies tailored to the specific needs of the system under specification. For example, see A.8 for an organization combining user class and feature. Any additional requirements may be put in a separate section at the end of the SRS.

There are many notations, methods, and automated support tools available to aid in the documentation of requirements. For the most part, their usefulness is a function of organization. For example, when organizing by mode, finite state machines or state charts may prove helpful; when organizing by object, object-oriented analysis may prove helpful; when organizing by feature, stimulus-response sequences may prove helpful; and when organizing by functional hierarchy, data flow diagrams and data dictionaries may prove helpful.

In any of the outlines given in A.1 through A.8, those sections called "Functional Requirement i" may be described in native language (e.g., English), in pseudocode, in a system definition language, or in four subsections titled: Introduction, Inputs, Processing, and Outputs.


# 4 Supporting information

The supporting information makes the SRS easier to use. It includes the following:

- Table of contents;
- Index;
- Appendixes.

## 4.1 Table of contents and index

The table of contents and index are quite important and should follow general compositional practices.

## 4.2 Appendixes

The appendixes are not always considered part of the actual SRS and are not always necessary. They may include

- Sample input/output formats, descriptions of cost analysis studies, or results of user surveys;
- Supporting or background information that can help the readers of the SRS;
- A description of the problems to be solved by the software;
- Special packaging instructions for the code and the media to meet security, export, initial loading, or other requirements.

When appendixes are included, the SRS should explicitly state whether or not the appendixes are to be considered part of the requirements.
