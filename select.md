select * 
from table1_name
# first specify the columbs you want it to select useing there headers in this case * witch means all coulumbs
# then specify the table you want it to select these coulumbs from





#if you tell it to look in multiple tables and the columbe you want has the same name in 2 or more difrent tables you will need to specify the 
#table it should select from ie

select table1_name.T1coulumb1_name , table2_name.T2coulumb1_name
from table1_name , table2_name


#like
#if you want to find rows containing a certin word or number you can use like

SELECT * FROM table1_name
WHERE T1columb1_name LIKE '4%';  

#or

SELECT * FROM table1_name
WHERE T1columb1_name LIKE '%0';

#or you can even do both

SELECT * FROM table1_name
WHERE T1columb1_name LIKE '4%0';

#joining
#in some cases you may want to join two seprat querys rather than just search 2 tabels as one

SELECT table1_name.T1columb1_name, tables2_name.T2columb1_name, tables2_name.T2columb2_name
FROM table1_name
INNER JOIN tables2_name
ON table1_name.T1columb1_name = tables2_name.T2columb3_name;  #assuming table1's first columb and table2's second are the same

