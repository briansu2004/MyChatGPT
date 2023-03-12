# Interview with ChatGPT - Java Core

## [Java] @NamedQuery

@NamedQuery is a JPA (Java Persistence API) annotation that is used to define a pre-defined query with a specific name. This named query can be then referenced in code to execute the query.

For example, consider a case where we have a JPA entity named "User" and we want to retrieve all the users from the database whose age is greater than a certain value. We can define a named query using the @NamedQuery annotation as follows:

```java
@Entity
@NamedQuery(name = "User.findByAgeGreaterThan", query = "SELECT u FROM User u WHERE u.age > :age")
public class User {
    // Class definition
}
```

In this example, we have defined a named query with the name "User.findByAgeGreaterThan" and the actual query to be executed is "SELECT u FROM User u WHERE u.age > :age". We can now use this named query in our code to retrieve the required data as follows:

```java
TypedQuery<User> query = entityManager.createNamedQuery("User.findByAgeGreaterThan", User.class);
query.setParameter("age", 25);
List<User> users = query.getResultList();
```

In this code snippet, we have created a TypedQuery object using the named query "User.findByAgeGreaterThan" and then set the value of the parameter "age" to 25. Finally, we have executed the query and obtained the result list.

## [Java] 0

## [Java] 1

## [Java] 2

## [Java] 3
