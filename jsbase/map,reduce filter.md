如何使用 map() 方法
假设你有一个数组 arrOne，你在其中存储了一些数字，你想对每一个数字进行一些计算，但你也不想弄乱原始数组。
这就是 map() 出现的地方。map() 方法将帮助你做到这一点。

，map() 方法将从索引 [0] 开始挑选该数组的每个值，并对每个值执行所需的计算。然后，它将用计算后的值组成一个新的数组。
 So, the map() method will pick each value of that array starting from the index[0] and perform the desired calculation on each value. Then it'll form a new array with the calculated values.

重要的是：注意我是如何强调不改变原始数组的。这是因为这个属性使 map() 方法与 forEach() 方法不同。map() 方法会产生一个新的数组，而 forEach()  方法会用计算出的数组改变原始数组
Important: Notice how I’m stressing not changing the original array. That is because this property is what makes the map() method different from the ‘forEach()’ method. The map() method makes a new array whereas the ‘forEach()’ method mutates/changes the original array with the calculated array.

[1, 4, 6, 14, 32, 78].map(val => val * 10)
// the result is: [10, 40, 60, 140, 320, 780]


如何使用 filter() 方法
这个名字有点暴露了它，不是吗？你用这个方法根据你提供的条件来过滤数组。 filter() 方法也会创建一个新的数组。
让我们举个例子：假设你有一个数组 arrName，这个数组存储了一堆数字。现在，你想看看哪些数字可以被 3 整除，并将它们组成一个单独的数组。

How to Use the filter() Method
The name kind of gives it away, doesn't it? You use this method to filter the array based on conditions you provide. The filter() method also creates a new array.
Let’s take an example: Suppose you have an array arrName and that array stores a bunch of numbers. Now, you would like to see what numbers can be divided by 3 and make a separate array from them.

所以，filter() 方法将从index[0] 开始挑选该数组的每个值，并对每个值进行操作。然后，它将用计算出来的值形成一个新的数组。
So, the filter() method will pick each value of that array starting from the index[0] and perform the operation on each value. Then it'll form a new array with the calculated values.

[1, 4, 6, 14, 32, 78].filter(val => val > 10)
// the result is: [14, 32, 78]


如何使用 reduce() 方法
假设您被要求求出一个数组所有元素的总和。现在，您可以使用 for 循环或 forEach() 方法，但 reduce 是为此类任务构建的。
该reduce()方法通过对元素共同执行所需的操作来将数组缩减为单个值。
让我们以上面的例子为例并对其使用 reduce ：
这里，reduce 有两个参数，a1和a2，其中a1充当累加器，而a2具有索引值。
现在，在第一次运行时，累加器等于零并a2保存数组的第一个元素。reduce 所做的是将 a2 保存的累加器中的值抛出并将其递增到下一个。之后，reduce() 方法对两个操作数执行操作。在这种情况下，它是加法。

How to Use the reduce() Method
Let’s say you are asked to find the sum of all elements of an array. Now, you could use a for loop or the forEach() method, but reduce is built for this kind of task.
The reduce() method reduces an array to a single value by performing the desired operation on the elements collectively.
Let’s take the above example and use reduce on it:
Now, on the first run the accumulator is equal to zero and a2 holds the first element of the array. What reduce does is that it throws the value in the accumulator that a2 holds and increments it to the next one. After that, the reduce() method performs the operation on both operands. In this case it is addition.

