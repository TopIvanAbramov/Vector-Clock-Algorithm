# Vector Clock Algorithm

**A vector clock** is a data structure used for determining the partial ordering of events in a distributed system and detecting causality violations

There is one script: main.py

There can be several types of events:
+ Send message
+ Receive message
+ Event (just a random one)

You should define each event of each process in process_{count} function

For example:

```python
def process_one(pipe12):
    pid = 0
    counter = [0, 0, 0]
    
    counter = send_message(pipe12, pid, counter)
    counter = event(pid, counter)
```

To run it simply type in terminal:

```
python3 main.py
```


Here is a good explanation of this algorithm: [link](https://towardsdatascience.com/understanding-lamport-timestamps-with-pythons-multiprocessing-library-12a6427881c6)
