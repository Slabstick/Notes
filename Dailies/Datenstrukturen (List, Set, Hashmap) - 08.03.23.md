#List #Set #Map #Hashmap #Hashset #Queue #Dequeue #Stack

## 2 Dimensionale Arrays

``` java
char[][] array = new char[][]{
	new char[]{'a', 'b', 'c', 'd'},
	new char[]{'e', 'f', 'g', 'h'},
	new char[]{'i', 'j', 'k', 'l'}	
};
```

## Stack

- Dynamisch
- FILO First In Last Out
- Wie ein Stapel

## Queue

- Dynamisch
- FIFO First In First Out
- Wie eine Schlange
- Deque: Double ended queue
- `Queue<String> queue = new LinkedList<>();`

``` java
queue.add("Hello");
queue.remove("Hello"); // gibt Fehler aus, wenn queue leer ist
queue.poll("Hello"); // gibt null aus, wenn queue leer ist

dequeue.addFirst("HelloFirst");
dequeue.addLast("HelloLast");
```

## List

- Dynamisch
- Weder FILO oder FIFO - Zugriff auf jedes Element möglich
- Bevorzugte Implementierung: ArrayList

## Set

- Dynamisch
- Keine Duplikate
- Keine Reihenfolge
- Bevorzugte Implementierung: HashSet
- hat Iterator

``` Java
Set<String> set = new HashSet<>();

set.add("test");
set.add("test");
System.out.println(set.size()); //1

for (String element : set) {
	System.out.println(element);
}
```

## Map

- Dynamische Datenstruktur
- Speichert "Key-Value"-Paare
- Bevorzugte Implementierung: HashMap

``` java
Map<String, Integer> map = new HashMap<>();
map.put("A", 1);
map.put("B", 2);
map.put("C", 3);
map.put("D", 4);

System.out.println(map.get("B")); // 2
System.out.println(map.get("A")); // 4
System.out.println(map.get("test")); // null

Set<String> keySet = map.keySet();
Set<Map.Entry<String, Integer>> entrySet = map.entrySet();
Collection<Integer> values = map.values();
```

