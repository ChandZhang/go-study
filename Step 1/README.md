 Step 1
========================================

value, ok := myMap[key]
if ok {
}

关键字 func 、函数名、参数列表、返回值、函数体和返回语句。

小写字母开头的函数只在本包内可见，大写字母开头的函数才能被其他包使用


```
	func MyPrintf(args ...interface{}) {
		for _, arg := range args {
			switch arg.(type) {
				case int:
				fmt.Println(arg, "is an int value.")
				case string:
				fmt.Println(arg, "is a string value.")
				case int64:
				fmt.Println(arg, "is an int64 value.")
				default:
				fmt.Println(arg, "is an unknown type.")
			}
		}
	}
```

