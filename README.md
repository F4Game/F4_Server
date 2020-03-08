# F4_Server

## 代码规范

# python

## 基本数据类型

类型 | 格式 | 示例
---|--- |---
函数（共有） | func_todo_somthing |look_npc
函数（私有） | _func_todo_somthing|_write_to_file
变量（共有） | type_name|i_cnt、s_name、lst_name、set_id、dict_date、tpl_ids、b_result、f_number、bt_byte
变量（私有） | _type_name|_i_cnt、_s_name、_lst_name、_set_id、_dict_date、_tpl_ids
类（公有） | CName|CPlayer
类（私有） | _CName|_CPlayer
全局变量 |g_name|g_member
枚举类型（公有) | NAME_NAME|MAX_NUMBER
枚举类型（私有) | _NAME_NAME|_MAX_NUMBER
类变量 | m_name| m_reward
类实例 | o_name| o_player
临时变量 | name| number
## if else

```
#变量不加类型修饰，不要带有下划线
# 实例 playername、userinfo
if name in lst_name:
    print(name)
else:
    return
```

## 函数参数

```
def func_add(number1,number2)
    return number1+number2
    
def func_add(n1,n2)
    return n1+n2
```

## 类
```
class CPlayer(object):
    m_id = 1
    m_age = 18
    def __init__(self,name):
        self.m_sex = 1
        self.m_child = CChildren()
        self.m_info = {
            "Height" : 170,
            "Weight" : 65,
        }
        self.m_name = name
    
    def say(message):
        print(message)
        
    def _open_eyes():
        pass
    
    def look():
        self._open_eyes()
```

## 注释
```
# todo 2020-3-8 记得祝母亲节日快乐 [author-name]

"""
content
"""

def func(name, age):
    """
    
    :param name: 
    :param age: 
    :return: 
    """
    return name, age

```

## key
```
# key不需要多余内容，首字母大写，驼峰命名即可，记得最后一个也要补上`,`号
dict_info = {
    "Height" : 170,
    "Weight" : 65,
}
```

## import
```
import os
import sys
from math import exp
from math import 
from math import expm1 as ep1

# 尽量少用
from math import *
```
