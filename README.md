### 7.2 李白买酒

李白街上走，提壶去买酒。

遇店加一倍，见花喝一斗。

三遇店和花，喝光壶中酒。

诚问酒壶中，原有多少酒。

```c++
int main()
{
	double x=0 ;                    //最终剩下0斗酒
	int count = 0;                  //遇到店的次数
	int flowercount = 0;            //遇到花的次数

	while (1) {
		x++;
		flowercount++;

		x = x/2 ;
		count++;

		if (count == 3 && flowercount == 3) {
			break;
		}
	}
	cout << x << endl;
	return 0;
}
```

```
0.875
```

思路：倒叙循环
