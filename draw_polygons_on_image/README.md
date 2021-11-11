To draw polygons depending on an array. And draw the polygons on an image using matplotlib you can use this.
Note : Append the first coordinate to the list to create a closed loop.

```
import matplotlib.pyplot as plt

test = [[26, 77], [26, 78], [26, 79], [26, 80], [26, 81]]
test.append(test[0])

xs, ys = zip(*test)

plt.plot(xs,ys)
```

![image](https://user-images.githubusercontent.com/42489236/141278032-704c5cb4-d100-4d5f-bc8a-a34647473b83.png)

I solved this problem with the help of this stackoverflow topic : https://stackoverflow.com/questions/43971259/how-to-draw-polygons-with-python
