# Goup Java Collection Doc
# Interfaces
### The Collection Interface
### The Set Interface
### The List Interface
<p>
List是有序的Collection

<b><h2>Iterator</h2></br>
List類專用的 ListIterator。</br>
一般的Iterator只能remove元素，ListIterator可以add()、set()、remove()
ListIteratoru也可以在游標<br>向後或向前previous()

<b><h2>Range-View Operation</h2></br>

<p>
    
    //subList(int fromIndex, int toIndex)

    //for (int i = fromIndex; i < toIndex; i++) {
    ...
    }
<p>
fromIndex - 截取元素的起始位置，包含该索引位置元素</br>
toIndex - 截取元素的结束位置，不包含该索引位置元素</br>

swap— 交換 a 中指定位置的元素List。</br>
copy— 將源複製List到目標List。</br>
sort—List使用合併排序算法對 a 進行排序，</br>
</P>
### The Queue Interface
### The Deque Interface
### The Map Interface
### Object Ordering
### The SortedSet Interface
### The SortedMap Interface

# Aggregate Operations
<p> 
聚合操作(aggregate operations)的預備知識：lambda expressions , method references
下面一個簡短的例子說明聚合操作(aggregate operations)跟for-each語法上的差異：
</p>

    // for-each
    for (Person p : roster) {
        System.out.println(p.getName());
    }
    // aggregate op
    roster
    .stream()
    .forEach(e -> System.out.println(e.getName());
<p>
Pipelines and Streams<br/>
* pipeline 指的是一連串的聚合操作，通常會有下面元件：</p>
 
 - 一個來源:collection,array or I/O channel(java.nio.file)
 - 0-* 中間操作(intermediate op):像是filter 會產生新的stream,stream並非像collection一樣是個資料結構，而是元素序列。
 - 一個終結操作(terminal op):像是foreach產生非stream的結果(基本型態數值、集合)


<p>
Differences Between Aggregate Operations and Iterators<br/>

</p>

### Reduction
### Parallelism
  
# Implementations
### Set Implementations
### List Implementations
### Map Implementations
### Queue Implementations
### Deque Implementations
# Deque
<P>Deque是一個雙端隊列 Quene和Deque 實現了 stack和Quene<br/>
Queue佇列有點像先進先出<br/>
Dequey可以對尾端加入物件或取出物件<br/>


### Wrapper Implementations
### Convenience Implementations