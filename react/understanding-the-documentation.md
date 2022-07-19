# Understanding the Documentation

### Code Blocks

The documentation utilises a communication, metalanguage-type, method to define the structure of elements, components, and groups.&#x20;

_Elements_, _first-level components_ (i.e. not subelements or subcomponents), and _first-level groups_, indicate its respective syntax, disregarding props (including required ones), and describes its children or contents:

* `/* Content */` is used to indicate where text should be u — whether an element, component, or group — is to be implemented at that point in the code for a certain amount of times (including none at all, which may be defined in the sed (i.e. no child elements or components)
* `/* Children */` is used to indicate where child(ren) should be implemented into the code. The requirements and restrictions on what elements and components to use are defined under the heading: _Child Restrictions_.
* `/* { <Child> } */` is used to indicate a specific `Child`_Child Restrictions_).&#x20;
* `/* [ <Child> ] */` is used to indicate a specific `Child` is optional at that point in the code.
* `<Child>` is used to indicate that a specific `Child` is required at that point in the code.&#x20;
