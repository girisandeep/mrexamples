# Map Reduce Example
~~~~
These are the examples of Map-Reduce
git clone https://github.com/girisandeep/mrexamples.git
cd mrexamples/
ant jar
hadoop jar build/jar/MR.jar my.StubDriver /data/mr/wordcount/input javamrout
~~~~

# Hive Example

## 1. Compile and build the jar
`ant hiveudfjar`

## 2. Start Hive
`hive`

## 3. On the hive prompt execute
~~~~
add jar build/jar/kbdexamples.jar
create temporary function my_lower as 'hiveudf.Lower';
select my_lower('sandeeGGGGGHHHkkp');
~~~~
