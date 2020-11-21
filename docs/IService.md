## Описание интерфейса IService

Интерфейс предназначен для работы с методами класса [Service](Service)

###Реализация интерфейса

- +Add (Service: [Service](Service)): String — функция, добавляющая услугу в базу данных. Параметр «[Service](Service)» — услуга, которую необходимо добавить в БД;

- +Save (Service: [Service](Service)): String — функция, сохраняющая данные о услуге. Параметр «[Service](Service)» — услуга, которую необходимо сохранить в БД;

- +Edit (Service: [Service](Service)): String — функция, редактирующая данные о услуге. Параметр «[Service](Service)» — услуга, которую необходимо редактировать в БД;

- +Delete (ID): Int — функция удаляет услугу из БД;

- +FindAll(sortingA:string,sortingB:string, filterA:[Service](Service),filterB:[Service](Service), count:int, page:int):List< [Service](Service) > -  функция, возвращающая список услуг, удовлетворяющих заданным параметрам.
Параметры: 

+ sorting: string — отвечает, по какому полю будет сортироваться список;
+ sortingА: string — отвечает, по возрастанию или убыванию будут сортироваться элементы;
+ filterA: [Service](Service) — отвечает за фильтрацию;
+ filterB: [Service](Service) —необходим для количественных атрибутов;
+ count: int — отвечает, сколько элементов необходимо показать;

- +GetClient(IDService:Int):List< [Client](Client.md) > - функция возвращает список клиентов, у которых была данная услуга
