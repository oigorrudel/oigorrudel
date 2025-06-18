```java
    public static void main(String[] args) {
        final var igor = Person.builder()
            .firstName("Igor")
            .lastName("Rudel")
            .age(Period.between(LocalDate.of(1993, Month.APRIL, 1), LocalDate.now()).getYears())
            .build();

        System.out.println(igor);
    }

    @Data
    @Builder
    public static class Person {
        private String firstName;
        private String lastName;
        private Integer age;
    }

```
