# Porting guide for {{NAME}}

This document provides a porting guide for {{MODULE_NAME}} version {{VERSION}}.

The {{NAME}} API is declared in the [{{FILE_NAME}} header file]({{LINK_TO_HEADER}}).

[Optional] The generated documentation is located at {{DOCS.MBED_LINK}}.

## Requirements
- list of requirements for the implementation to be ported - headers to be included, use of any other files outside of this porting, etc

Some more info about the module comes here.

## API

A few words about what the API does and doesn't offer. Especially if functionality I might expect is actually in a different API.

Please implement the functions listed below.

### {{FUNCTION_NAME}}

```
/** This is a copy from the header file where the function is documented
 *
 */
void function_declaration(void);
```

More detailed information here. 

#### [Optional] Implementation example 

The ideal generic implementation can be added, what is expected from the implementation.

```
//
void function_declaration(void)
{
    // enable clocks
    enable_clock();
    // toggle pin
    toggle_pin();
}
```

## {{OPTIONAL_SECTIONS}} (Limitations, known problems, ..)

[Optional] To be created only when relevant.

## Example

[Optional] This section should show how to implement an interface - a simple “bare bones” 
