# Python-to-Golang-note

### list append
#### python
```
_list = []
_list.append(1)
# _list = [1]
```

#### go
```
var list []int
list = append(list, 1)
// list = [1]
```
---
### list remove
#### python
```
_list = [1, 2, 3]
_list.remove(1)  # value
# _list = [2, 3]
_list.pop(1)  # index
# _list = [2]
```

#### go
```
list := []int{1, 2, 3}
list = append(list[:1], list[2:]...)
// list = [1 3]
```
---
### list find element
#### python
```
_list = [1, 2, 3, 4]
_list.index(2)  # find by value, return index
```

####
go
```
list := []int{1, 2, 3, 4}
var position int

for index, value := range list {
    if value == 2 {
        position = index
    }
}
```
