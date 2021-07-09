# Demonstrating faulty Kotlin codegen on protobuf v3.17.3

1. Clone this repo
2. `./gradlew clean compileKotlin`
3. Should see the following output:
```
> Task :compileKotlin FAILED
e: .../gradle-kotlin-proto-test/build/generated/source/proto/main/kotlin/org/example/addressbook/AddressBookKt.kt: (13, 5): JvmField has no effect on a private property
e: .../gradle-kotlin-proto-test/build/generated/source/proto/main/kotlin/org/example/addressbook/PersonKt.kt: (13, 5): JvmField has no effect on a private property
e: .../gradle-kotlin-proto-test/build/generated/source/proto/main/kotlin/org/example/addressbook/PersonKt.kt: (154, 7): JvmField has no effect on a private property
```