# payment-service

> Interview discussion for architects

This is simple Payment service that makes use of an external(fake) Payment switch to perform the actual transaction.

It exposes a simple REST API endpoint

```
POST /payments
```
```json
{
  "paymentAmt":10000.0,
  "toAcc":"b123",
  "fromAcc":"a123",
  "note" : "Paying rent"
}
```
## Build

To build you can use either Gradle or Maven

For Gradle

```
./gradlew clean build
```

For Maven

```
./mvnw clean install
```

## Run the app

For Gradle

```
java -jar build/libs/payment-service-0.1.0.jar
```

For Maven

```
java -jar target/payment-service-0.1.0.jar
```

Application will be running at http://localhost:8080/