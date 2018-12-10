# ParamProject
Defines a JSON schema to be used by computational modeling projects


Why have an inputs schema?
----------------------------------

- Provides documentation for the user about how they can configure simulations.

- Provides information that the project can use for baseline configurations and to validate user inputs.

- If many projects use the same schema, then they can share inputs processing and validation code and will be more interoperable*

    \* When projects use similar inputs schemas and a similar inputs validation flow, developers/modelers can more intuitively link together several projects.

What are the essential elements of the schema?
----------------------------------------------------

Essentially, a value is needed for each parameter when a model is run. This value can be specified by the user or by the project as a baseline parameter. If the user is going to specify a parameter, then they will need the following pieces of information:

- What's the name of this parameter?
- What does this parameter do?
- What type of value should this parameter have? Should it be an integer, float, boolean, and so on? How many dimensions does it have?
- What's its range? Does it have a minimum, maximum, or discrete set of values that must include it?
- What action should be taken if it is outside of the specified range? Should a warning be shown to the user? Should the program halt?
- What messages should be shown to the user if the value is not specified correctly?

Many projects will need more information than these basic elements, and thus, there should be a way to specify those elements, too.

The Schema
----------------------

coming soon....


Implementations
------------------------

- **Python**

  - [ParamTools](https://github.com/hdoupe/ParamTools) - Python implementation of this schema
