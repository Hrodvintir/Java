# A Computed, Read-Only Property

In the prior video lesson, we created the Car class, and gave it a single read-write property for speed, based on the presence of a speed attribute.

In this reading, we take a look at what it takes to create a simple read-only property for date that we do not even have as an attribute.

In order to have a readable property, we need a getter method.  The getter, int getAge(), does not expose how we are finding and returning the value.  Our particular implementation uses the new Java 8 classes, but we could have done it some other way.  We added a manufactured attribute to contain the date on which the car were made, and implemented the age property using the new Java 8 Time package, but we could have done it differently, so long as we yielded the same result to the caller.
```java
	private LocalDate manufactured;
	
	public int getAge() {
		return Period.between(manufactured, LocalDate.now()).getYears();
	}
	
```
Feel free to look ahead at the Java 8 Time package to see what LocalDate and Period provide.

The lecture discussed attributes and methods.  A JavaBean property is, in a sense, neither.  It is an abstract notion derived from the presence of certain methods.  It feels like data, but it is not an attribute.  It is managed by code that has required method signatures, but it feels more like data.  Either way, JavaBean properties are essential to many of the frameworks we want to use, including Spring.
