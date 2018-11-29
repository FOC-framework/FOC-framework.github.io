User management
===============

Creating users
--------------
The foc entity superclass is FocObject. All your foc entities are a subclass of FocObject. When created using annotations it will extend PojoFocObject which extends FocWorkflowObject which extends FocObject.

Changing site beonging
----------------------
Every property in an Entity like “First name” “Last Name” “Age” is a sub class of FocProperty. So every FocObject contains a list of FocProperty. Obviously each property type is a subclass of FocProperty. FString, FInt, FDouble, FBoolean, FDate, FTime, …
