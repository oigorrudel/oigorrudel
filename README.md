```java
    public static void main(String[] args) {
        final var igor = Person.builder()
            .firstName("Igor")
            .lastName("Rudel")
            .age(Period.between(LocalDate.of(1993, Month.APRIL, 1), LocalDate.now()).getYears())
            .hobbies(List.of(
                "Assistir jogos de CS:GO",
                "Séries",
                "Filmes"
            ))
            .favoriteSeries(List.of("Friends", "GoT", "Snowpiercer", "Bridgerton"))
            .readBooks(
                List.of(
                    "Harry Potter", "Crônicas de Gelo e Fogo",
                    "Ponto de Impacto", "Fortaleza Digital", "Símbolo Perdido",
                    "Crônicas de Nárnia", "O Hobbit"
                )
            )
            .build();

        System.out.println(igor);
    }

    @Getter
    @Builder
    @ToString
    public static class Person {
        private String firstName;
        private String lastName;
        private Integer age;
        private List<String> hobbies;
        private List<String> favoriteSeries;
        private List<String> readBooks;
    }

```
