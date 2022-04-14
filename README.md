```java
public static class Person {
  private String firstName;
  private String lastName;
  private Integer age;
  
  public Person(final String firstName, final String lastName) {
    this.firstName = firstName;
    this.lastName = lastName;
  }
}

public static void main(String[] args) {
  
  final var igor = new Person("Igor", "Rudel");
  igor.setAge(29);
}

```
