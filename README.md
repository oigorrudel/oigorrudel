```java
@Data
public static class Person {
  private String firstName;
  private String lastName;
  private Integer age;
  private List<String> hobbies;
  private List<String> favoriteSeries;
  private List<String> readBooks;
  
  public Person(final String firstName, final String lastName) {
    this.firstName = firstName;
    this.lastName = lastName;
  }
}

public static void main(String[] args) {
  
  final var igor = new Person("Igor", "Rudel");
  igor.setAge(29);
  igor.setHobbies(
    List.of(
      "Ver jogos de CS:GO", 
      "Ver jogos da Premier League", 
      "Séries", 
      "Filmes"
    )
  );
  
  igor.setFavoriteSeries(
    List.of("Friends", "GoT", "Snowpiercer")
  );
  
  igor.setReadBooks(
    List.of(
      "Harry Potter", "Crônicas de Gelo e Fogo", 
      "Ponto de Impacto", "Fortaleza Digital", "Símbolo Perdido",
      "Crônicas de Nárnia", "O Hobbit"
    )
  );
}

```
