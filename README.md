<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0C4A6E,50:00599C,100:659AD2&height=160&section=header&text=C%2B%2B%20Queue&fontSize=50&fontColor=ffffff&fontAlignY=40&desc=Array-based%20queue%20data%20structure&descSize=17&descAlignY=62&animation=fadeIn" width="100%" alt="C++ Queue — array-based queue data structure"/>

# Queue Data Structure in C++ — Array Implementation with Enqueue, Dequeue & Menu

<p>
  <img src="https://img.shields.io/badge/C%2B%2B-00599C?style=for-the-badge&logo=cplusplus&logoColor=white" alt="C++"/>
  <img src="https://img.shields.io/badge/Data%20Structures-FIFO%20Queue-6E40C9?style=for-the-badge" alt="Data structures: FIFO queue"/>
</p>

</div>

---

A software-engineering coursework exercise: a **FIFO queue** built on a fixed-size array (`MAX_SIZE = 10`) with a console menu to try every operation.

## ⚙️ Operations

| Function | What it does | Complexity |
|---|---|---|
| `init()` | Sets `front = 0`, `rear = -1` | O(1) |
| `enqueue(x)` | Adds `x` at the rear (menu checks `isFull()` first) | O(1) |
| `dequeue()` | Removes and returns the front element (menu checks `isEmpty()` first) | O(1) |
| `size()` | `rear - front + 1` | O(1) |
| `isEmpty()` / `isFull()` | Bounds checks | O(1) |
| `display()` | Prints elements front → rear | O(n) |

```mermaid
flowchart LR
    E["enqueue → rear"] --> Q["[ front · · · rear ]"] --> D["dequeue ← front"]
```

## ▶️ Run

```bash
g++ Untitled1.cpp -o queue
./queue
```

```text
1. Enqueue
2. Dequeue
3. Size
4. Display all element
5. Quit
```

## 📚 Concepts

- **FIFO** (first in, first out) ordering
- Front/rear index management in a linear array
- Overflow and underflow checks

> [!NOTE]
> This is a linear (non-circular) queue kept as a learning snapshot: slots freed by `dequeue` aren't reused, and the source is in its original classroom form, so it may need small fixes (explicit return types, the stray line inside `main`) to compile on modern compilers.

---

<div align="center">

**By [Intikhab Azam](https://github.com/intikhab49)** — AI & automation engineer

<sub>Keywords: queue in C++ · array implementation of queue · data structures and algorithms · enqueue dequeue · FIFO · DSA lab</sub>

</div>
