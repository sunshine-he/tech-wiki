# Get Started

## 代码高亮

```python
print('hello world!')

class LinkList:

    def __init__(self):
        self.head = Node(None)

    def init_list(self, list_target):
        p = self.head
        for i in list_target:
            p.next = Node(i)
            p = p.next
```

## 漂亮的提示信息
!!! note "这是 note 类型的提示框"

!!! success "这是 success 类型的提示框"

!!! failure "这是 failure 类型的提示框"

!!! bug "这是 bug 类型的提示框"

!!! tip "这里是普通提示信息"

