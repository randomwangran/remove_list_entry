
# Table of Contents

1.  [remove a linked list](#orgc1bcf95)

<https://github.com/jiahao42/blog/issues/1>


<a id="orgc1bcf95"></a>

# remove a linked list

It seems that when one element is deleting from a list, one can change
the content of address. This address was originally pointed to the
element that was set to be deleted.

This inlines with what someone expected to see:

> 此时我们只需将被删除节点的前置节点的next指针指向被删除节点的后置节点即可

This manipulation uses the address info of the next element to the
deleted element. The new address info will overwrite the previous
element to the deleted element.

> 直接将需要被删除节点的后置节点的next地址复制到被删除节点的前置
> 节点的next指针上，无需考虑被删除节点是否是head这个问题

What is the real life example of such a manipulation?
