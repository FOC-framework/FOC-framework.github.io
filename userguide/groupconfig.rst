Rights Group
============

FocObject
---------
The foc entity superclass is FocObject. All your foc entities are a subclass of FocObject. When created using annotations it will extend PojoFocObject which extends FocWorkflowObject which extends FocObject.

FocProperty
-----------
Every property in an Entity like “First name” “Last Name” “Age” is a sub class of FocProperty. So every FocObject contains a list of FocProperty. Obviously each property type is a subclass of FocProperty. FString, FInt, FDouble, FBoolean, FDate, FTime, …

FocDesc
-------
FocDesc is the description of an Entity (FocObject). All instances of the same type of entity share the same single instance of FocDesc describing the underlying table strucure or ore generally the data strucure.

So if you have an entity Empoyee aand you have 100 employee rows in your DB, you will have 100 instances of Employee and one single instance of FocDesc. You don’t have to create a super class for FocDesc but should you decide to do so you should call it EmployeeDesc.