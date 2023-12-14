# AutoCAD
In this repository you can find the automation tools for AutoCAD that are basically based on .NET.

For **first tool** <tool_name> you need to download all .dll files from this repository
Description: this tool can automatically create a batch AutoCAD drawings using the Data base tables and queries from Microsoft Access
How to launch:
1. Put ClassLibrary1.dll and AdvancedDataGridView.dll to the same folder
2. Launch AutoCAD and run the command "netload" in terminal bar below
3. Choose ClassLibrary1.dll and click OK
4. Now try to run command "loop". If AutoCAD can't find it then try again from step 2
   ...to be continued
   One problem I forgot about. The progrmamm is Russian at all and I don't even know why I'm writing in English. Here we switch to Russian (sry)
   
6. Логика работы макроса
   **Генерация следует логике**
    1. В шаблоне есть текст. блок с указанной ссылкой формата
        &1!Поле, 
        где
             1 - номер контура (один контур - один датчик)
             Поле - имя столбца Базы данных
    2. Замена ссылочных полей на чертеже на соответствующие данные из Базы данных
       
7. Краткое объяснение всех интерфейсных блоков макроса ниже.

   **Способ генерации**
    1. Один шаблон за цикл - генерация чертежей по выбранному шаблону 
    2. Несколько шаблонов за цикл - генерация чертежей по шаблонам, указанным в БД отдельным столбцом
    
    **Файл Access**
    1. Выбрать БД - указать путь к БД (access database)
    2. Загрузить БД - загрузка данных в таблицу макроса (серое поле)
    
    **Файл AutoCAD** 
    1. Загрузить шаблоны - выбор пути расположения шаблонов
    
    **Режимы генерации**
    1. Один файл .dwg - генерация чертежей в одном файле .dwg
    2. Множество файлов .dwg - генерация чертежей по принципу "Один лист - один файл .dwg"
    
    **При варианте "Множество файлов .dwg"**
    Путь генерации чертежей - выбор расположения для генерации чертежей
    Номер листа - начальное значение отсчета нумерации генерируемых листов
    
    

