****CREATE - [[DDL]]-операция для создания объектов в БД

CREATE [[TABLE]]
CREATE [[VIEW]]

Например: 
CREATE OR [[REPLACE]] [[TEMP]] | [[TEMPORARY]] [[RECURSIVE]] [[VIEW]] 'NAME' [ ( _`имя_столбца`_ [, ...] ) ]
    [ WITH ( _`имя_параметра_представления`_ [= _`значение_параметра_представления`_] [, ... ] ) ]
    AS _`запрос`_
    [ [[WITH]] [ [[CASCADED]] | [[LOCAL]] ] CHECK OPTION ]

