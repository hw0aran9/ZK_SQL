Можно делать [[SELECT]] для большого числа фейковых значений без помощи union, а сделав конструкцию select unnest(array[]) из ниоткуда в postgresql.

Вместо 

select 1 as id, 0 as fake_value union all
select 2 as id, 2 as fake_value

можно сделать так: 

select 
unnest(array[1,2]) id,
unnest(array[0,2]) fake_value
