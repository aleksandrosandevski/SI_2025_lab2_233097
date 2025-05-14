# SI_2025_lab2_233097

Александро Сандевски 233097

3. Според предикатните јазли коишто се обоени во сино, може да се заклули дека има 8 предикатни јазли и 8+1 = 9. Затоа цикломатската сложеност е 9.

4.  Треба да има 6 тест случаеви за да се покрие Every statement критериумот.
   Првиот тест случај е           allItems = null          cardNumber = "1234567812345678"
                              овој случај го покрива if (allItems == null)

    Вториот тест случај е      allItems = [Item(name = null, quantity = 1, price = 100, discount = 0.0)]
                                cardNumber = "1234567812345678"
                              овој случај покрива за невалидно име како null или празен стринг

    Третиот тест случај  е    allItems = [Item(name = "ItemA", quantity = 1, price = 100, discount = 0.0)]
                              cardNumber = "1234567812345678"
                              валиден предмет, нема попуст, валиден број на картица, ема одземање на 30 поени

    Четвртиот тест случај е     allItems = [Item(name = "ItemB", quantity = 2, price = 200, discount = 0.25)]
                                  cardNumber = "1234567812345678"
                                  калкулација на попуст и и валидна картичка

    Петтиот тест случај е         allItems = [Item(name = "ItemC", quantity = 1, price = 100, discount = 0.0)]
                                cardNumber = "1234" (invalid length)
                                невалидна должина на картицжчата односно под 16 броеви

    Шестиот тест случај        allItems = [Item(name = "ItemD", quantity = 1, price = 100, discount = 0.0)]
                                cardNumber = "12345678abcd5678" (contains letters)
                                проверува за невалиден знак преку циклус,
