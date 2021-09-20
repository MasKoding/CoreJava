##  Java OOP (Object Oriented Programming)

#Introduction OOP
Pemrograman Berorientasi Object atau disingkat OOP merupakan paradigma pemrograman berdasarkan konsep objek yang berisi attribut atau field serta method atau function.

Dalam paradigma ini semua data dan method dibungkus dalam kelas kelas atau objek objek.

## Definisi
1. Class merupakan blueprint atau prototype dari objek yang akan kita buat. Di dalam class kiat mendeklarasikan properti dan method yang akan digunakan dalam objek kita
2. Object merupakan instance dari class yang memiliki state dan behavior

## Diagram Class
```plantuml
@startuml

    class User {
        - name : String
        - age : Integer
        - address : String

        .. Simple Setter ..
        setName(name : String) :void
        setAge(age : String) : void
        setAddress(address : String) : void
        .. Simple Getter ..
        getName() : String
        getAge() : String
        getAddress : String
    }

    note top of User
        Ini merupakan kelas user
    end note

    object user1
    user1 : name = "Dummy"
    user1 : age = 20
    user1 : address = "Jakarta"

    object user2
    user2 : name="Dummy2"
    user2 : age = 22
    user2 : address = "Bogor"


User --> user1 : Object
User --> user2 : Object
@enduml
```
