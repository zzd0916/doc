## javascript执行编译重要知识点

### 要点记录

- 函数提升高于变量提升
- 后面的函数提升会覆盖前面的变量提升
- 变量提升相当于变量初始值为undefined
- a(){} 及 a:()=>{} 两种方式定义的函数，不能使用new，会报错
- 方法被谁调用，this就指向谁
- var a = function g(){},此时g是只读的，只能在函数内部访问
- new foo()时，内部函数的this指向当前函数的构造函数
- 箭头函数this会指向其父级



### 题目
1. 依次输出什么？ <br>
    ``` 
    alert(a)
    a();
    var a = 3;
    function a(){
        alert(4)
    }
    alert(a)
    a=6;
    a();
    ```

2. 依次输出什么？ <br>
    ```
    var a = function b(num){
        b = num;
        console.log(typeof b)
    }
    a(1);
    console.log(typeof b)
    ```

2. 依次输出什么？ <br>
    ```
    this.a = "进击的小牛牛";
    var test = function() {
        a: 40,
        init: ()=> {
            function go() {
                console.log(this.a)
            }
            go.prototype.a = 20;
            return go
        }
    }
    var fn = test.init;
    fn();
    ```
3. 依次输出什么？ <br>
    ```
    this.a = "进击的小牛牛";
    var test = function() {
        a: 40,
        init: ()=> {
            function go() {
                console.log(this.a)
            }
            go.prototype.a = 20;
            return go
        }
    };
    (function(){
        var fn = test.init;
        fn();
    })()
    ```
