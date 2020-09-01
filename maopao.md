### 时间复杂度

1.如果我们的数据正序，只需要走一趟即可完成排序。所需的比较次数C和记录移动次数M均达到最小值，即：Cmin=n-1;Mmin=0;所以，冒泡排序最好的时间复杂度为O(n)。

2.如果很不幸我们的数据是反序的，则需要进行n-1趟排序。每趟排序要进行n-i次比较(1≤i≤n-1)，且每次比较都必须移动记录三次来达到交换记录位置。在这种情况下，比较和移动次数均达到最大值：
综上所述：冒泡排序总的平均时间复杂度为：O(n2) ,时间复杂度和数据状况无关。

```py
i = input()
        a = i.split(',')
        for aidx in range(len(a)):

            for idx, item in enumerate(a):
                if idx < len(a)-1-aidx:
                    if item > a[idx+1]:
                        a[idx] = a[idx+1]
                        a[idx+1] = item
                else:
                    break
        print(a)

```
