# Proof of concept to read attributes to a string

## Disclaimer

This is a personal guide not a peer reviewed journal or a sponsored publication. We make
no representations as to accuracy, completeness, correctness, suitability, or validity of any
information and will not be liable for any errors, omissions, or delays in this information or any
losses injuries, or damages arising from its display or use. All information is provided on an as
is basis. It is the reader’s responsibility to verify their own facts.

The views and opinions expressed in this guide are those of the authors and do not
necessarily reflect the official policy or position of any other agency, organization, employer or
company. Assumptions made in the analysis are not reflective of the position of any entity
other than the author(s) and, since we are critically thinking human beings, these views are
always subject to change, revision, and rethinking at any time. Please do not hold us to them
in perpetuity.

## Overview

This is a proof of concept that you can read the attribute value to a string of any size.

## Screenshot

![image](./docs/images/Screenshot.png)

![image](./docs/images/ScreenshotOffline.png)

## Code Snippets

The following section of code shows the E_Colors Enum.

```
PROGRAM MAIN
VAR
	{attribute 'foobar' := 'helloworld'}
	myBool : BOOL;

	found : BOOL;
	attributeValue : STRING(80);
END_VAR

// -----------------------------------

found := TryReadAttributeValue('Main.myBool','foobar', adr(attributeValue), sizeof(attributeValue));

```

## Versions

- TcXaeShell 3.1.4024.53

## Need more help?

Please visit http://beckhoff.com/ for further guides
