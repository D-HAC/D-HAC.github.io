# Find Person

This is a classic OO practice problem that we're going to do a twist on. Create a simple object (or struct, if you really want) that has properties:
age, name, birthMonth, SSN, ZIPCode. These can be public and primitive type, encapsulation and type safety aren't the point here. The simplest form of the java class is below
```
public class Person
{
	public int age;
	public int birthMonth;
	public String name;
	public String ssn;
	public int zipCode;
}
```
### Next
 write a group of functions or methods to do the following:
* Given an age and a list of people, return a list of people who are at least the given age
* Given an SSN and a list of people, return the person's name
* Given a list of people and a month, get a list of people with birthdays that month
* Given a month and a list of people, get the zip codes of all people with birthdays in that month

### Finally
Refactor the functions you wrote to reduce the amount of repeated code.
