## <u>SYSTEM-GC</u>

## About:

This is a java agent that causes a System.gc() to occur in a background thread while your java application is running.

## Purpose:

Save memory for those who have memory restrictions when running java applications.

## Recommended:

Together with this, use a reasonable -Xmx value (maximum heap size) and optional combination of:

-  -XX:MinHeapFreeRatio=1
-  -XX:MaxHeapFreeRatio=2 

 to improve performance and avoid huge heaps even once GC occurs.